
---
title: "Backup"
title_tag: "google-native.file/v1beta1.Backup"
meta_desc: "Documentation for the google-native.file/v1beta1.Backup resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Creates a backup.




## Create a Backup Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">Backup</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">,</span> <span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">BackupArgs</a></span><span class="p">,</span> <span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class=nd>@overload</span>
<span class="k">def </span><span class="nx">Backup</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">,</span>
           <span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">,</span>
           <span class="nx">backup_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
           <span class="nx">backups_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
           <span class="nx">description</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
           <span class="nx">labels</span><span class="p">:</span> <span class="nx">Optional[Mapping[str, str]]</span> = None<span class="p">,</span>
           <span class="nx">locations_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
           <span class="nx">projects_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
           <span class="nx">source_file_share</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
           <span class="nx">source_instance</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span>
<span class=nd>@overload</span>
<span class="k">def </span><span class="nx">Backup</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">,</span>
           <span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">BackupArgs</a></span><span class="p">,</span>
           <span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewBackup</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">,</span> <span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">,</span> <span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">BackupArgs</a></span><span class="p">,</span> <span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">Backup</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">Backup</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">,</span> <span class="nx"><a href="#inputs">BackupArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">,</span> <span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">BackupArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

{{% /choosable %}}

{{% choosable language python %}}

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">BackupArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties"><dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>Context object for the current deployment.</dd><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">BackupArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">BackupArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

{{% /choosable %}}

