---
title: "Module config"
title_tag: "Module config | Package @pulumi/rancher2 | Node.js SDK"
linktitle: "config"
meta_desc: "Explore members of the config module in the @pulumi/rancher2 package."
git_sha: "8d8a62ede0219bbed1edb6bdb2938527b62a667d"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-rancher2)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-rancher2` repo](https://github.com/pulumi/pulumi-rancher2/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-rancher2` repo](https://github.com/terraform-providers/terraform-provider-rancher2/issues).







<h3>APIs</h3>
<ul class="api">
    <li><a href="#accessKey"><span class="symbol api"></span>accessKey</a></li>
    <li><a href="#apiUrl"><span class="symbol api"></span>apiUrl</a></li>
    <li><a href="#bootstrap"><span class="symbol api"></span>bootstrap</a></li>
    <li><a href="#caCerts"><span class="symbol api"></span>caCerts</a></li>
    <li><a href="#insecure"><span class="symbol api"></span>insecure</a></li>
    <li><a href="#retries"><span class="symbol api"></span>retries</a></li>
    <li><a href="#secretKey"><span class="symbol api"></span>secretKey</a></li>
    <li><a href="#tokenKey"><span class="symbol api"></span>tokenKey</a></li>
</ul>




<h2 id="apis">APIs</h2>
<h3 class="pdoc-module-header" id="accessKey" data-link-title="accessKey">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L12">
        let <strong>accessKey</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> accessKey: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;accessKey&#34;) || utilities.getEnv(&#34;RANCHER_ACCESS_KEY&#34;)</span>;</code></pre>

API Key used to authenticate with the rancher server

<h3 class="pdoc-module-header" id="apiUrl" data-link-title="apiUrl">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L16">
        let <strong>apiUrl</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> apiUrl: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;apiUrl&#34;) || utilities.getEnv(&#34;RANCHER_URL&#34;)</span>;</code></pre>

The URL to the rancher API

<h3 class="pdoc-module-header" id="bootstrap" data-link-title="bootstrap">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L20">
        let <strong>bootstrap</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> bootstrap: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;boolean&gt;(&#34;bootstrap&#34;) || (utilities.getEnvBoolean(&#34;RANCHER_BOOTSTRAP&#34;) || false)</span>;</code></pre>

Bootstrap rancher server

<h3 class="pdoc-module-header" id="caCerts" data-link-title="caCerts">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L24">
        let <strong>caCerts</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> caCerts: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;caCerts&#34;) || utilities.getEnv(&#34;RANCHER_CA_CERTS&#34;)</span>;</code></pre>

CA certificates used to sign rancher server tls certificates. Mandatory if self signed tls and insecure option false

<h3 class="pdoc-module-header" id="insecure" data-link-title="insecure">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L28">
        let <strong>insecure</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> insecure: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;boolean&gt;(&#34;insecure&#34;) || (utilities.getEnvBoolean(&#34;RANCHER_INSECURE&#34;) || false)</span>;</code></pre>

Allow insecure connections to Rancher. Mandatory if self signed tls and not ca_certs provided

<h3 class="pdoc-module-header" id="retries" data-link-title="retries">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L32">
        let <strong>retries</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> retries: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;number&gt;(&#34;retries&#34;)</span>;</code></pre>

Rancher connection retries

<h3 class="pdoc-module-header" id="secretKey" data-link-title="secretKey">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L36">
        let <strong>secretKey</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> secretKey: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;secretKey&#34;) || utilities.getEnv(&#34;RANCHER_SECRET_KEY&#34;)</span>;</code></pre>

API secret used to authenticate with the rancher server

<h3 class="pdoc-module-header" id="tokenKey" data-link-title="tokenKey">
    <a href="https://github.com/pulumi/pulumi-rancher2/blob/8d8a62ede0219bbed1edb6bdb2938527b62a667d/sdk/nodejs/config/vars.ts#L40">
        let <strong>tokenKey</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kd'>let</span> tokenKey: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;tokenKey&#34;) || utilities.getEnv(&#34;RANCHER_TOKEN_KEY&#34;)</span>;</code></pre>

API token used to authenticate with the rancher server

