

# Catalog<a name="catalog_catalog"></a>
    
## DataProviders<a name="catalog_catalog_dataproviders"></a>
### NestedKeyDataProvider<a name="catalog_dataproviders_nestedkeydataprovider"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\DataProviders`





#### Methods

<pre>public <strong>getKey</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getNestedRows</strong>($parentId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$parentId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getNestedData</strong>(<a target="_blank" href="http://php.net/string">string</a> $parentId, <a target="_blank" href="http://php.net/string">string</a> $query = &quot;&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$parentId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getRows</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getDataByValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $id):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>



### BaseDataProvider<a name="catalog_dataproviders_basedataprovider"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\DataProviders`





#### Methods

<pre>public <strong>getRows</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### KeyDataProvider<a name="catalog_dataproviders_keydataprovider"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\DataProviders`





#### Methods

<pre>public <strong>getKey</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getRows</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
## Contracts<a name="catalog_catalog_contracts"></a>
### CatalogExportFilterServiceContract<a name="catalog_contracts_catalogexportfilterservicecontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>applyFilters</strong>(<a href="cloud#cloud_document_documentsearch">DocumentSearch</a>
 $documentSearch, <a target="_blank" href="http://php.net/array">array</a> $config):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_document_documentsearch">DocumentSearch</a>
</td>
        <td>$documentSearch</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$config</td>
        <td></td>
    </tr>
</table>



### CatalogRepositoryContract<a name="catalog_contracts_catalogrepositorycontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="catalog#catalog_models_catalog">Catalog</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $id):<a href="catalog#catalog_models_catalog">Catalog</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $perPage = 25):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the filter array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the filter array.
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### NestedDataProviderContract<a name="catalog_contracts_nesteddataprovidercontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>getNestedData</strong>(<a target="_blank" href="http://php.net/string">string</a> $parentId, <a target="_blank" href="http://php.net/string">string</a> $query = &quot;&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$parentId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDataByValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $id):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getData</strong>(<a target="_blank" href="http://php.net/string">string</a> $query = &quot;&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$query</td>
        <td></td>
    </tr>
</table>



### TemplateContract<a name="catalog_contracts_templatecontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getMappings</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMapping</strong>(<a target="_blank" href="http://php.net/array">array</a> $mapping):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$mapping</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPreMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPostMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addFilter</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getIdentifier</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPreMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPostMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setSkuCallback</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSkuCallback</strong>():<a target="_blank" href="http://php.net/callable">callable</a></pre>

    

    
<pre>public <strong>addSetting</strong>(<a target="_blank" href="http://php.net/array">array</a> $setting):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$setting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSettings</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setMetaInfo</strong>(<a target="_blank" href="http://php.net/array">array</a> $meta):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$meta</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMetaInfo</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
<pre>public <strong>jsonSerialize</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### TemplateContainerContract<a name="catalog_contracts_templatecontainercontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>register</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/string">string</a> $providerClass = &quot;&quot;):<a href="catalog#catalog_contracts_templatecontract">TemplateContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$providerClass</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getTemplates</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getTemplate</strong>(<a target="_blank" href="http://php.net/string">string</a> $identifier):<a href="catalog#catalog_contracts_templatecontract">TemplateContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$identifier</td>
        <td></td>
    </tr>
</table>



### CatalogExportServiceContract<a name="catalog_contracts_catalogexportservicecontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>setAdditionalFields</strong>(<a target="_blank" href="http://php.net/array">array</a> $additionalFields):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$additionalFields</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $mutator):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSettings</strong>(<a target="_blank" href="http://php.net/array">array</a> $settings):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$settings</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setNumberOfDocumentsPerShard</strong>(<a target="_blank" href="http://php.net/int">int</a> $numberOfDocumentsPerShard):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$numberOfDocumentsPerShard</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setUpdatedSince</strong>(<a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
 $timestamp):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
        <td>$timestamp</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getResult</strong>():<a href="catalog#catalog_models_catalogexportresult">CatalogExportResult</a>
</pre>

    

    

### DataProviderContract<a name="catalog_contracts_dataprovidercontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>getData</strong>(<a target="_blank" href="http://php.net/string">string</a> $query = &quot;&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$query</td>
        <td></td>
    </tr>
</table>



### CatalogContentRepositoryContract<a name="catalog_contracts_catalogcontentrepositorycontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $id):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/string">string</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### CatalogTemplateProviderContract<a name="catalog_contracts_catalogtemplateprovidercontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>getMappings</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPreMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPostMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSkuCallback</strong>():<a target="_blank" href="http://php.net/callable">callable</a></pre>

    

    
<pre>public <strong>getSettings</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getMetaInfo</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### CatalogExportRepositoryContract<a name="catalog_contracts_catalogexportrepositorycontract"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Contracts`





#### Methods

<pre>public <strong>exportById</strong>(<a target="_blank" href="http://php.net/string">string</a> $id):<a href="catalog#catalog_contracts_catalogexportservicecontract">CatalogExportServiceContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


## Models<a name="catalog_catalog_models"></a>
### Catalog<a name="catalog_models_catalog"></a>

The catalog model


#### Namespace

`Plenty\Modules\Catalog\Models`




#### Properties

<table class="table table-bordered table-striped table-condensed table-hover">
    <thead>
    <tr>
        <th>Type</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    </thead>
    <tbody><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>data</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>template</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>id</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CatalogExportResult<a name="catalog_models_catalogexportresult"></a>

To be written


#### Namespace

`Plenty\Modules\Catalog\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Templates<a name="catalog_catalog_templates"></a>
### Template<a name="catalog_templates_template"></a>

foo


#### Namespace

`Plenty\Modules\Catalog\Templates`





#### Methods

<pre>public <strong>getMappings</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMapping</strong>(<a target="_blank" href="http://php.net/array">array</a> $section):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$section</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addPreMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPostMutator</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addFilter</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPreMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPostMutators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setSkuCallback</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSkuCallback</strong>():<a target="_blank" href="http://php.net/callable">callable</a></pre>

    

    
<pre>public <strong>addSetting</strong>(<a target="_blank" href="http://php.net/array">array</a> $setting):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$setting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSettings</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setMetaInfo</strong>(<a target="_blank" href="http://php.net/array">array</a> $meta):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$meta</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMetaInfo</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>jsonSerialize</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getIdentifier</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>boot</strong>(<a href="catalog#catalog_contracts_catalogtemplateprovidercontract">CatalogTemplateProviderContract</a>
 $provider):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="catalog#catalog_contracts_catalogtemplateprovidercontract">CatalogTemplateProviderContract</a>
</td>
        <td>$provider</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isBooted</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
