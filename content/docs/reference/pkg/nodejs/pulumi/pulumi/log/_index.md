---
title: "Module log"
title_tag: "Module log | Package @pulumi/pulumi | Node.js SDK"
linktitle: "log"
meta_desc: "Explore members of the log module in the @pulumi/pulumi package."
git_sha: "8ea38f633d472788fea20899fbbb183ff1284561"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

{{< resource-docs-alert "pulumi" >}}






<h3>APIs</h3>
<ul class="api">
    <li><a href="#debug"><span class="symbol api"></span>debug</a></li>
    <li><a href="#error"><span class="symbol api"></span>error</a></li>
    <li><a href="#hasErrors"><span class="symbol api"></span>hasErrors</a></li>
    <li><a href="#info"><span class="symbol api"></span>info</a></li>
    <li><a href="#warn"><span class="symbol api"></span>warn</a></li>
</ul>




<h2 id="apis">APIs</h2>
<h3 class="pdoc-module-header" id="debug" data-link-title="debug">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/log/index.ts#L41">
        function <strong>debug</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>debug(msg: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, resource?: resourceTypes.Resource, streamId?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>, ephemeral?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span>&gt;</code></pre>


debug logs a debug-level message that is generally hidden from end-users.

<h3 class="pdoc-module-header" id="error" data-link-title="error">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/log/index.ts#L82">
        function <strong>error</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>error(msg: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, resource?: resourceTypes.Resource, streamId?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>, ephemeral?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span>&gt;</code></pre>


error logs a fatal condition. Consider raising an exception after calling error to stop the Pulumi program.

<h3 class="pdoc-module-header" id="hasErrors" data-link-title="hasErrors">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/log/index.ts#L34">
        function <strong>hasErrors</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>hasErrors(): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></code></pre>


hasErrors returns true if any errors have occurred in the program.

<h3 class="pdoc-module-header" id="info" data-link-title="info">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/log/index.ts#L54">
        function <strong>info</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>info(msg: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, resource?: resourceTypes.Resource, streamId?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>, ephemeral?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span>&gt;</code></pre>


info logs an informational message that is generally printed to stdout during resource operations.

<h3 class="pdoc-module-header" id="warn" data-link-title="warn">
    <a href="https://github.com/pulumi/pulumi/blob/8ea38f633d472788fea20899fbbb183ff1284561/sdk/nodejs/log/index.ts#L68">
        function <strong>warn</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>warn(msg: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, resource?: resourceTypes.Resource, streamId?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>, ephemeral?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span>&gt;</code></pre>


warn logs a warning to indicate that something went wrong, but not catastrophically so.

