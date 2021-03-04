
---
title: "ManagementAssociation"
title_tag: "azure-native.operationsmanagement.ManagementAssociation"
meta_desc: "Documentation for the azure-native.operationsmanagement.ManagementAssociation resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

The container for solution.
API Version: 2015-11-01-preview.

{{% examples %}}
## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}
### SolutionCreate
{{% example csharp %}}
```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var managementAssociation = new AzureNative.OperationsManagement.ManagementAssociation("managementAssociation", new AzureNative.OperationsManagement.ManagementAssociationArgs
        {
            Location = "East US",
            ManagementAssociationName = "managementAssociation1",
            Properties = new AzureNative.OperationsManagement.Inputs.ManagementAssociationPropertiesArgs
            {
                ApplicationId = "/subscriptions/sub1/resourcegroups/rg1/providers/Microsoft.Appliance/Appliances/appliance1",
            },
            ProviderName = "providerName",
            ResourceGroupName = "rg1",
            ResourceName = "resourceName",
            ResourceType = "resourceType",
        });
    }

}

```

{{% /example %}}

{{% example go %}}

```go
package main

import (
	operationsmanagement "github.com/pulumi/pulumi-azure-native/sdk/go/azure/operationsmanagement"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := operationsmanagement.NewManagementAssociation(ctx, "managementAssociation", &operationsmanagement.ManagementAssociationArgs{
			Location:                  pulumi.String("East US"),
			ManagementAssociationName: pulumi.String("managementAssociation1"),
			Properties: &operationsmanagement.ManagementAssociationPropertiesArgs{
				ApplicationId: pulumi.String("/subscriptions/sub1/resourcegroups/rg1/providers/Microsoft.Appliance/Appliances/appliance1"),
			},
			ProviderName:      pulumi.String("providerName"),
			ResourceGroupName: pulumi.String("rg1"),
			ResourceName:      pulumi.String("resourceName"),
			ResourceType:      pulumi.String("resourceType"),
		})
		if err != nil {
			return err
		}
		return nil
	})
}

```

{{% /example %}}

{{% example python %}}

```python
import pulumi
import pulumi_azure_native as azure_native

management_association = azure_native.operationsmanagement.ManagementAssociation("managementAssociation",
    location="East US",
    management_association_name="managementAssociation1",
    properties=azure_native.operationsmanagement.ManagementAssociationPropertiesArgs(
        application_id="/subscriptions/sub1/resourcegroups/rg1/providers/Microsoft.Appliance/Appliances/appliance1",
    ),
    provider_name="providerName",
    resource_group_name="rg1",
    resource_name="resourceName",
    resource_type="resourceType")

```

{{% /example %}}

