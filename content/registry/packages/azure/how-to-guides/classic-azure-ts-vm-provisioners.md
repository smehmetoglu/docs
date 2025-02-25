---
title: "Azure WebServer with Manual Provisioning | TypeScript"
h1: "Azure WebServer with Manual Provisioning"
linktitle: "Azure WebServer with Manual Provisioning"
no_edit_this_page: true
cloud: classic-azure
language: ts
layout: how-to-guide
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/mktutorial. -->

<p class="mb-4 flex">
    <a class="flex flex-wrap items-center rounded text-xs text-white bg-blue-600 border-2 border-blue-600 px-2 mr-2 whitespace-no-wrap hover:text-white" style="height: 32px" href="https://github.com/pulumi/examples/tree/master/classic-azure-ts-vm-provisioners" target="_blank">
        <span><i class="fab fa-github pr-2"></i> View Code</span>
    </a>
</p>


This demonstrates using Pulumi dynamic providers to accomplish post-provisioning configuration steps.

Using these building blocks, one can accomplish much of the same as Terraform provisioners.

https://github.com/pulumi/pulumi/issues/1691 tracks designing and developing a complete replacement for provisioners.

## Running the Example

First, create a stack, using `pulumi stack init`.

Now, we need to ensure that our dependencies are installed:

```
$ npm install
``` 


You'll need to log in to the azure cli. You will be prompted to do this during deployment if you forget this step.

```
$ az login
```

We'll need to set some config for login credentials, and location information.

```
pulumi config set azure:location westus
pulumi config set username <your_username>
pulumi config set password --secret <your_desired_password>

```

Next, generate an OpenSSH keypair for use with your server - as per the Azure [Requirements][1]

```
$ ssh-keygen -t rsa -f rsa -m PEM
```

This will output two files, `rsa` and `rsa.pub`, in the current directory. Be sure not to commit these files!

We then need to configure our stack so that the public key is used by our VM, and the private key used
for subsequent SCP and SSH steps to configure our server after it is stood up.

```
$ cat rsa.pub | pulumi config set publicKey --
$ cat rsa | pulumi config set privateKey --secret --
```

If your key is protected by a passphrase, add that too:

```
$ pulumi config set privateKeyPassphrase --secret [yourPassphraseHere]
```

Notice that we've used `--secret` for both `privateKey` and `privateKeyPassphrase`. This ensures their are
stored in encrypted form in the Pulumi secrets system.


From there, you can run `pulumi up` and all resources will be provisioned and configured.

[1]: https://docs.microsoft.com/en-us/azure/virtual-machines/linux/ssh-from-windows#create-an-ssh-key-pair

