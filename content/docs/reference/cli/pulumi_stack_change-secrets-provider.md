---
title: "pulumi stack change-secrets-provider"
---



Change the secrets provider for the current stack

### Synopsis

Change the secrets provider for the current stack. Valid secret providers types are `default`, `passphrase`, `awskms`, `azurekeyvault`, `gcpkms`, `hashivault`.

To change to using the Pulumi Default Secrets Provider, use the following:

pulumi stack change-secrets-provider default

To change the stack to use a cloud secrets backend, use one of the following:

* `pulumi stack change-secrets-provider "awskms://alias/ExampleAlias?region=us-east-1"`
* `pulumi stack change-secrets-provider "awskms://1234abcd-12ab-34cd-56ef-1234567890ab?region=us-east-1"`
* `pulumi stack change-secrets-provider "azurekeyvault://mykeyvaultname.vault.azure.net/keys/mykeyname"`
* `pulumi stack change-secrets-provider "gcpkms://projects/<p>/locations/<l>/keyRings/<r>/cryptoKeys/<k>"`
* `pulumi stack change-secrets-provider "hashivault://mykey"`

```
pulumi stack change-secrets-provider <new-secrets-provider> [flags]
```

### Options

```
  -h, --help   help for change-secrets-provider
```

### Options inherited from parent commands

```
      --color string                 Colorize output. Choices are: always, never, raw, auto (default "auto")
  -C, --cwd string                   Run pulumi as if it had been started in another directory
      --disable-integrity-checking   Disable integrity checking of checkpoint files
  -e, --emoji                        Enable emojis in the output
      --logflow                      Flow log settings to child processes (like plugins)
      --logtostderr                  Log to stderr instead of to files
      --non-interactive              Disable interactive mode for all commands
      --profiling string             Emit CPU and memory profiles and an execution trace to '[filename].[pid].{cpu,mem,trace}', respectively
  -s, --stack string                 The name of the stack to operate on. Defaults to the current stack
      --tracing file:                Emit tracing to the specified endpoint. Use the file: scheme to write tracing data to a local file
  -v, --verbose int                  Enable verbose logging (e.g., v=3); anything >3 is very verbose
```

### SEE ALSO

* [pulumi stack](/docs/reference/cli/pulumi_stack/)	 - Manage stacks

###### Auto generated by spf13/cobra on 2-Dec-2021
