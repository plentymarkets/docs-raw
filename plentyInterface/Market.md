

# Credentials<a name="market_credentials"></a>
    
## Contracts<a name="market_credentials_contracts"></a>
### CredentialsRepositoryContract<a name="market_contracts_credentialsrepositorycontract"></a>

The contract for the fitment repository.


#### Namespace

`Plenty\Modules\Market\Credentials\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_credentials">Credentials</a>
</pre>

    
Get credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the credentials.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="market#market_models_credentials">Credentials</a>
</pre>

    
Create credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The credentials data. The properties that are required to update credentials can be found in the credentials model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="market#market_models_credentials">Credentials</a>
</pre>

    
Update credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the credentials.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The credentials data. The properties that are required to update credentials can be found in the credentials model.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the credentials.</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Credentials can be filtered by ID, market, status, environment.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = \Plenty\Modules\Market\Credentials\Models\Credentials::MAX_ITEMS_PER_PAGE):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Credentials can be filtered by ID, market, status, environment.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>Current page of the response.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The requested amount of credentials per result page.</td>
    </tr>
</table>


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
    
## Models<a name="market_credentials_models"></a>
### Credentials<a name="market_models_credentials"></a>

The credentials model


#### Namespace

`Plenty\Modules\Market\Credentials\Models`


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
            <td>The ID of the credentials.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>environment</td>
            <td>The environment for the credentials. Possible values: sandbox, production</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>status</td>
            <td>The status of the credentials. Possible values: active, inactive, pending</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>data</td>
            <td>The data of the credentials.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>market</td>
            <td>The market for the current credentials.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the credentials was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the credentials was updated last.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Api<a name="market_api"></a>
    
## Exceptions<a name="market_api_exceptions"></a>
### InvalidEndPointException<a name="market_exceptions_invalidendpointexception"></a>

InvalidEndPointException.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Exceptions`



#### Methods

<pre>public <strong>getMessage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getLine</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTrace</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getPrevious</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTraceAsString</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### InvalidPropertyTypeException<a name="market_exceptions_invalidpropertytypeexception"></a>

InvalidPropertyTypeException.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Exceptions`



#### Methods

<pre>public <strong>getMessage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getLine</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTrace</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getPrevious</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTraceAsString</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### UnknownPropertyException<a name="market_exceptions_unknownpropertyexception"></a>

InvalidPropertyTypeException.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Exceptions`



#### Methods

<pre>public <strong>getMessage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getLine</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTrace</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getPrevious</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTraceAsString</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Services<a name="market_api_services"></a>
### BaseRestService<a name="market_services_baserestservice"></a>

The service for making eBay REST calls.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Services`



#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $config):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$config</td>
        <td>Configuration option values.</td>
    </tr>
</table>


<pre>public static <strong>getConfigDefinitions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns definitions for each configuration option that is supported.
    
<pre>public <strong>getConfig</strong>(<a target="_blank" href="http://php.net/string">string</a> $option = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get the service&#039;s configuration.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$option</td>
        <td>The name of the option whos value will be returned.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>callOperation</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a href="market#market_types_basetype">BaseType</a>
 $request = null):<a href="market#market_types_basetype">BaseType</a>
</pre>

    
Build API request and send.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The name of the operation.</td>
    </tr>
    <tr>
        <td><a href="market#market_types_basetype">BaseType</a>
</td>
        <td>$request</td>
        <td>Request object containing the request information.</td>
    </tr>
</table>


<pre>public <strong>getEbayHeaders</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Derived classes must implement this method that will build the needed eBay http headers.
    
## Types<a name="market_api_types"></a>
### Base64BinaryType<a name="market_types_base64binarytype"></a>

The service for eBay Base64BinaryType.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### BaseType<a name="market_types_basetype"></a>

The service for base type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Can pass an associative array that will set the objects properties.</td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>



### BooleanType<a name="market_types_booleantype"></a>

The service for boolean type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### DecimalType<a name="market_types_decimaltype"></a>

The service for decimal type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### DoubleType<a name="market_types_doubletype"></a>

The service for double type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### IntegerType<a name="market_types_integertype"></a>

The service for integer type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### RepeatableType<a name="market_types_repeatabletype"></a>

The service for repeatable type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`



