

# Contracts<a name="elasticsync_contracts"></a>
    
## Core<a name="elasticsync_contracts_core"></a>
### ElasticSyncMappingRepositoryContract<a name="elasticsync_core_elasticsyncmappingrepositorycontract"></a>

This interface allows you to get, list, create, update and delete elastic sync mappings.


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Core`





#### Methods

<pre>public <strong>createSyncMapping</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a sync mapping.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>getSyncMapping</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a sync mapping.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listSyncMappings</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $paginate = 1, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List sync mappings.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSyncMapping</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a sync mapping.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncMapping</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a sync mapping.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncMappings</strong>(<a target="_blank" href="http://php.net/array">array</a> $mappingIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete one or more mappings.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$mappingIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>copySyncMapping</strong>(<a target="_blank" href="http://php.net/array">array</a> $mappingIds):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Copy sync mapping.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$mappingIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>mappingValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $sync_type):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the mapping values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sync_type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>fieldValuesMap</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated!             </h3>
        </div>
        <div class="panel-body">
            This method will not be supported in the future. Please refrain from using it as soon as possible.
        </div>
    </div>
    
Get the field value map for all sync types.
    
<pre>public <strong>listVariationMatched</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a list with variation matches.
    
<pre>public <strong>modelKeyToFieldValueKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $syncType):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the model key to field value key.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$syncType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>filterLabelList</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the label list for mapping filtration.
    
<pre>public <strong>mappingValuesTree</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the mapping values tree.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>csvColumns</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the csv columns of a sync.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>rowCsv</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the csv rows.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPlentyFieldsValueMap</strong>(<a target="_blank" href="http://php.net/string">string</a> $syncDataType):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the plenty fields value map for a particular sync type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$syncDataType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
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
    

### ElasticSyncMatchingRepositoryContract<a name="elasticsync_core_elasticsyncmatchingrepositorycontract"></a>

This interface allows you to get, list, create, update and delete elastic sync matches.


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Core`





#### Methods

