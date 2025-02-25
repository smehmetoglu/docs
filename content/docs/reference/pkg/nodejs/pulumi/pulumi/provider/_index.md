---
title: "Module provider"
title_tag: "Module provider | Package @pulumi/pulumi | Node.js SDK"
linktitle: "provider"
meta_desc: "Explore members of the provider module in the @pulumi/pulumi package."
git_sha: "8ea38f633d472788fea20899fbbb183ff1284561"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

{{< resource-docs-alert "pulumi" >}}






<h3>APIs</h3>
<ul class="api">
    <li><a href="#CheckFailure"><span class="symbol api"></span>CheckFailure</a></li>
    <li><a href="#CheckResult"><span class="symbol api"></span>CheckResult</a></li>
    <li><a href="#ConstructResult"><span class="symbol api"></span>ConstructResult</a></li>
    <li><a href="#CreateResult"><span class="symbol api"></span>CreateResult</a></li>
    <li><a href="#DiffResult"><span class="symbol api"></span>DiffResult</a></li>
    <li><a href="#InvokeResult"><span class="symbol api"></span>InvokeResult</a></li>
    <li><a href="#main"><span class="symbol api"></span>main</a></li>
    <li><a href="#parseArgs"><span class="symbol api"></span>parseArgs</a></li>
    <li><a href="#Provider"><span class="symbol api"></span>Provider</a></li>
    <li><a href="#ReadResult"><span class="symbol api"></span>ReadResult</a></li>
    <li><a href="#UpdateResult"><span class="symbol api"></span>UpdateResult</a></li>
</ul>




<h2 id="apis">APIs</h2>
<h3 class="pdoc-module-header" id="CheckFailure" data-link-title="CheckFailure">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L37">
        interface <strong>CheckFailure</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>CheckFailure</span></code></pre>

CheckFailure represents a single failure in the results of a call to `ResourceProvider.check`

<h4 class="pdoc-member-header" id="CheckFailure-property">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L41">property <b>property</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>property: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The property that failed validation.

<h4 class="pdoc-member-header" id="CheckFailure-reason">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L46">property <b>reason</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>reason: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The reason that the property failed validation.

<h3 class="pdoc-module-header" id="CheckResult" data-link-title="CheckResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L22">
        interface <strong>CheckResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>CheckResult</span></code></pre>

CheckResult represents the results of a call to `ResourceProvider.check`.

<h4 class="pdoc-member-header" id="CheckResult-failures">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L31">property <b>failures</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>failures?: <a href='#CheckFailure'>CheckFailure</a>[];</code></pre>

Any validation failures that occurred.

<h4 class="pdoc-member-header" id="CheckResult-inputs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L26">property <b>inputs</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>inputs?: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>;</code></pre>

The inputs to use, if any.

<h3 class="pdoc-module-header" id="ConstructResult" data-link-title="ConstructResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L114">
        interface <strong>ConstructResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ConstructResult</span></code></pre>

ConstructResult represents the results of a call to `ResourceProvider.construct`.

<h4 class="pdoc-member-header" id="ConstructResult-state">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L123">property <b>state</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>state: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Inputs'>Inputs</a>;</code></pre>

Any state that was computed during construction.

<h4 class="pdoc-member-header" id="ConstructResult-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L118">property <b>urn</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>Input</a>&lt;resource.URN&gt;;</code></pre>

The URN of the constructed resource.

<h3 class="pdoc-module-header" id="CreateResult" data-link-title="CreateResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L78">
        interface <strong>CreateResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>CreateResult</span></code></pre>

CreateResult represents the results of a call to `ResourceProvider.create`.

<h4 class="pdoc-member-header" id="CreateResult-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L82">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: resource.ID;</code></pre>

The ID of the created resource.

<h4 class="pdoc-member-header" id="CreateResult-outs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L87">property <b>outs</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>outs?: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>;</code></pre>

Any properties that were computed during creation.

<h3 class="pdoc-module-header" id="DiffResult" data-link-title="DiffResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L52">
        interface <strong>DiffResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>DiffResult</span></code></pre>

DiffResult represents the results of a call to `ResourceProvider.diff`.

<h4 class="pdoc-member-header" id="DiffResult-changes">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L56">property <b>changes</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>changes?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>;</code></pre>

If true, this diff detected changes and suggests an update.

<h4 class="pdoc-member-header" id="DiffResult-deleteBeforeReplace">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L72">property <b>deleteBeforeReplace</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>deleteBeforeReplace?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>;</code></pre>

If true, and a replacement occurs, the resource will first be deleted before being recreated.  This is to
avoid potential side-by-side issues with the default create before delete behavior.

<h4 class="pdoc-member-header" id="DiffResult-replaces">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L61">property <b>replaces</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>replaces?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];</code></pre>

If this update requires a replacement, the set of properties triggering it.

<h4 class="pdoc-member-header" id="DiffResult-stables">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L66">property <b>stables</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>stables?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];</code></pre>

An optional list of properties that will not ever change.

<h3 class="pdoc-module-header" id="InvokeResult" data-link-title="InvokeResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L129">
        interface <strong>InvokeResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>InvokeResult</span></code></pre>

