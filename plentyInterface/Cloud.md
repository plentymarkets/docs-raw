

# Storage<a name="cloud_storage"></a>
    
## Models<a name="cloud_storage_models"></a>
### StorageObject<a name="cloud_models_storageobject"></a>

Represent a storage object


#### Namespace

`Plenty\Modules\Cloud\Storage\Models`




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
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastModified</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>metaData</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>eTag</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>size</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageClass</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>body</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contentType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contentLength</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### StorageObjectList<a name="cloud_models_storageobjectlist"></a>

Represent a list of storage objects


#### Namespace

`Plenty\Modules\Cloud\Storage\Models`




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
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isTruncated</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>nextContinuationToken</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>objects</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>commonPrefixes</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ElasticSearch<a name="cloud_elasticsearch"></a>
    
## Contracts<a name="cloud_elasticsearch_contracts"></a>
### ElasticSearchSearchRepositoryContract<a name="cloud_contracts_elasticsearchsearchrepositorycontract"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Contracts`





#### Methods

<pre>public <strong>setIndex</strong>(<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
 $index):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSearch</strong>($search):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### ElasticSearchMultiSearchRepositoryContract<a name="cloud_contracts_elasticsearchmultisearchrepositorycontract"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Contracts`





#### Methods

<pre>public <strong>setIndex</strong>(<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
 $index):<a href="cloud#cloud_contracts_elasticsearchmultisearchrepositorycontract">ElasticSearchMultiSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSearch</strong>($search):<a href="cloud#cloud_contracts_elasticsearchmultisearchrepositorycontract">ElasticSearchMultiSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
## Lib<a name="cloud_elasticsearch_lib"></a>
### ElasticSearch<a name="cloud_lib_elasticsearch"></a>

elastic search constants


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib`





#### Methods

<pre>public static <strong>getKeyByLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $language):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
</table>


# Lib<a name="cloud_lib"></a>
    
## Processor<a name="cloud_lib_processor"></a>
### BaseProcessor<a name="cloud_processor_baseprocessor"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Processor`





#### Methods

<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### DocumentInnerHitsToRootProcessor<a name="cloud_processor_documentinnerhitstorootprocessor"></a>

DocumentInnerHitsToRootProcessor


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Processor`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### ProcessorInterface<a name="cloud_processor_processorinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Processor`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### SuggestionProcessor<a name="cloud_processor_suggestionprocessor"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Processor`





#### Methods

<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### DocumentProcessor<a name="cloud_processor_documentprocessor"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Processor`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>


## Source<a name="cloud_lib_source"></a>
### ExcludeSource<a name="cloud_source_excludesource"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>activateAll</strong>():<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</pre>

    

    
<pre>public <strong>activate</strong>():<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</pre>

    

    
<pre>public <strong>activateList</strong>(<a target="_blank" href="http://php.net/array">array</a> $fields):<a href="cloud#cloud_lib_source">Source</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fields</td>
        <td></td>
    </tr>
</table>



### IncludeSource<a name="cloud_source_includesource"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>activateAll</strong>():<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</pre>

    

    
<pre>public <strong>activate</strong>():<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</pre>

    

    
<pre>public <strong>activateList</strong>(<a target="_blank" href="http://php.net/array">array</a> $fields):<a href="cloud#cloud_lib_source">Source</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fields</td>
        <td></td>
    </tr>
</table>



### SourceInterface<a name="cloud_source_sourceinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### IndependentSource<a name="cloud_source_independentsource"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>activateAll</strong>():<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</pre>

    

    
<pre>public <strong>activate</strong>():<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</pre>

    

    
<pre>public <strong>activateList</strong>(<a target="_blank" href="http://php.net/array">array</a> $fields):<a href="cloud#cloud_lib_source">Source</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fields</td>
        <td></td>
    </tr>
</table>


## Output<a name="cloud_lib_output"></a>
### OutputInterface<a name="cloud_output_outputinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Output`





#### Methods

<pre>public <strong>write</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>info</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>error</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>



### DevNullOutput<a name="cloud_output_devnulloutput"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Output`





#### Methods