{{% example typescript %}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const managementAssociation = new azure_native.operationsmanagement.ManagementAssociation("managementAssociation", {
    location: "East US",
    managementAssociationName: "managementAssociation1",
    properties: {
        applicationId: "/subscriptions/sub1/resourcegroups/rg1/providers/Microsoft.Appliance/Appliances/appliance1",
    },
    providerName: "providerName",
    resourceGroupName: "rg1",
    resourceName: "resourceName",
    resourceType: "resourceType",
});

```

{{% /example %}}

{{% /examples %}}


## Create a ManagementAssociation Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">ManagementAssociation</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">ManagementAssociationArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">ManagementAssociation</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">location</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">management_association_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">properties</span><span class="p">:</span> <span class="nx">Optional[ManagementAssociationPropertiesArgs]</span> = None<span class="p">, </span><span class="nx">provider_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_name_</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_type</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewManagementAssociation</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">ManagementAssociationArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">ManagementAssociation</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">ManagementAssociation</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">ManagementAssociationArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ManagementAssociationArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language python %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type">
            <a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a>
        </span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
  
    <dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>
      Context object for the current deployment.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ManagementAssociationArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ManagementAssociationArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

## ManagementAssociation Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The ManagementAssociation resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="providername_csharp">
<a href="#providername_csharp" style="color: inherit; text-decoration: inherit;">Provider<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Provider name for the parent resource.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group to get. The name is case insensitive.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcename_csharp">
<a href="#resourcename_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Parent resource name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcetype_csharp">
<a href="#resourcetype_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type for the parent resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="location_csharp">
<a href="#location_csharp" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="managementassociationname_csharp">
<a href="#managementassociationname_csharp" style="color: inherit; text-decoration: inherit;">Management<wbr>Association<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User ManagementAssociation Name.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="properties_csharp">
<a href="#properties_csharp" style="color: inherit; text-decoration: inherit;">Properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#managementassociationproperties">Pulumi.<wbr>Azure<wbr>Native.<wbr>Operations<wbr>Management.<wbr>Inputs.<wbr>Management<wbr>Association<wbr>Properties<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Properties for ManagementAssociation object supported by the OperationsManagement resource provider.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="providername_go">
<a href="#providername_go" style="color: inherit; text-decoration: inherit;">Provider<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Provider name for the parent resource.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group to get. The name is case insensitive.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcename_go">
<a href="#resourcename_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Parent resource name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcetype_go">
<a href="#resourcetype_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type for the parent resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="location_go">
<a href="#location_go" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="managementassociationname_go">
<a href="#managementassociationname_go" style="color: inherit; text-decoration: inherit;">Management<wbr>Association<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User ManagementAssociation Name.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="properties_go">
<a href="#properties_go" style="color: inherit; text-decoration: inherit;">Properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#managementassociationproperties">Management<wbr>Association<wbr>Properties</a></span>
    </dt>
    <dd>{{% md %}}Properties for ManagementAssociation object supported by the OperationsManagement resource provider.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="providername_nodejs">
<a href="#providername_nodejs" style="color: inherit; text-decoration: inherit;">provider<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Provider name for the parent resource.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group to get. The name is case insensitive.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcename_nodejs">
<a href="#resourcename_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Parent resource name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcetype_nodejs">
<a href="#resourcetype_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type for the parent resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="location_nodejs">
<a href="#location_nodejs" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="managementassociationname_nodejs">
<a href="#managementassociationname_nodejs" style="color: inherit; text-decoration: inherit;">management<wbr>Association<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User ManagementAssociation Name.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="properties_nodejs">
<a href="#properties_nodejs" style="color: inherit; text-decoration: inherit;">properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#managementassociationproperties">Management<wbr>Association<wbr>Properties</a></span>
    </dt>
    <dd>{{% md %}}Properties for ManagementAssociation object supported by the OperationsManagement resource provider.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="provider_name_python">
<a href="#provider_name_python" style="color: inherit; text-decoration: inherit;">provider_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Provider name for the parent resource.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group to get. The name is case insensitive.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resource_name_python">
<a href="#resource_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Parent resource name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resource_type_python">
<a href="#resource_type_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource type for the parent resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="location_python">
<a href="#location_python" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="management_association_name_python">
<a href="#management_association_name_python" style="color: inherit; text-decoration: inherit;">management_<wbr>association_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}User ManagementAssociation Name.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="properties_python">
<a href="#properties_python" style="color: inherit; text-decoration: inherit;">properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#managementassociationproperties">Management<wbr>Association<wbr>Properties<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Properties for ManagementAssociation object supported by the OperationsManagement resource provider.{{% /md %}}</dd>
</dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the ManagementAssociation resource produces the following output properties:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource name.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}







## Supporting Types



<h4 id="managementassociationproperties">Management<wbr>Association<wbr>Properties</h4>

{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="applicationid_csharp">
<a href="#applicationid_csharp" style="color: inherit; text-decoration: inherit;">Application<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="applicationid_go">
<a href="#applicationid_go" style="color: inherit; text-decoration: inherit;">Application<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="applicationid_nodejs">
<a href="#applicationid_nodejs" style="color: inherit; text-decoration: inherit;">application<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="application_id_python">
<a href="#application_id_python" style="color: inherit; text-decoration: inherit;">application_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

<h4 id="managementassociationpropertiesresponse">Management<wbr>Association<wbr>Properties<wbr>Response</h4>

{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="applicationid_csharp">
<a href="#applicationid_csharp" style="color: inherit; text-decoration: inherit;">Application<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="applicationid_go">
<a href="#applicationid_go" style="color: inherit; text-decoration: inherit;">Application<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="applicationid_nodejs">
<a href="#applicationid_nodejs" style="color: inherit; text-decoration: inherit;">application<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="application_id_python">
<a href="#application_id_python" style="color: inherit; text-decoration: inherit;">application_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The applicationId of the appliance for this association.{{% /md %}}</dd>
</dl>
{{% /choosable %}}
## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:operationsmanagement:ManagementAssociation managementAssociation1 /subscriptions/subid/resourcegroups/rg1/providers/Microsoft.OperationalInsights/workspaces/ws1/Microsoft.OperationsManagement/ManagementAssociations/managementAssociation1 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>