InvokeResult represents the results of a call to `ResourceProvider.invoke`.

<h4 class="pdoc-member-header" id="InvokeResult-failures">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L138">property <b>failures</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>failures?: <a href='#CheckFailure'>CheckFailure</a>[];</code></pre>

Any validation failures that occurred.

<h4 class="pdoc-member-header" id="InvokeResult-outputs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L133">property <b>outputs</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>outputs?: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>;</code></pre>

The outputs returned by the invoked function, if any.

<h3 class="pdoc-module-header" id="main" data-link-title="main">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/server.ts#L599">
        function <strong>main</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>main(provider: <a href='#Provider'>Provider</a>, args: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[]): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span>&gt;</code></pre>

<h3 class="pdoc-module-header" id="parseArgs" data-link-title="parseArgs">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/internals.ts#L27">
        function <strong>parseArgs</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>parseArgs(args: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[]): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | {
    engineAddress: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
}</code></pre>

<h3 class="pdoc-module-header" id="Provider" data-link-title="Provider">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L144">
        interface <strong>Provider</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>Provider</span></code></pre>

Provider represents an object that implements the resources and functions for a particular Pulumi package.

<h4 class="pdoc-member-header" id="Provider-call">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L220">property <b>call</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>call?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (token: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, inputs: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Inputs'>Inputs</a>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#InvokeResult'>InvokeResult</a>&gt;;</code></pre>

Call calls the indicated method.

<h4 class="pdoc-member-header" id="Provider-check">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L161">property <b>check</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>check?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (urn: resource.URN, olds: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>, news: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#CheckResult'>CheckResult</a>&gt;;</code></pre>

Check validates that the given property bag is valid for a resource of the given type.

<h4 class="pdoc-member-header" id="Provider-construct">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L211">property <b>construct</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>construct?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, type: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, inputs: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Inputs'>Inputs</a>, options: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ComponentResourceOptions'>ComponentResourceOptions</a>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#ConstructResult'>ConstructResult</a>&gt;;</code></pre>

Construct creates a new component resource.

<h4 class="pdoc-member-header" id="Provider-create">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L178">property <b>create</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>create?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (urn: resource.URN, inputs: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#CreateResult'>CreateResult</a>&gt;;</code></pre>

Create allocates a new instance of the provided resource and returns its unique ID afterwards.
If this call fails, the resource must not have been created (i.e., it is "transactional").

<h4 class="pdoc-member-header" id="Provider-delete">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L201">property <b>delete</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>delete?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (id: resource.ID, urn: resource.URN, props: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span>&gt;;</code></pre>

Delete tears down an existing resource with the given ID.  If it fails, the resource is assumed to still exist.

<h4 class="pdoc-member-header" id="Provider-diff">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L170">property <b>diff</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>diff?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (id: resource.ID, urn: resource.URN, olds: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>, news: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#DiffResult'>DiffResult</a>&gt;;</code></pre>

Diff checks what impacts a hypothetical update will have on the resource's properties.

<h4 class="pdoc-member-header" id="Provider-invoke">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L228">property <b>invoke</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>invoke?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (token: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, inputs: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#InvokeResult'>InvokeResult</a>&gt;;</code></pre>

Invoke calls the indicated function.

<h4 class="pdoc-member-header" id="Provider-read">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L184">property <b>read</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>read?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (id: resource.ID, urn: resource.URN, props?: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#ReadResult'>ReadResult</a>&gt;;</code></pre>

Reads the current live state associated with a resource.  Enough state must be included in the inputs to uniquely
identify the resource; this is typically just the resource ID, but it may also include some properties.

<h4 class="pdoc-member-header" id="Provider-schema">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L153">property <b>schema</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>schema?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The JSON-encoded schema for this provider's package.

<h4 class="pdoc-member-header" id="Provider-update">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L193">property <b>update</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>update?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | (id: resource.ID, urn: resource.URN, olds: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>, news: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>) => <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#UpdateResult'>UpdateResult</a>&gt;;</code></pre>

Update updates an existing resource with new values.

<h4 class="pdoc-member-header" id="Provider-version">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L148">property <b>version</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>version: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The version of the provider. Must be valid semver.

<h3 class="pdoc-module-header" id="ReadResult" data-link-title="ReadResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L90">
        interface <strong>ReadResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ReadResult</span></code></pre>
<h4 class="pdoc-member-header" id="ReadResult-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L94">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id?: resource.ID;</code></pre>

The ID of the resource ready back (or blank if missing).

<h4 class="pdoc-member-header" id="ReadResult-props">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L98">property <b>props</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>props?: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>;</code></pre>

The current property state read from the live environment.

<h3 class="pdoc-module-header" id="UpdateResult" data-link-title="UpdateResult">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L104">
        interface <strong>UpdateResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>UpdateResult</span></code></pre>

UpdateResult represents the results of a call to `ResourceProvider.update`.

<h4 class="pdoc-member-header" id="UpdateResult-outs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/provider/provider.ts#L108">property <b>outs</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>outs?: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>;</code></pre>

Any properties that were computed during updating.