<pre>public <strong>write</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>info</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>error</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>


## Collapse<a name="cloud_lib_collapse"></a>
### BaseCollapse<a name="cloud_collapse_basecollapse"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Collapse`





#### Methods

<pre>public <strong>addInnerHit</strong>(<a href="cloud#cloud_innerhit_innerhitinterface">InnerHitInterface</a>
 $innerHit):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_innerhit_innerhitinterface">InnerHitInterface</a>
</td>
        <td>$innerHit</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### CollapseInterface<a name="cloud_collapse_collapseinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Collapse`





#### Methods

<pre>public <strong>addInnerHit</strong>(<a href="cloud#cloud_innerhit_innerhitinterface">InnerHitInterface</a>
 $innerHit):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_innerhit_innerhitinterface">InnerHitInterface</a>
</td>
        <td>$innerHit</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Search<a name="cloud_lib_search"></a>
### SearchGroup<a name="cloud_search_searchgroup"></a>

To be written...


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search`





#### Methods

<pre>public <strong>addSearch</strong>(<a href="cloud#cloud_search_searchinterface">SearchInterface</a>
 $search):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_search_searchinterface">SearchInterface</a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $query):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>



### BaseSearch<a name="cloud_search_basesearch"></a>

Base class for different Search classes


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search`





#### Methods

<pre>public <strong>setIsSourceDisabled</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $isSourceDisabled):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isSourceDisabled</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPostFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $query):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSuggestion</strong>(<a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
 $suggestion):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
</td>
        <td>$suggestion</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setCollapse</strong>(<a href="cloud#cloud_collapse_collapseinterface">CollapseInterface</a>
 $collapse):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_collapse_collapseinterface">CollapseInterface</a>
</td>
        <td>$collapse</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setScoreModifier</strong>(<a href="cloud#cloud_scoremodifier_scoremodifierinterface">ScoreModifierInterface</a>
 $scoreModifier):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_scoremodifier_scoremodifierinterface">ScoreModifierInterface</a>
</td>
        <td>$scoreModifier</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setMaxResultWindow</strong>(<a target="_blank" href="http://php.net/int">int</a> $maxResults = 10000):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$maxResults</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    

### SearchInterface<a name="cloud_search_searchinterface"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search`





#### Methods

<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $query):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSuggestion</strong>(<a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
 $suggestion):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
</td>
        <td>$suggestion</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setMaxResultWindow</strong>(<a target="_blank" href="http://php.net/int">int</a> $maxResults = 10000):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$maxResults</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Sorting<a name="cloud_lib_sorting"></a>
### SingleSorting<a name="cloud_sorting_singlesorting"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Sorting`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### MultipleSorting<a name="cloud_sorting_multiplesorting"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Sorting`





#### Methods

<pre>public <strong>addSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/string">string</a> $path, <a target="_blank" href="http://php.net/string">string</a> $order = \Plenty\Modules\Cloud\ElasticSearch\Lib\ElasticSearch::SORTING_ORDER_ASC):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### SortingInterface<a name="cloud_sorting_sortinginterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Sorting`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    

### SingleNestedSorting<a name="cloud_sorting_singlenestedsorting"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Sorting`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
## Index<a name="cloud_lib_index"></a>
### ReindexIndex<a name="cloud_index_reindexindex"></a>

to bew written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index`





#### Methods

<pre>public <strong>getType</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getVersion</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getDomain</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getMeta</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSettingsClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getMappingClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getDynamicTemplateClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getNext</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getScrollRepositoryClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasUpdatedAt</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isReady</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>maySynchronize</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Vorrübergehender Cheat - alles was noch keine Version hat,
darf nicht über die &quot;neuen&quot; Prozesse befüllt werden!
    
<pre>public <strong>getPlentyId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getIdentifier</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether ElasticSearch is generally available,
and whether the index has already been created.
    
<pre>public <strong>setRefreshInterval</strong>($value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>resetAvailibilityStatus</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getInfo</strong>():<a href="cloud#cloud_info_baseinfo">BaseInfo</a>
</pre>

    

    
<pre>public <strong>mayBeQueuedForCreation</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>hasAllField</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>refresh</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### IndexInterface<a name="cloud_index_indexinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index`





