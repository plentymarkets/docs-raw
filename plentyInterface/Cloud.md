

# ElasticSearch<a name="cloud_elasticsearch"></a>
    
## Contracts<a name="cloud_elasticsearch_contracts"></a>
### ElasticSearchSearchRepositoryContract<a name="cloud_contracts_elasticsearchsearchrepositorycontract"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Contracts`



#### Methods

<pre>public <strong>setIndex</strong>(<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
 $index):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</td>
        <td>$index</td>
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


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $result):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$result</td>
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


<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPostProcessor</strong>(<a href="cloud#cloud_processor_processorinterface">ProcessorInterface</a>
 $processor):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_processor_processorinterface">ProcessorInterface</a>
</td>
        <td>$processor</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
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


<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# Lib<a name="cloud_lib"></a>
    
## Aggregating<a name="cloud_lib_aggregating"></a>
### AggregatingInterface<a name="cloud_aggregating_aggregatinginterface"></a>

foo


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Aggregating`



#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Index<a name="cloud_lib_index"></a>
### IndexInterface<a name="cloud_index_indexinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index`



#### Methods

<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getVersion</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getIdentifier</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
## Output<a name="cloud_lib_output"></a>
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


## Sorting<a name="cloud_lib_sorting"></a>
### SortingInterface<a name="cloud_sorting_sortinginterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Sorting`



#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Source<a name="cloud_lib_source"></a>
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

    

    

### SourceInterface<a name="cloud_source_sourceinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source`



#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# Data<a name="cloud_data"></a>
    
## Document<a name="cloud_data_document"></a>
### DocumentInterface<a name="cloud_document_documentinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Data\Document`



#### Methods

<pre>public <strong>getIndex</strong>():<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
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
    
# Index<a name="cloud_index"></a>
    
## Settings<a name="cloud_index_settings"></a>
### SettingsInterface<a name="cloud_settings_settingsinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Index\Settings`



#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
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
    
# Source<a name="cloud_source"></a>
    
## Mutator<a name="cloud_source_mutator"></a>
### BaseMutator<a name="cloud_mutator_basemutator"></a>

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


<pre>public <strong>setSetLanguageAsIndex</strong>(<a target="_blank" href="http://php.net/boolean">boolean</a> $setLanguageAsIndex):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
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


## Processor<a name="cloud_mutator_processor"></a>
### BaseProcessor<a name="cloud_processor_baseprocessor"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Mutator\Processor`



#### Methods

<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_mutator_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
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



### ProcessorInterface<a name="cloud_processor_processorinterface"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Mutator\Processor`



#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### QueryProcessor<a name="cloud_processor_queryprocessor"></a>

to be written


#### Namespace

`Plenty\Modules\Cloud\ElasticSearch\Lib\Source\Mutator\Processor`



#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_mutator_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