#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/string">string</a> $property, <a target="_blank" href="http://php.net/string">string</a> $expectedType):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class that the property is a member of.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$property</td>
        <td>The name of the property that acts like an array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expectedType</td>
        <td>The type that values assigned to the array should be.</td>
    </tr>
</table>


<pre>public <strong>offsetExists</strong>(<a target="_blank" href="http://php.net/int">int</a> $offset):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determines if the offset exists in the array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td>The array index to check.</td>
    </tr>
</table>


<pre>public <strong>offsetGet</strong>(<a target="_blank" href="http://php.net/int">int</a> $offset):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the value of the given offset.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td>The array index.</td>
    </tr>
</table>


<pre>public <strong>offsetSet</strong>($offset, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets a value for the given offset.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$offset</td>
        <td>The array index or null to add the value to the end of the array.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>The value to add.</td>
    </tr>
</table>


<pre>public <strong>offsetUnset</strong>(<a target="_blank" href="http://php.net/int">int</a> $offset):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Unsets the value of the given offset.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td>The array index.</td>
    </tr>
</table>


<pre>public <strong>count</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>current</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>key</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>next</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Move onto the next array index.
    
<pre>public <strong>rewind</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Reset the array index to the start of the array.
    
<pre>public <strong>valid</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### StringType<a name="market_types_stringtype"></a>

The service for string type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### TokenType<a name="market_types_tokentype"></a>

The service for token type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### URIType<a name="market_types_uritype"></a>

The service for uri type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`


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
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>


# PartsFitment<a name="market_partsfitment"></a>
    
## Contracts<a name="market_partsfitment_contracts"></a>
### FitmentItemPropertyRepositoryContract<a name="market_contracts_fitmentitempropertyrepositorycontract"></a>

The contract for the fitment item property repository.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitemproperty">FitmentItemProperty</a>
</pre>

    
Returns a fitment item property by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item property that should be found.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitemproperty">FitmentItemProperty</a>
</pre>

    
Creates a new fitment item property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item property data as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The fitment item ID that the current property should belong to.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>

    
Updates an existing fitment item property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item property data to update as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item property that should be updated.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a fitment item property. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item property that should be deleted.</td>
    </tr>
</table>



### FitmentItemRepositoryContract<a name="market_contracts_fitmentitemrepositorycontract"></a>

The contract for the fitment item repository.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>

    
Returns a fitment item by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The id of the fitment item that should be found.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>

    
Creates a new fitment item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item data as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that the current fitment item belongs to.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>

    
Updates an existing fitment item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item data to update as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item that should be updated.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a fitment item. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item that should be deleted.</td>
    </tr>
</table>



### FitmentRepositoryContract<a name="market_contracts_fitmentrepositorycontract"></a>

The contract for the fitment repository.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="market#market_models_fitment">Fitment</a>
</pre>

    
Returns a fitment by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be found.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Fitment instance. The relations available are 'items', 'items.properties'.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="market#market_models_fitment">Fitment</a>
</pre>

    
Creates a new fitment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment data as associative array.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitment">Fitment</a>
</pre>

    
Updates an existing fitment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment data to update as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be updated.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a fitment. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be deleted.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Search fitments
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Fitment instance. The relations available are 'items', 'items.properties'.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that could be applied: 'id', 'categoryId', 'marketId', 'name', 'property', 'propertyName', 'propertyValue'.</td>
    </tr>
</table>


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
    
## Models<a name="market_partsfitment_models"></a>
### Fitment<a name="market_models_fitment"></a>

The fitment model. This can contain multiple FitmentItems models.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Models`


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
            <td>The id of the fitment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketId</td>
            <td>The id of the market the fitment belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the fitment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryId</td>
            <td>The id of the category the fitment belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>items</td>
            <td>The list of the items that belong to the fitment.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FitmentItem<a name="market_models_fitmentitem"></a>

The fitment item model. This belongs to one fitment model and can contain multiple FitmentItemProperty models.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Models`


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
            <td>The id of the item that belongs to the fitment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>fitmentId</td>
            <td>The id of the fitment.</td>
        </tr><tr>
            <td><a href="market#market_models_fitment">Fitment</a>
</td>
            <td>fitment</td>
            <td>The fitment this fitment item belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>properties</td>
            <td>A collection of this fitment item properties. Available names are 'Make', 'Model', 'Platform', 'Type', 'Production Period', 'Engine', 'FitmentComments', 'KType'.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FitmentItemProperty<a name="market_models_fitmentitemproperty"></a>

The fitment item property model. This bleongs to an FitmentItem model.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Models`


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
            <td>The ID of the fitment item property.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>fitmentItemId</td>
            <td>The ID that the fitment item this property belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property.</td>
        </tr><tr>
            <td><a href="market#market_models_fitmentitem">FitmentItem</a>
</td>
            <td>fitmentItem</td>
            <td>The fitment item this property belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ShopCategory<a name="market_shopcategory"></a>
    
## Contracts<a name="market_shopcategory_contracts"></a>
### ShopCategoryRepositoryContract<a name="market_contracts_shopcategoryrepositorycontract"></a>

The contract for the eBay shop categories.


#### Namespace

`Plenty\Modules\Market\Ebay\ShopCategory\Contracts`



#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $credentialsId, <a target="_blank" href="http://php.net/string">string</a> $viewType = &quot;list&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns a fitment by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$credentialsId</td>
        <td>The credentials ID for whom we want to load the eBay shop categories.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$viewType</td>
        <td>How should the eBay shop categories be returned. Possible values: 'list' or 'tree'. Default is 'list'.</td>
    </tr>
</table>


# Helper<a name="market_helper"></a>
    
## Contracts<a name="market_helper_contracts"></a>
### MarketAttributeHelperRepositoryContract<a name="market_contracts_marketattributehelperrepositorycontract"></a>

The contract for the market attribute helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`



#### Methods

<pre>public <strong>getAttributeName</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the attribute name for the given attribute id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeValueName</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the attribute value name for the given attribute value id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeNames</strong>(<a href="item#item_models_record">Record</a>
 $record, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/string">string</a> $delimiter = &quot;,&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns all attribute names for the given language as a string delimited by the given delimiter.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_record">Record</a>
</td>
        <td>$record</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeValueSetShortFrontendName</strong>(<a href="item#item_models_record">Record</a>
 $record, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/string">string</a> $delimiter = &quot;, &quot;, <a target="_blank" href="http://php.net/array">array</a> $attributeNameCombination = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the attribute value set short frontend name. Ex.: blue, XL
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_record">Record</a>
</td>
        <td>$record</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeNameCombination</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeNameAndValueCombination</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeNames, <a target="_blank" href="http://php.net/string">string</a> $attributeValues, <a target="_blank" href="http://php.net/string">string</a> $delimiter = &quot;,&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the combination of attribute names with their attribute values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeNames</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeValues</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getVariationNameAndAttributeNameAndValueCombination</strong>(<a href="item#item_models_record">Record</a>
 $record, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the name for a variation with all attribute names and attribute values. Ex.: T-Shirt (Size: L, Color: red)
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_record">Record</a>
</td>
        <td>$record</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>



### MarketCategoryHelperRepositoryContract<a name="market_contracts_marketcategoryhelperrepositorycontract"></a>

The contract for the market category helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`



#### Methods

<pre>public <strong>getCategoryBranchName</strong>(<a target="_blank" href="http://php.net/int">int</a> $branchId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/string">string</a> $separator = &quot;&gt;&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the category bread crumbs as string for a given branchId, lang and plentyId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$branchId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$separator</td>
        <td>default</td>
    </tr>
</table>



### MarketItemHelperRepositoryContract<a name="market_contracts_marketitemhelperrepositorycontract"></a>

The contract for the item helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`



#### Methods

<pre>public <strong>getExternalManufacturerName</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the external manufacturer name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateSku</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/float">float</a> $marketId, <a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/bool">bool</a> $setLastExportedTimestamp):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Generates or updates the sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$setLastExportedTimestamp</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $availabilityId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/bool">bool</a> $returnAvailabilityName):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the availability name or the availability average days
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$availabilityId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$returnAvailabilityName</td>
        <td></td>
    </tr>
</table>



### MarketPropertyHelperRepositoryContract<a name="market_contracts_marketpropertyhelperrepositorycontract"></a>

The contract for the market property helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`



#### Methods

<pre>public <strong>getMarketProperty</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrerId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns a list of the market properties
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td></td>
    </tr>
</table>


# Settings<a name="market_settings"></a>
    
## Contracts<a name="market_settings_contracts"></a>
### SettingsRepositoryContract<a name="market_contracts_settingsrepositorycontract"></a>

Use this interface to store and retrieve market specific settings.


#### Namespace

`Plenty\Modules\Market\Settings\Contracts`



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $marketplaceId, <a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/array">array</a> $settings):<a href="market#market_models_settings">Settings</a>
</pre>

    
Create market settings.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$marketplaceId</td>
        <td>The marketplace ID that the settings belong to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of settings. Possible values: shipping, attribute, category, property.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$settings</td>
        <td>The settings that will be saved.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $settingsData, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update one market settings entry.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$settingsData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_settings">Settings</a>
</pre>

    
Return the settings for a given settings ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The settings id.</td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/string">string</a> $marketplaceId, <a target="_blank" href="http://php.net/string">string</a> $type = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Find settings for a given marketplace ID and type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$marketplaceId</td>
        <td>The marketplace id for which to retrieve the settings</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The typo of settings that should be searched for. Possible values: shipping, attribute, category, property.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteAll</strong>(<a target="_blank" href="http://php.net/string">string</a> $marketplaceId, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete all settings for a given type and marketplace ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Factories<a name="market_settings_factories"></a>
### SettingsCorrelationFactory<a name="market_factories_settingscorrelationfactory"></a>

Factory that allows to store correlation between market settings and plentymarkets settings.


#### Namespace

`Plenty\Modules\Market\Settings\Factories`



#### Methods

<pre>public <strong>type</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="market#market_factories_settingscorrelationfactory">SettingsCorrelationFactory</a>
</pre>

    
Set here the type of relation that should be created.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The relation type. Possible values: shipping, attribute, category, property</td>
    </tr>
</table>


<pre>public <strong>createRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $settingsId, <a target="_blank" href="http://php.net/int">int</a> $correlationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Use this method to create a relation of the chosen type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$settingsId</td>
        <td>The id of the market settings we want to create the relation for.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td>The id of the plentymarkets settings we want to create the relation to.</td>
    </tr>
</table>


<pre>public <strong>clear</strong>($marketplaceId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clear all relations for a given correlation type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>($marketplaceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all correlations for a given marketplace ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSettingsByCorrelation</strong>($marketplaceId, <a target="_blank" href="http://php.net/int">int</a> $correlationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a specific settings by marketplace id and correlation id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td></td>
    </tr>
</table>


## Models<a name="market_settings_models"></a>
### Settings<a name="market_models_settings"></a>

The market settings model.


#### Namespace

`Plenty\Modules\Market\Settings\Models`


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
            <td>The id of the market settings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketplaceId</td>
            <td>The id of the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the current settings. Possible values are: attribute, property, category, shipping.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>settings</td>
            <td>The settings for the current marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>category</td>
            <td>The category that this settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>parcelServicePreset</td>
            <td>The parcel service preset that this settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attribute</td>
            <td>The attribute that this settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>property</td>
            <td>The property item that this settings are related to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
