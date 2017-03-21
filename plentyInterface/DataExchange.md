

# DataExchange<a name="dataexchange_dataexchange"></a>
    
## Contracts<a name="dataexchange_dataexchange_contracts"></a>
### CSVGenerator<a name="dataexchange_contracts_csvgenerator"></a>

generator for csv content


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>setDelimiter</strong>(<a target="_blank" href="http://php.net/string">string</a> $delimiter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setEnclosure</strong>(<a target="_blank" href="http://php.net/string">string</a> $enclosure):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$enclosure</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCSVContent</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addContent</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateContent</strong>($resultData, <a target="_blank" href="http://php.net/array">array</a> $formatSettings = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resultData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
</table>



### CSVPluginGenerator<a name="dataexchange_contracts_csvplugingenerator"></a>

generator for csv content


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>setDelimiter</strong>(<a target="_blank" href="http://php.net/string">string</a> $delimiter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setEnclosure</strong>(<a target="_blank" href="http://php.net/string">string</a> $enclosure):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$enclosure</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCSVContent</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addContent</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generatePluginContent</strong>($resultData, <a target="_blank" href="http://php.net/array">array</a> $formatSettings = [], <a target="_blank" href="http://php.net/array">array</a> $filter = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resultData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>



### Filters<a name="dataexchange_contracts_filters"></a>

Filters


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>generateFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $formatSettings = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
</table>



### Generator<a name="dataexchange_contracts_generator"></a>

Generator


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>addContent</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateContent</strong>($resultData, <a target="_blank" href="http://php.net/array">array</a> $formatSettings = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resultData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
</table>



### Output<a name="dataexchange_contracts_output"></a>

Output


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>out</strong>(<a target="_blank" href="http://php.net/string">string</a> $ressource, <a target="_blank" href="http://php.net/array">array</a> $outputParams = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
process export output
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$ressource</td>
        <td>filename to ressource</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$outputParams</td>
        <td></td>
    </tr>
</table>



### PluginGenerator<a name="dataexchange_contracts_plugingenerator"></a>

PluginGenerator


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>addContent</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generatePluginContent</strong>($resultData, <a target="_blank" href="http://php.net/array">array</a> $formatSettings = [], <a target="_blank" href="http://php.net/array">array</a> $filter = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resultData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>



### ResultFields<a name="dataexchange_contracts_resultfields"></a>

ResultFields


#### Namespace

`Plenty\Modules\DataExchange\Contracts`



#### Methods

<pre>public <strong>generateResultFields</strong>(<a target="_blank" href="http://php.net/array">array</a> $formatSettings = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setGroupByList</strong>(<a target="_blank" href="http://php.net/array">array</a> $groupByList):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$groupByList</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setOrderByList</strong>(<a target="_blank" href="http://php.net/array">array</a> $orderByList):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$orderByList</td>
        <td></td>
    </tr>
</table>



### XMLGenerator<a name="dataexchange_contracts_xmlgenerator"></a>

generator for xml content


#### Namespace

`Plenty\Modules\DataExchange\Contracts`


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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>version</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>encoding</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>formatOutput</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>preserveWhiteSpace</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>init</strong>(<a target="_blank" href="http://php.net/string">string</a> $rootName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initializes the xml document and the root element.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$rootName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>root</strong>():<a href="miscellaneous#miscellaneous__domelement">DOMElement</a>
</pre>

    

    
<pre>public <strong>build</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Build the XML.
    
<pre>public <strong>createElement</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value = null):<a href="miscellaneous#miscellaneous__domelement">DOMElement</a>
</pre>

    
Create an XML element.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createCDATASection</strong>(<a target="_blank" href="http://php.net/string">string</a> $data):<a href="miscellaneous#miscellaneous__domcdatasection">DOMCdataSection</a>
</pre>

    
Create a CDATA section.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createAttribute</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value = null):<a href="miscellaneous#miscellaneous__domattr">DOMAttr</a>
</pre>

    
Create an XML attribute.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createTextNode</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__domtext">DOMText</a>
</pre>

    
Create new text node.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addContent</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateContent</strong>($resultData, <a target="_blank" href="http://php.net/array">array</a> $formatSettings = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resultData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
</table>



### XMLPluginGenerator<a name="dataexchange_contracts_xmlplugingenerator"></a>

generator for xml content


#### Namespace

`Plenty\Modules\DataExchange\Contracts`


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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>version</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>encoding</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>formatOutput</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>preserveWhiteSpace</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>init</strong>(<a target="_blank" href="http://php.net/string">string</a> $rootName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initializes the xml document and the root element.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$rootName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>root</strong>():<a href="miscellaneous#miscellaneous__domelement">DOMElement</a>
</pre>

    

    
<pre>public <strong>build</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Build the XML.
    
<pre>public <strong>createElement</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value = null):<a href="miscellaneous#miscellaneous__domelement">DOMElement</a>
</pre>

    
Create an XML element.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createCDATASection</strong>(<a target="_blank" href="http://php.net/string">string</a> $data):<a href="miscellaneous#miscellaneous__domcdatasection">DOMCdataSection</a>
</pre>

    
Create a CDATA section.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createAttribute</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value = null):<a href="miscellaneous#miscellaneous__domattr">DOMAttr</a>
</pre>

    
Create an XML attribute.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createTextNode</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__domtext">DOMText</a>
</pre>

    
Create new text node.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addContent</strong>(<a target="_blank" href="http://php.net/string">string</a> $content):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generatePluginContent</strong>($resultData, <a target="_blank" href="http://php.net/array">array</a> $formatSettings = [], <a target="_blank" href="http://php.net/array">array</a> $filter = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resultData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$formatSettings</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


## Models<a name="dataexchange_dataexchange_models"></a>
### Export<a name="dataexchange_models_export"></a>

Export model


#### Namespace

`Plenty\Modules\DataExchange\Models`


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
            <td>export id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>export name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>export type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>limit</td>
            <td>maximum number of entries</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>formatKey</td>
            <td>the format key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>outputType</td>
            <td>the output type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>filters</td>
            <td>list of filters defined by backend users</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>outputParams</td>
            <td>list of output params</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>formatSettings</td>
            <td>list of format settings</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Filter<a name="dataexchange_models_filter"></a>

export filter


#### Namespace

`Plenty\Modules\DataExchange\Models`


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
            <td>filter id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>exportId</td>
            <td>depending export id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>filter key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>filter value</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FormatSetting<a name="dataexchange_models_formatsetting"></a>

format setting


#### Namespace

`Plenty\Modules\DataExchange\Models`


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
            <td>format setting id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>exportId</td>
            <td>depending export id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>format setting key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>format setting value</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OutputParam<a name="dataexchange_models_outputparam"></a>

output params


#### Namespace

`Plenty\Modules\DataExchange\Models`


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
            <td>output param id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>exportId</td>
            <td>depending export id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>output param key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>output param value</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="dataexchange_dataexchange_services"></a>
### ExportPresetContainer<a name="dataexchange_services_exportpresetcontainer"></a>

Register export presets


#### Namespace

`Plenty\Modules\DataExchange\Services`



#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/string">string</a> $exportKey, <a target="_blank" href="http://php.net/string">string</a> $resultFieldsClass, <a target="_blank" href="http://php.net/string">string</a> $generatorClass, <a target="_blank" href="http://php.net/string">string</a> $filterClass = &quot;&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $isPlugin = false):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$exportKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$resultFieldsClass</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$generatorClass</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filterClass</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isPlugin</td>
        <td></td>
    </tr>
</table>


# Resource<a name="dataexchange_resource"></a>
    
## Contracts<a name="dataexchange_resource_contracts"></a>
### ResourceLoaderContract<a name="dataexchange_contracts_resourceloadercontract"></a>

Repository Contract for ResourceLoader


#### Namespace

`Plenty\Modules\DataExchange\Resource\Contracts`



#### Methods

<pre>public <strong>getResource</strong>(<a target="_blank" href="http://php.net/array">array</a> $sourceOptions):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$sourceOptions</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>validateSourceOptions</strong>(<a target="_blank" href="http://php.net/array">array</a> $sourceOptions):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$sourceOptions</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getLoaderType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### ResourceParserContract<a name="dataexchange_contracts_resourceparsercontract"></a>

Repository Contract for ResourceParser


#### Namespace

`Plenty\Modules\DataExchange\Resource\Contracts`



#### Methods

<pre>public <strong>next</strong>($resource, <a target="_blank" href="http://php.net/array">array</a> $parseOptions):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$resource</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parseOptions</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getParserType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
## Factories<a name="dataexchange_resource_factories"></a>
### ResourceLoaderFactory<a name="dataexchange_factories_resourceloaderfactory"></a>




#### Namespace

`Plenty\Modules\DataExchange\Resource\Factories`



#### Methods

<pre>public <strong>getResourceLoaderByType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="dataexchange#dataexchange_contracts_resourceloadercontract">ResourceLoaderContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addLoader</strong>(<a href="dataexchange#dataexchange_contracts_resourceloadercontract">ResourceLoaderContract</a>
 $loader):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="dataexchange#dataexchange_contracts_resourceloadercontract">ResourceLoaderContract</a>
</td>
        <td>$loader</td>
        <td></td>
    </tr>
</table>



### ResourceParserFactory<a name="dataexchange_factories_resourceparserfactory"></a>




#### Namespace

`Plenty\Modules\DataExchange\Resource\Factories`



#### Methods

<pre>public <strong>getResourceParserByType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="dataexchange#dataexchange_contracts_resourceparsercontract">ResourceParserContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addParser</strong>(<a href="dataexchange#dataexchange_contracts_resourceparsercontract">ResourceParserContract</a>
 $parser):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="dataexchange#dataexchange_contracts_resourceparsercontract">ResourceParserContract</a>
</td>
        <td>$parser</td>
        <td></td>
    </tr>
</table>