## Backup Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The Backup resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="backupid_csharp">
<a href="#backupid_csharp" style="color: inherit; text-decoration: inherit;">Backup<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="backupsid_csharp">
<a href="#backupsid_csharp" style="color: inherit; text-decoration: inherit;">Backups<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="locationsid_csharp">
<a href="#locationsid_csharp" style="color: inherit; text-decoration: inherit;">Locations<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="projectsid_csharp">
<a href="#projectsid_csharp" style="color: inherit; text-decoration: inherit;">Projects<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="description_csharp">
<a href="#description_csharp" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A description of the backup with 2048 characters or less. Requests with longer descriptions will be rejected.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="labels_csharp">
<a href="#labels_csharp" style="color: inherit; text-decoration: inherit;">Labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}Resource labels to represent user provided metadata.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="sourcefileshare_csharp">
<a href="#sourcefileshare_csharp" style="color: inherit; text-decoration: inherit;">Source<wbr>File<wbr>Share</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the file share in the source Cloud Filestore instance that the backup is created from.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="sourceinstance_csharp">
<a href="#sourceinstance_csharp" style="color: inherit; text-decoration: inherit;">Source<wbr>Instance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource name of the source Cloud Filestore instance, in the format projects/{project_id}/locations/{location_id}/instances/{instance_id}, used to create this backup.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="backupid_go">
<a href="#backupid_go" style="color: inherit; text-decoration: inherit;">Backup<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="backupsid_go">
<a href="#backupsid_go" style="color: inherit; text-decoration: inherit;">Backups<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="locationsid_go">
<a href="#locationsid_go" style="color: inherit; text-decoration: inherit;">Locations<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="projectsid_go">
<a href="#projectsid_go" style="color: inherit; text-decoration: inherit;">Projects<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="description_go">
<a href="#description_go" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A description of the backup with 2048 characters or less. Requests with longer descriptions will be rejected.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="labels_go">
<a href="#labels_go" style="color: inherit; text-decoration: inherit;">Labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}Resource labels to represent user provided metadata.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="sourcefileshare_go">
<a href="#sourcefileshare_go" style="color: inherit; text-decoration: inherit;">Source<wbr>File<wbr>Share</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the file share in the source Cloud Filestore instance that the backup is created from.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="sourceinstance_go">
<a href="#sourceinstance_go" style="color: inherit; text-decoration: inherit;">Source<wbr>Instance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource name of the source Cloud Filestore instance, in the format projects/{project_id}/locations/{location_id}/instances/{instance_id}, used to create this backup.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="backupid_nodejs">
<a href="#backupid_nodejs" style="color: inherit; text-decoration: inherit;">backup<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="backupsid_nodejs">
<a href="#backupsid_nodejs" style="color: inherit; text-decoration: inherit;">backups<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="locationsid_nodejs">
<a href="#locationsid_nodejs" style="color: inherit; text-decoration: inherit;">locations<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="projectsid_nodejs">
<a href="#projectsid_nodejs" style="color: inherit; text-decoration: inherit;">projects<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="description_nodejs">
<a href="#description_nodejs" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A description of the backup with 2048 characters or less. Requests with longer descriptions will be rejected.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="labels_nodejs">
<a href="#labels_nodejs" style="color: inherit; text-decoration: inherit;">labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}Resource labels to represent user provided metadata.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="sourcefileshare_nodejs">
<a href="#sourcefileshare_nodejs" style="color: inherit; text-decoration: inherit;">source<wbr>File<wbr>Share</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the file share in the source Cloud Filestore instance that the backup is created from.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="sourceinstance_nodejs">
<a href="#sourceinstance_nodejs" style="color: inherit; text-decoration: inherit;">source<wbr>Instance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource name of the source Cloud Filestore instance, in the format projects/{project_id}/locations/{location_id}/instances/{instance_id}, used to create this backup.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="backup_id_python">
<a href="#backup_id_python" style="color: inherit; text-decoration: inherit;">backup_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="backups_id_python">
<a href="#backups_id_python" style="color: inherit; text-decoration: inherit;">backups_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="locations_id_python">
<a href="#locations_id_python" style="color: inherit; text-decoration: inherit;">locations_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="projects_id_python">
<a href="#projects_id_python" style="color: inherit; text-decoration: inherit;">projects_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="description_python">
<a href="#description_python" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A description of the backup with 2048 characters or less. Requests with longer descriptions will be rejected.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="labels_python">
<a href="#labels_python" style="color: inherit; text-decoration: inherit;">labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}Resource labels to represent user provided metadata.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="source_file_share_python">
<a href="#source_file_share_python" style="color: inherit; text-decoration: inherit;">source_<wbr>file_<wbr>share</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the file share in the source Cloud Filestore instance that the backup is created from.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="source_instance_python">
<a href="#source_instance_python" style="color: inherit; text-decoration: inherit;">source_<wbr>instance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The resource name of the source Cloud Filestore instance, in the format projects/{project_id}/locations/{location_id}/instances/{instance_id}, used to create this backup.{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the Backup resource produces the following output properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="capacitygb_csharp">
<a href="#capacitygb_csharp" style="color: inherit; text-decoration: inherit;">Capacity<wbr>Gb</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Capacity of the source file share when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="createtime_csharp">
<a href="#createtime_csharp" style="color: inherit; text-decoration: inherit;">Create<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="downloadbytes_csharp">
<a href="#downloadbytes_csharp" style="color: inherit; text-decoration: inherit;">Download<wbr>Bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Amount of bytes that will be downloaded if the backup is restored{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource name of the backup, in the format projects/{project_id}/locations/{location_id}/backups/{backup_id}.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sourceinstancetier_csharp">
<a href="#sourceinstancetier_csharp" style="color: inherit; text-decoration: inherit;">Source<wbr>Instance<wbr>Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The service tier of the source Cloud Filestore instance that this backup is created from.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="state_csharp">
<a href="#state_csharp" style="color: inherit; text-decoration: inherit;">State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The backup state.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="storagebytes_csharp">
<a href="#storagebytes_csharp" style="color: inherit; text-decoration: inherit;">Storage<wbr>Bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The size of the storage used by the backup. As backups share storage, this number is expected to change with backup creation/deletion.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="capacitygb_go">
<a href="#capacitygb_go" style="color: inherit; text-decoration: inherit;">Capacity<wbr>Gb</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Capacity of the source file share when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="createtime_go">
<a href="#createtime_go" style="color: inherit; text-decoration: inherit;">Create<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="downloadbytes_go">
<a href="#downloadbytes_go" style="color: inherit; text-decoration: inherit;">Download<wbr>Bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Amount of bytes that will be downloaded if the backup is restored{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource name of the backup, in the format projects/{project_id}/locations/{location_id}/backups/{backup_id}.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sourceinstancetier_go">
<a href="#sourceinstancetier_go" style="color: inherit; text-decoration: inherit;">Source<wbr>Instance<wbr>Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The service tier of the source Cloud Filestore instance that this backup is created from.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="state_go">
<a href="#state_go" style="color: inherit; text-decoration: inherit;">State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The backup state.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="storagebytes_go">
<a href="#storagebytes_go" style="color: inherit; text-decoration: inherit;">Storage<wbr>Bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The size of the storage used by the backup. As backups share storage, this number is expected to change with backup creation/deletion.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="capacitygb_nodejs">
<a href="#capacitygb_nodejs" style="color: inherit; text-decoration: inherit;">capacity<wbr>Gb</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Capacity of the source file share when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="createtime_nodejs">
<a href="#createtime_nodejs" style="color: inherit; text-decoration: inherit;">create<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="downloadbytes_nodejs">
<a href="#downloadbytes_nodejs" style="color: inherit; text-decoration: inherit;">download<wbr>Bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Amount of bytes that will be downloaded if the backup is restored{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource name of the backup, in the format projects/{project_id}/locations/{location_id}/backups/{backup_id}.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sourceinstancetier_nodejs">
<a href="#sourceinstancetier_nodejs" style="color: inherit; text-decoration: inherit;">source<wbr>Instance<wbr>Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The service tier of the source Cloud Filestore instance that this backup is created from.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="state_nodejs">
<a href="#state_nodejs" style="color: inherit; text-decoration: inherit;">state</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The backup state.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="storagebytes_nodejs">
<a href="#storagebytes_nodejs" style="color: inherit; text-decoration: inherit;">storage<wbr>Bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The size of the storage used by the backup. As backups share storage, this number is expected to change with backup creation/deletion.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="capacity_gb_python">
<a href="#capacity_gb_python" style="color: inherit; text-decoration: inherit;">capacity_<wbr>gb</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Capacity of the source file share when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="create_time_python">
<a href="#create_time_python" style="color: inherit; text-decoration: inherit;">create_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The time when the backup was created.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="download_bytes_python">
<a href="#download_bytes_python" style="color: inherit; text-decoration: inherit;">download_<wbr>bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Amount of bytes that will be downloaded if the backup is restored{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The resource name of the backup, in the format projects/{project_id}/locations/{location_id}/backups/{backup_id}.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="source_instance_tier_python">
<a href="#source_instance_tier_python" style="color: inherit; text-decoration: inherit;">source_<wbr>instance_<wbr>tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The service tier of the source Cloud Filestore instance that this backup is created from.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="state_python">
<a href="#state_python" style="color: inherit; text-decoration: inherit;">state</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The backup state.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="storage_bytes_python">
<a href="#storage_bytes_python" style="color: inherit; text-decoration: inherit;">storage_<wbr>bytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The size of the storage used by the backup. As backups share storage, this number is expected to change with backup creation/deletion.{{% /md %}}</dd></dl>
{{% /choosable %}}








<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-google-native">https://github.com/pulumi/pulumi-google-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

