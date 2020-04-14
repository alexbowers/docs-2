
---
title: "GetMultiClusterApp"
block_external_search_index: true
---



Use this data source to retrieve information about a Rancher v2 multi cluster app.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as rancher2 from "@pulumi/rancher2";

const foo = pulumi.output(rancher2.getMultiClusterApp({
    name: "foo",
}, { async: true }));
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-rancher2/blob/master/website/docs/d/multiClusterApp.html.markdown.





## Using GetMultiClusterApp

{{< chooser language "javascript,typescript,python,go,csharp" / >}}


{{% choosable language typescript %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getMultiClusterApp<span class="p">(</span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#GetMultiClusterAppArgs">GetMultiClusterAppArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#GetMultiClusterAppResult">GetMultiClusterAppResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">function </span> get_multi_cluster_app(</span>name=None<span class="p">, </span>opts=None<span class="p">)</span></code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupMultiClusterApp<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#GetMultiClusterAppArgs">GetMultiClusterAppArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#LookupMultiClusterAppResult">LookupMultiClusterAppResult</a></span>, error)</span></code></pre></div>
{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetMultiClusterApp </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.GetMultiClusterAppResult.html">GetMultiClusterAppResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.GetMultiClusterAppArgs.html">GetMultiClusterAppArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span>? <span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The multi cluster app name (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The multi cluster app name (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The multi cluster app name (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The multi cluster app name (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## GetMultiClusterApp Result

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Answers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappanswer">List&lt;Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Answer&gt;</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app answers (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Catalog<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app catalog name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}(Computed) Labels for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Members</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappmember">List&lt;Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Member&gt;</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app members (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Revision<wbr>History<wbr>Limit</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app revision history limit (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Revision<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) Current revision id for the multi cluster app (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Roles</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app roles (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Targets</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterapptarget">List&lt;Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Target&gt;</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app target projects (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Template<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Template<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Template<wbr>Version<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Upgrade<wbr>Strategies</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategy">List&lt;Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy&gt;</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app upgrade strategy (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Answers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappanswer">[]Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Answer</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app answers (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Catalog<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app catalog name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Members</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappmember">[]Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Member</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app members (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Revision<wbr>History<wbr>Limit</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app revision history limit (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Revision<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) Current revision id for the multi cluster app (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Roles</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app roles (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Targets</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterapptarget">[]Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app target projects (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Template<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Template<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Template<wbr>Version<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Upgrade<wbr>Strategies</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategy">[]Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app upgrade strategy (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>answers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappanswer">Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Answer[]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app answers (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>catalog<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app catalog name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>members</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappmember">Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Member[]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app members (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>revision<wbr>History<wbr>Limit</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app revision history limit (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>revision<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) Current revision id for the multi cluster app (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>roles</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app roles (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>targets</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterapptarget">Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Target[]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app target projects (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>template<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>template<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>template<wbr>Version<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>upgrade<wbr>Strategies</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategy">Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy[]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app upgrade strategy (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>answers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappanswer">List[Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Answer]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app answers (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>catalog_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app catalog name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels for multi cluster app object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>members</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappmember">List[Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Member]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app members (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>revision_<wbr>history_<wbr>limit</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app revision history limit (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>revision_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) Current revision id for the multi cluster app (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>roles</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app roles (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>targets</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterapptarget">List[Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Target]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app target projects (list)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>template_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>template_<wbr>version</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>template_<wbr>version_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app template version ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>upgrade_<wbr>strategies</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategy">List[Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy]</a></span>
    </dt>
    <dd>{{% md %}}(Computed) The multi cluster app upgrade strategy (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Supporting Types

<h4>Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Answer</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#GetMultiClusterAppAnswer">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#GetMultiClusterAppAnswer">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Values</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Values</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>values</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>project_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>values</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Member</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#GetMultiClusterAppMember">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#GetMultiClusterAppMember">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Access<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Principal<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Principal<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Access<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Principal<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Principal<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>access<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Principal<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Principal<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>access<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>principal_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>principal_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Target</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#GetMultiClusterAppTarget">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#GetMultiClusterAppTarget">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>App<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Health<wbr>State</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>State</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>App<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Health<wbr>State</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>State</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>app<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>health<wbr>State</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>state</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>app<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>health<wbr>State</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>project_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>state</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#GetMultiClusterAppUpgradeStrategy">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#GetMultiClusterAppUpgradeStrategy">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Rolling<wbr>Update</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategyrollingupdate">Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy<wbr>Rolling<wbr>Update<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Rolling<wbr>Update</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategyrollingupdate">*Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy<wbr>Rolling<wbr>Update</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>rolling<wbr>Update</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategyrollingupdate">Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy<wbr>Rolling<wbr>Update?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>rolling<wbr>Update</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getmulticlusterappupgradestrategyrollingupdate">Dict[Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy<wbr>Rolling<wbr>Update]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Get<wbr>Multi<wbr>Cluster<wbr>App<wbr>Upgrade<wbr>Strategy<wbr>Rolling<wbr>Update</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#GetMultiClusterAppUpgradeStrategyRollingUpdate">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#GetMultiClusterAppUpgradeStrategyRollingUpdate">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Batch<wbr>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Batch<wbr>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>batch<wbr>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>batch<wbr>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}