#### Methods

<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getVersion</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getDomain</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getIdentifier</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isReady</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getSettingsClassName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getMappingClassName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDynamicTemplateClassName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getMeta</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getInfo</strong>():<a href="cloud#cloud_info_infointerface">InfoInterface</a>
</pre>

    

    
<pre>public <strong>resetAvailibilityStatus</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasUpdatedAt</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>hasAllField</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getNext</strong>():<a href="cloud#cloud_index_nextindex">NextIndex</a>
</pre>

    

    
<pre>public <strong>getScrollRepositoryClassName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>refresh</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### NextIndex<a name="cloud_index_nextindex"></a>

to bew written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index`





#### Methods

<pre>public <strong>getType</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getVersion</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getDomain</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getSettingsClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getMappingClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getDynamicTemplateClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getNext</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getScrollRepositoryClassName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasUpdatedAt</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isReady</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>maySynchronize</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Vorrübergehender Cheat - alles was noch keine Version hat,
darf nicht über die &quot;neuen&quot; Prozesse befüllt werden!
    
<pre>public <strong>getPlentyId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getIdentifier</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether ElasticSearch is generally available,
and whether the index has already been created.
    
<pre>public <strong>setRefreshInterval</strong>($value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>resetAvailibilityStatus</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getMeta</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getInfo</strong>():<a href="cloud#cloud_info_baseinfo">BaseInfo</a>
</pre>

    

    
<pre>public <strong>mayBeQueuedForCreation</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>hasAllField</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>refresh</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
# Source<a name="cloud_source"></a>
    
## Condition<a name="cloud_source_condition"></a>
### ConditionInterface<a name="cloud_condition_conditioninterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Condition`





#### Methods

<pre>public <strong>isValid</strong>(<a target="_blank" href="http://php.net/array">array</a> $document):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$document</td>
        <td></td>
    </tr>
</table>


## Mutator<a name="cloud_source_mutator"></a>
### BaseMutator<a name="cloud_mutator_basemutator"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Mutator`





#### Methods

<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### MutatorInterface<a name="cloud_mutator_mutatorinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Mutator`





#### Methods

<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# Mutator<a name="cloud_mutator"></a>
    
## BuiltIn<a name="cloud_mutator_builtin"></a>
### LanguageMutator<a name="cloud_builtin_languagemutator"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Mutator\BuiltIn`





#### Methods

<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $language):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setLanguages</strong>(<a target="_blank" href="http://php.net/array">array</a> $languages):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$languages</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSetLanguageAsIndex</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $setLanguageAsIndex):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$setLanguageAsIndex</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>isSeqArray</strong>($array):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$array</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# Collapse<a name="cloud_collapse"></a>
    
## InnerHit<a name="cloud_collapse_innerhit"></a>
### BaseInnerHit<a name="cloud_innerhit_baseinnerhit"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Collapse\InnerHit`





#### Methods

<pre>public <strong>setSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### InnerHitInterface<a name="cloud_innerhit_innerhitinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Collapse\InnerHit`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
# Search<a name="cloud_search"></a>
    
## Aggregation<a name="cloud_search_aggregation"></a>
### AggregationInterface<a name="cloud_aggregation_aggregationinterface"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search\Aggregation`





#### Methods

<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Suggestion<a name="cloud_search_suggestion"></a>
### SuggestionInterface<a name="cloud_suggestion_suggestioninterface"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search\Suggestion`





#### Methods

<pre>public <strong>setText</strong>(<a target="_blank" href="http://php.net/string">string</a> $text):<a href="cloud#cloud_search_suggestion">Suggestion</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$text</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    

### TermSuggestion<a name="cloud_suggestion_termsuggestion"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search\Suggestion`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setText</strong>(<a target="_blank" href="http://php.net/string">string</a> $text):<a href="cloud#cloud_search_suggestion">Suggestion</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$text</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
## Document<a name="cloud_search_document"></a>
### DocumentSearch<a name="cloud_document_documentsearch"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Search\Document`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPostFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getQuery</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getAggregations</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSuggestions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setName</strong>($name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$name</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setIsSourceDisabled</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $isSourceDisabled):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isSourceDisabled</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPostFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $query):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSuggestion</strong>(<a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
 $suggestion):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
