
---
title: "GetUser"
title_tag: "Function GetUser | Module identitystore | Package AWS"
meta_desc: "Explore the GetUser function of the identitystore module, including examples, input properties, output properties, and supporting types. Use this data source to get an Identity Store User."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Use this data source to get an Identity Store User.




## Using GetUser {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getUser<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/identitystore/#GetUserArgs">GetUserArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/identitystore/#GetUserResult">GetUserResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_user(</span><span class="nx">filters</span><span class="p">:</span> <span class="nx">Optional[Sequence[GetUserFilterArgs]]</span> = None<span class="p">, </span><span class="nx">identity_store_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">user_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetUserResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetUser<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/v3/go/aws/identitystore?tab=doc#GetUserArgs">GetUserArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/v3/go/aws/identitystore?tab=doc#GetUserResult">GetUserResult</a></span>, error)</span></code></pre></div>

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetUser </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Identitystore.GetUserResult.html">GetUserResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.IdentityStore.GetUserArgs.html">GetUserArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="filters_csharp">
<a href="#filters_csharp" style="color: inherit; text-decoration: inherit;">Filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">List&lt;Get<wbr>User<wbr>Filter<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}Configuration block(s) for filtering. Currently, the AWS Identity Store API supports only 1 filter. Detailed below.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="identitystoreid_csharp">
<a href="#identitystoreid_csharp" style="color: inherit; text-decoration: inherit;">Identity<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Identity Store ID associated with the Single Sign-On Instance.
{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="userid_csharp">
<a href="#userid_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The identifier for a user in the Identity Store.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="filters_go">
<a href="#filters_go" style="color: inherit; text-decoration: inherit;">Filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">[]Get<wbr>User<wbr>Filter</a></span>
    </dt>
    <dd>{{% md %}}Configuration block(s) for filtering. Currently, the AWS Identity Store API supports only 1 filter. Detailed below.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="identitystoreid_go">
<a href="#identitystoreid_go" style="color: inherit; text-decoration: inherit;">Identity<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Identity Store ID associated with the Single Sign-On Instance.
{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="userid_go">
<a href="#userid_go" style="color: inherit; text-decoration: inherit;">User<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The identifier for a user in the Identity Store.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="filters_nodejs">
<a href="#filters_nodejs" style="color: inherit; text-decoration: inherit;">filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">Get<wbr>User<wbr>Filter[]</a></span>
    </dt>
    <dd>{{% md %}}Configuration block(s) for filtering. Currently, the AWS Identity Store API supports only 1 filter. Detailed below.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="identitystoreid_nodejs">
<a href="#identitystoreid_nodejs" style="color: inherit; text-decoration: inherit;">identity<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Identity Store ID associated with the Single Sign-On Instance.
{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="userid_nodejs">
<a href="#userid_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The identifier for a user in the Identity Store.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="filters_python">
<a href="#filters_python" style="color: inherit; text-decoration: inherit;">filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">Sequence[Get<wbr>User<wbr>Filter<wbr>Args]</a></span>
    </dt>
    <dd>{{% md %}}Configuration block(s) for filtering. Currently, the AWS Identity Store API supports only 1 filter. Detailed below.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="identity_store_id_python">
<a href="#identity_store_id_python" style="color: inherit; text-decoration: inherit;">identity_<wbr>store_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Identity Store ID associated with the Single Sign-On Instance.
{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="user_id_python">
<a href="#user_id_python" style="color: inherit; text-decoration: inherit;">user_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The identifier for a user in the Identity Store.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}




## GetUser Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="filters_csharp">
<a href="#filters_csharp" style="color: inherit; text-decoration: inherit;">Filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">List&lt;Get<wbr>User<wbr>Filter&gt;</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="identitystoreid_csharp">
<a href="#identitystoreid_csharp" style="color: inherit; text-decoration: inherit;">Identity<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="userid_csharp">
<a href="#userid_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="username_csharp">
<a href="#username_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user's user name value.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="filters_go">
<a href="#filters_go" style="color: inherit; text-decoration: inherit;">Filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">[]Get<wbr>User<wbr>Filter</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="identitystoreid_go">
<a href="#identitystoreid_go" style="color: inherit; text-decoration: inherit;">Identity<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="userid_go">
<a href="#userid_go" style="color: inherit; text-decoration: inherit;">User<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="username_go">
<a href="#username_go" style="color: inherit; text-decoration: inherit;">User<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user's user name value.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="filters_nodejs">
<a href="#filters_nodejs" style="color: inherit; text-decoration: inherit;">filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">Get<wbr>User<wbr>Filter[]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="identitystoreid_nodejs">
<a href="#identitystoreid_nodejs" style="color: inherit; text-decoration: inherit;">identity<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="userid_nodejs">
<a href="#userid_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="username_nodejs">
<a href="#username_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user's user name value.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="filters_python">
<a href="#filters_python" style="color: inherit; text-decoration: inherit;">filters</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getuserfilter">Sequence[Get<wbr>User<wbr>Filter]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="identity_store_id_python">
<a href="#identity_store_id_python" style="color: inherit; text-decoration: inherit;">identity_<wbr>store_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="user_id_python">
<a href="#user_id_python" style="color: inherit; text-decoration: inherit;">user_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="user_name_python">
<a href="#user_name_python" style="color: inherit; text-decoration: inherit;">user_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The user's user name value.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}




## Supporting Types


<h4 id="getuserfilter">Get<wbr>User<wbr>Filter</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/aws/types/input/#GetUserFilter">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/aws/types/output/#GetUserFilter">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/v3/go/aws/identitystore?tab=doc#GetUserFilterArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/v3/go/aws/identitystore?tab=doc#GetUserFilter">output</a> API doc for this type.
{{% /choosable %}}
{{% choosable language csharp %}}
> See the <a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.IdentityStore.Inputs.GetUserFilterArgs.html">input</a> and <a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.IdentityStore.Outputs.GetUserFilter.html">output</a> API doc for this type.
{{% /choosable %}}



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="attributepath_csharp">
<a href="#attributepath_csharp" style="color: inherit; text-decoration: inherit;">Attribute<wbr>Path</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The attribute path that is used to specify which attribute name to search. Currently, `UserName` is the only valid attribute path.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="attributevalue_csharp">
<a href="#attributevalue_csharp" style="color: inherit; text-decoration: inherit;">Attribute<wbr>Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The value for an attribute.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="attributepath_go">
<a href="#attributepath_go" style="color: inherit; text-decoration: inherit;">Attribute<wbr>Path</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The attribute path that is used to specify which attribute name to search. Currently, `UserName` is the only valid attribute path.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="attributevalue_go">
<a href="#attributevalue_go" style="color: inherit; text-decoration: inherit;">Attribute<wbr>Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The value for an attribute.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="attributepath_nodejs">
<a href="#attributepath_nodejs" style="color: inherit; text-decoration: inherit;">attribute<wbr>Path</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The attribute path that is used to specify which attribute name to search. Currently, `UserName` is the only valid attribute path.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="attributevalue_nodejs">
<a href="#attributevalue_nodejs" style="color: inherit; text-decoration: inherit;">attribute<wbr>Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The value for an attribute.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="attribute_path_python">
<a href="#attribute_path_python" style="color: inherit; text-decoration: inherit;">attribute_<wbr>path</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The attribute path that is used to specify which attribute name to search. Currently, `UserName` is the only valid attribute path.
{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="attribute_value_python">
<a href="#attribute_value_python" style="color: inherit; text-decoration: inherit;">attribute_<wbr>value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The value for an attribute.
{{% /md %}}</dd>
</dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-aws">https://github.com/pulumi/pulumi-aws</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>This Pulumi package is based on the [`aws` Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws).</dd>
</dl>
