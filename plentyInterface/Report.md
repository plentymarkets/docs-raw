

# Report<a name="report_report"></a>
    
## Contracts<a name="report_report_contracts"></a>
### RawDataRepositoryContract<a name="report_contracts_rawdatarepositorycontract"></a>

This interface allows you to get a list of generated raw data files


#### Namespace

`Plenty\Modules\Report\Contracts`





#### Methods

<pre>public <strong>searchRawData</strong>(<a target="_blank" href="http://php.net/string">string</a> $dataName, <a target="_blank" href="http://php.net/int">int</a> $createdAtTimestamp, <a target="_blank" href="http://php.net/string">string</a> $processStatus, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 20, <a target="_blank" href="http://php.net/string">string</a> $sortOrder = &quot;asc&quot;, <a target="_blank" href="http://php.net/string">string</a> $after = &quot;&quot;):<a href="report#report_models_rawdatasearchresult">RawDataSearchResult</a>
</pre>

    
Get list of raw data. Valid filter combinations: (dataName), (dataName &amp; processStatus), (createdAtTimestamp)
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$dataName</td>
        <td>Filter that restricts the search result to raw data files.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$createdAtTimestamp</td>
        <td>Timestamp from when daily generated raw data are to be filtered. The maximum distance may not exceed one year.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$processStatus</td>
        <td>Process status after which filtering is to take place</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of raw data files to be returned. The default number of files is 20 and the maximum is 100.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sortOrder</td>
        <td>Defines the sort order, possible values are: asc, desc. With simultaneous filtering to dataName, only the current result is sorted.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$after</td>
        <td>The last evaluated key as base64, provide that as the starting point for the next query (pagination).</td>
    </tr>
</table>


<pre>public <strong>getRawDataFile</strong>(<a target="_blank" href="http://php.net/string">string</a> $path):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a raw data file from the storage, the storage path of the file must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td>The raw data file path</td>
    </tr>
</table>


<pre>public <strong>getRawDataCreatorModels</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get list of all raw data creators
    
<pre>public <strong>getRawDataConfigs</strong>():<a href="report#report_models_rawdataconfigs">RawDataConfigs</a>
</pre>

    
Returns list of all saved configurations
    
<pre>public <strong>updateRawDataConfigs</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="report#report_models_rawdataconfigs">RawDataConfigs</a>
</pre>

    
Resets all saved raw data configurations with given data
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The configs data</td>
    </tr>
</table>


## Models<a name="report_report_models"></a>
### RawDataConfig<a name="report_models_rawdataconfig"></a>

The report raw data config model


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>dataName</td>
            <td>The raw data name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>active</td>
            <td>If active, raw data is generated daily</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deleteRawDataAfterDays</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RawData<a name="report_models_rawdata"></a>

The report raw model


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>id</td>
            <td>The raw data id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>createdAtTimestamp</td>
            <td>Unix timestamp of creation of this raw data file</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td>The plentymarkets system id hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>dataName</td>
            <td>The raw data name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>dataNameProcessStatus</td>
            <td>Composite index of dataName#processStatus#</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>processStatusPlentyIdHash</td>
            <td>Composite index of processStatus#plentyIdHash#</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td>Storage path to raw data file</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### KeyFigureFilter<a name="report_models_keyfigurefilter"></a>

The key figure filter model is the base class of all key figure filter classes. Each KeyFigure class needs a filter class, which defines the allowed fields to be filtered.


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>filters</td>
            <td>List of allowed filter names</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RawDataCreator<a name="report_models_rawdatacreator"></a>

The report raw data creator model


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>dataName</td>
            <td>Exclusive identifier for this raw data.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileFormat</td>
            <td>File format</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>limitPage</td>
            <td>Number of data rows to be queried maximum per request.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>limitDay</td>
            <td>Number of data rows to be queried maximum per day.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>earliestPossibleDataDate</td>
            <td>Earliest possible date from which data should be requested.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deleteRawDataAfterDaysMinimum</td>
            <td>Minimum number of days after the generated raw data is deleted</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deleteRawDataAfterDaysMaximum</td>
            <td>Maximum number of days after the generated raw data is deleted</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>filterType</td>
            <td>Defines how this raw data is filtered.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>dataUpdatedAtColumnName</td>
            <td>Name of the column that contains the date of the last change to a data row.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>defaultActive</td>
            <td>If true, then these raw data are collected independently of the user configuration.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>interval</td>
            <td>Interval in which this creator runs through</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>shouldProcessed</td>
            <td>Internal param</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RawDataSearchResult<a name="report_models_rawdatasearchresult"></a>

The report raw data search result model


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>after</td>
            <td>The last evaluated key as base64, provide that as the starting point for the next query (pagination).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>searchResult</td>
            <td>The raw data search result</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### KeyFigureResult<a name="report_models_keyfigureresult"></a>

Represents a key figure result


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>keyFigureConfigId</td>
            <td>Id of key figure config</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>scaleBasisTime</td>
            <td>Scale basis time</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keyFigure</td>
            <td>Key figure name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td>System id hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>resultData</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### KeyFigureConfig<a name="report_models_keyfigureconfig"></a>

The key figure config model represents the configuration of a key figure.


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>id</td>
            <td>Id of this configuration</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td>The plentymarkets system id hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keyFigure</td>
            <td>Key figure name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keyFigureName</td>
            <td>User defined name</td>
        </tr><tr>
            <td><a href="report#report_models_keyfigurefilter">KeyFigureFilter</a>
</td>
            <td>filter</td>
            <td>Filter for calculating key this key figure</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>calculateAt</td>
            <td>Time of last calculation (Unixtime)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>Time of last change</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>Time of creation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RawDataConfigs<a name="report_models_rawdataconfigs"></a>

List of all saved raw data configurations


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>plentyIdHash</td>
            <td>The plentymarkets system id hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>configs</td>
            <td>List of all saved configurations</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Report<a name="report_models_report"></a>

Represents the configuration of a report and its key figures.


#### Namespace

`Plenty\Modules\Report\Models`




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
            <td>id</td>
            <td>Id of this report</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td>The plentymarkets system id hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>reportName</td>
            <td>Name of this report</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>Time of last change</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>Time of creation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