</td>
        <td>$suggestion</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setCollapse</strong>(<a href="cloud#cloud_collapse_collapseinterface">CollapseInterface</a>
 $collapse):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_collapse_collapseinterface">CollapseInterface</a>
</td>
        <td>$collapse</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setScoreModifier</strong>(<a href="cloud#cloud_scoremodifier_scoremodifierinterface">ScoreModifierInterface</a>
 $scoreModifier):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_scoremodifier_scoremodifierinterface">ScoreModifierInterface</a>
</td>
        <td>$scoreModifier</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setMaxResultWindow</strong>(<a target="_blank" href="http://php.net/int">int</a> $maxResults = 10000):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$maxResults</td>
        <td></td>
    </tr>
</table>


# Mapping<a name="cloud_mapping"></a>
    
## Property<a name="cloud_mapping_property"></a>
### PropertyInterface<a name="cloud_property_propertyinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index\Mapping\Property`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
# Type<a name="cloud_type"></a>
    
## Complex<a name="cloud_type_complex"></a>
### ComplexPropertyInterface<a name="cloud_complex_complexpropertyinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index\Mapping\Property\Type\Complex`





#### Methods

<pre>public <strong>getProperties</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addProperty</strong>(<a href="cloud#cloud_property_propertyinterface">PropertyInterface</a>
 $property):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_property_propertyinterface">PropertyInterface</a>
</td>
        <td>$property</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## ScoreModifier<a name="cloud_type_scoremodifier"></a>
### ScoreModifierInterface<a name="cloud_scoremodifier_scoremodifierinterface"></a>

To be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Query\Type\ScoreModifier`





#### Methods

<pre>public <strong>setQuery</strong>($query):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    

### RandomScore<a name="cloud_scoremodifier_randomscore"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Query\Type\ScoreModifier`





#### Methods

<pre>public <strong>getFunction</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getBoostMode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getSeed</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setSeed</strong>(<a target="_blank" href="http://php.net/string">string</a> $seed):<a href="cloud#cloud_scoremodifier_randomscore">RandomScore</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$seed</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setQuery</strong>($query):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Query<a name="cloud_type_query"></a>
### MultiMatchQuery<a name="cloud_query_multimatchquery"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Query\Type\Query`





#### Methods

<pre>public <strong>addField</strong>(<a target="_blank" href="http://php.net/string">string</a> $field, <a target="_blank" href="http://php.net/int">int</a> $boost):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$boost</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setOperator</strong>(<a target="_blank" href="http://php.net/string">string</a> $operator):<a href="cloud#cloud_query_multimatchquery">MultiMatchQuery</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setFuzzy</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $fuzzy):<a href="cloud#cloud_query_multimatchquery">MultiMatchQuery</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$fuzzy</td>
        <td></td>
    </tr>
</table>


# Index<a name="cloud_index"></a>
    
## Settings<a name="cloud_index_settings"></a>
### SettingsInterface<a name="cloud_settings_settingsinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index\Settings`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Info<a name="cloud_index_info"></a>
### InfoInterface<a name="cloud_info_infointerface"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index\Info`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>set</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>remove</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>



### BaseInfo<a name="cloud_info_baseinfo"></a>

to bew written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index\Info`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>set</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>remove</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


# Query<a name="cloud_query"></a>
    
## Statement<a name="cloud_query_statement"></a>
### StatementInterface<a name="cloud_statement_statementinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Query\Statement`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Type<a name="cloud_query_type"></a>
### TypeInterface<a name="cloud_type_typeinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Query\Type`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
# Data<a name="cloud_data"></a>
    
## Document<a name="cloud_data_document"></a>
### DocumentInterface<a name="cloud_document_documentinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Data\Document`





#### Methods

<pre>public <strong>getIndex</strong>():<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</pre>

    

    
<pre>public <strong>getSize</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