<pre>public <strong>createSyncMatching</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a sync matching.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td>The id of the sync</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>getSyncMatching</strong>(<a target="_blank" href="http://php.net/int">int</a> $matchingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a sync matching.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$matchingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listSyncMatches</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List sync matches.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSyncMatching</strong>(<a target="_blank" href="http://php.net/int">int</a> $matchingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a sync matching.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$matchingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncMatching</strong>(<a target="_blank" href="http://php.net/int">int</a> $matchingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a sync matching.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$matchingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getEntity</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get an entity.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>matchingFields</strong>(<a target="_blank" href="http://php.net/string">string</a> $syncType):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a list of all mappings for a particular sync type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$syncType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createSyncMatches</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create sync matches.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td>The id of the sync</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateSyncMatches</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update sync matches.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listDecimals</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get list of decimals.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
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
    

### ElasticSyncMappingFilterRepositoryContract<a name="elasticsync_core_elasticsyncmappingfilterrepositorycontract"></a>

This interface allows you to get, list, create, update and delete elastic sync mapping filters.


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Core`





#### Methods

<pre>public <strong>createSyncMappingFilter</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a sync mapping filter.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td>The id of the mapping</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>getSyncMappingFilter</strong>(<a target="_blank" href="http://php.net/int">int</a> $filterId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a sync mapping filter.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$filterId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listSyncMappingFilters</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List sync mapping filters.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSyncMappingFilter</strong>(<a target="_blank" href="http://php.net/int">int</a> $filterId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a sync mapping filter.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$filterId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncMappingFilter</strong>(<a target="_blank" href="http://php.net/int">int</a> $filterId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a sync mapping filter.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$filterId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createSyncMappingFilters</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create sync mapping filters.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td>The id of the mapping</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateSyncMappingFilters</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update sync mapping filters.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
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
    

### ElasticSyncOptionRepositoryContract<a name="elasticsync_core_elasticsyncoptionrepositorycontract"></a>

This interface allows you to get, list, create, update and delete elastic sync options.


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Core`





#### Methods

<pre>public <strong>createSyncOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a sync option.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td>The sync id</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>getSyncOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a sync option.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listSyncOptions</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List sync options.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td>The sync id</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSyncOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a sync option.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a sync option.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createSyncOptions</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create sync options.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td>The sync id</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateSyncOptions</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update sync options.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
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
    

### ElasticSyncSyncRepositoryContract<a name="elasticsync_core_elasticsyncsyncrepositorycontract"></a>

This interface allows you to get, list, create, update and delete elastic sync syncs.


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Core`





#### Methods

<pre>public <strong>createSync</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a sync.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>getSync</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a sync.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listSyncs</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $paginate = 1, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Get all syncs
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSync</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a sync.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSync</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a sync.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncs</strong>(<a target="_blank" href="http://php.net/array">array</a> $syncIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete syncs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$syncIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getListTypes</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get list of sync types.
    
<pre>public <strong>getListIntervals</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get list of sync intervals.
    
<pre>public <strong>getListDecimals</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get list of sync decimals.
    
<pre>public <strong>export</strong>(<a target="_blank" href="http://php.net/array">array</a> $syncIds):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Export the syncs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$syncIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>copy</strong>(<a target="_blank" href="http://php.net/array">array</a> $syncIds):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Copy the syncs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$syncIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>resetCache</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Reset the cache.
    
<pre>public <strong>sourcePreview</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Preview the syncs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>scheduleTimes</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get schedule times.
    
<pre>public <strong>getReportLogs</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $paginate = 1, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Check Report Log.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>saveCsvToS3</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Save the CSV on S3.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>importSyncDifferent</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Import the sync with different plentyId.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPreviewValues</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get preview of csv values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>run</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Execute the run procedure.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>report</strong>($id):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get Log ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>reportAvailable</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $paginate = 1, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Check Report Log.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>exportSync</strong>(<a target="_blank" href="http://php.net/int">int</a> $syncId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Export the sync.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$syncId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
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
    

### ElasticSyncMappingRowRepositoryContract<a name="elasticsync_core_elasticsyncmappingrowrepositorycontract"></a>

This interface allows you to get, list, create, update and delete elastic sync mapping rows.


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Core`





#### Methods

<pre>public <strong>createSyncMappingRow</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a sync mapping row.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td>The id of the mapping</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>getSyncMappingRow</strong>(<a target="_blank" href="http://php.net/int">int</a> $rowId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a sync mapping row.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listSyncMappingRows</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List sync mapping rows.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSyncMappingRow</strong>(<a target="_blank" href="http://php.net/int">int</a> $rowId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a sync mapping row.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteSyncMappingRow</strong>(<a target="_blank" href="http://php.net/int">int</a> $rowId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a sync mapping row.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSyncMappingRows</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update sync mapping rows.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createSyncMappingRows</strong>(<a target="_blank" href="http://php.net/int">int</a> $mappingId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create sync mapping rows.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mappingId</td>
        <td>The id of the mapping</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
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
    
## Mapper<a name="elasticsync_contracts_mapper"></a>
### PropertyDescriptor<a name="elasticsync_mapper_propertydescriptor"></a>

describes properties of a Model


#### Namespace

`Plenty\Modules\ElasticSync\Contracts\Mapper`





#### Methods

<pre>public <strong>getPropertyInformation</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
        <td></td>
    </tr>
</table>


# Models<a name="elasticsync_models"></a>
    
## Core<a name="elasticsync_models_core"></a>
### ElasticSyncMappingRow<a name="elasticsync_core_elasticsyncmappingrow"></a>

The elastic sync mapping row model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Core`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the elastic sync mapping row</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mappingId</td>
            <td>The ID of the elastic sync mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>targetModel</td>
            <td>The target model of the elastic sync mapping row</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>targetAttribute</td>
            <td>The target attribute of the elastic sync mapping row</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>active</td>
            <td>The state of the elastic sync mapping row</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>entityType</td>
            <td>The entity type of the elastic sync mapping row (array values: 'ownValue', 'ownAssignment', 'regularExpression', 'csvColumn')</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the elastic sync mapping row</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>settings</td>
            <td>The settings of the elastic sync mapping row</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>identifiers</td>
            <td>The identifiers of the elastic sync mapping row</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ElasticSyncMapping<a name="elasticsync_core_elasticsyncmapping"></a>

The elastic sync mapping model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Core`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the elastic sync mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>syncId</td>
            <td>The ID of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the elastic sync mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the elastic sync mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>active</td>
            <td>The state of the elastic sync mapping</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ElasticSyncSync<a name="elasticsync_core_elasticsyncsync"></a>

The elastic sync sync model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Core`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>syncType</td>
            <td>The type of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sourceType</td>
            <td>The source type of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sourceDataType</td>
            <td>The source data type of the elastic sync sync</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastRun</td>
            <td>The date when elastic sync sync was last run</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the elastic sync sync was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the elastic sync sync was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ElasticSyncOption<a name="elasticsync_core_elasticsyncoption"></a>

The elastic sync option model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Core`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the elastic sync option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>syncId</td>
            <td>The ID of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>optionIdentifier</td>
            <td>The option identifier of the elastic sync option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>The key of the elastic sync option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the elastic sync option</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the elastic sync option was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the elastic sync option was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ElasticSyncMappingFilter<a name="elasticsync_core_elasticsyncmappingfilter"></a>

The elastic sync mapping filter model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Core`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the elastic sync mapping filter</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mappingId</td>
            <td>The ID of the elastic sync mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the elastic sync mapping filter</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>operator</td>
            <td>The operator of the elastic sync mapping filter</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>source</td>
            <td>The source of the elastic sync mapping filter</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the elastic sync mapping filter</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ElasticSyncMatching<a name="elasticsync_core_elasticsyncmatching"></a>

The elastic sync matching model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Core`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the elastic sync matching</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>syncId</td>
            <td>The ID of the elastic sync sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>target</td>
            <td>The target of the elastic sync matching</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>source</td>
            <td>The source of the elastic sync matching</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>additionalValue</td>
            <td>The additional value of the elastic sync matching</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## DataProvider<a name="elasticsync_models_dataprovider"></a>
### PropertyInformation<a name="elasticsync_dataprovider_propertyinformation"></a>

property information


#### Namespace

`Plenty\Modules\ElasticSync\Models\DataProvider`





#### Methods

<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDescription</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
## Sync<a name="elasticsync_models_sync"></a>
### SyncLog<a name="elasticsync_sync_synclog"></a>

The synclog model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Sync`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>syncId</td>
            <td>The syncId of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>syncHash</td>
            <td>The syncHash of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>jobHash</td>
            <td>The jobHash of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>hashDate</td>
            <td>The hashDate of the synclog</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the synclog was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the synclog was last updated</td>
        </tr><tr>
            <td><a href="elasticsync#elasticsync_sync_synclog">SyncLog</a>
</td>
            <td>syncLog</td>
            <td>The sync log from ElasticSync.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Mapping<a name="elasticsync_sync_mapping"></a>

The mapping model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Sync`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>data</td>
            <td>The data of the mapping</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the mapping was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the mapping was last updated</td>
        </tr><tr>
            <td><a href="elasticsync#elasticsync_sync_mapping">Mapping</a>
</td>
            <td>mapping</td>
            <td>The mapping from ElasticSync.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Sync<a name="elasticsync_sync_sync"></a>

The sync model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Sync`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>data</td>
            <td>The data of the sync</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the sync was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the sync was last updated</td>
        </tr><tr>
            <td><a href="elasticsync#elasticsync_sync_sync">Sync</a>
</td>
            <td>sync</td>
            <td>The sync from ElasticSync.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
