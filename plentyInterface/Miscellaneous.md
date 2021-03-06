

# Plenty<a name="miscellaneous_plenty"></a>
    
## Plugin<a name="miscellaneous_plenty_plugin"></a>
### Application<a name="miscellaneous_plugin_application"></a>

The main application


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>register</strong>(<a target="_blank" href="http://php.net/string">string</a> $providerClassName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a service provider with the application.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$providerClassName</td>
        <td>the classname with namespace of the provider</td>
    </tr>
</table>


<pre>public <strong>bind</strong>(<a target="_blank" href="http://php.net/string">string</a> $abstract, <a target="_blank" href="http://php.net/string">string</a> $concrete = null, <a target="_blank" href="http://php.net/bool">bool</a> $shared = false):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a binding with the container.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$abstract</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$concrete</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$shared</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>singleton</strong>(<a target="_blank" href="http://php.net/string">string</a> $abstract, <a target="_blank" href="http://php.net/string">string</a> $concrete = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a shared binding in the container.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$abstract</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$concrete</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>make</strong>(<a target="_blank" href="http://php.net/string">string</a> $abstract, <a target="_blank" href="http://php.net/array">array</a> $parameters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$abstract</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>makeWith</strong>(<a target="_blank" href="http://php.net/string">string</a> $abstract, <a target="_blank" href="http://php.net/array">array</a> $parameters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$abstract</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>abort</strong>(<a target="_blank" href="http://php.net/int">int</a> $code, <a target="_blank" href="http://php.net/string">string</a> $message = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $headers = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Throw an HttpException with the given data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getWebstoreId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Returns current webstoreId
    
<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>isAdminPreview</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isBackendRequest</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getPluginSetId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getUrlPath</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName = &quot;&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the URL to the plugin resources
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td></td>
    </tr>
</table>



### CachingRepository<a name="miscellaneous_plugin_cachingrepository"></a>

caching repository


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>has</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if an item exists in the cache.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Retrieve an item from the cache by key.
    
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


<pre>public <strong>many</strong>(<a target="_blank" href="http://php.net/array">array</a> $keys):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Retrieve multiple items from the cache by key.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$keys</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>pull</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Retrieve an item from the cache and delete it.
    
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


<pre>public <strong>put</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value, <a target="_blank" href="http://php.net/int">int</a> $minutes = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Store an item in the cache.
    
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
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$minutes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>putMany</strong>(<a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/int">int</a> $minutes):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Store multiple items in the cache for a given number of minutes.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$minutes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value, <a target="_blank" href="http://php.net/int">int</a> $minutes):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Store an item in the cache if the key does not exist.
    
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
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$minutes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>remember</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/int">int</a> $minutes, <a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get an item from the cache, or store the default value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$minutes</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>forget</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Remove an item from the cache.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### Controller<a name="miscellaneous_plugin_controller"></a>

Controller


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>__construct</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Controller constructor.
    

### RouteServiceProvider<a name="miscellaneous_plugin_routeserviceprovider"></a>

Route service provider


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>getApplication</strong>():<a href="miscellaneous#miscellaneous_plugin_application">Application</a>
</pre>

    

    
<pre>public <strong>getEventDispatcher</strong>():<a href="miscellaneous#miscellaneous_events_dispatcher">Dispatcher</a>
</pre>

    

    

### SessionRepository<a name="miscellaneous_plugin_sessionrepository"></a>

session repository


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>has</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the given session value exists.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get the specified session value.
    
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


<pre>public <strong>set</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Set a given session value.
    
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


<pre>public <strong>prepend</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Prepend a value onto an array session value.
    
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


<pre>public <strong>push</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Push a value onto an array session value.
    
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


<pre>public static <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### DataExchangeServiceProvider<a name="miscellaneous_plugin_dataexchangeserviceprovider"></a>

Data Exchange service provider


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>getApplication</strong>():<a href="miscellaneous#miscellaneous_plugin_application">Application</a>
</pre>

    

    
<pre>public <strong>getEventDispatcher</strong>():<a href="miscellaneous#miscellaneous_events_dispatcher">Dispatcher</a>
</pre>

    

    

### ConfigRepository<a name="miscellaneous_plugin_configrepository"></a>

configuration repository


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>has</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the given configuration value exists.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a target="_blank" href="http://php.net/mixed">mixed</a></pre>

    
Get the specified configuration value.
    
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


<pre>public <strong>set</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Set a given configuration value.
    
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


<pre>public <strong>prepend</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Prepend a value onto an array configuration value.
    
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


<pre>public <strong>push</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Push a value onto an array configuration value.
    
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


<pre>public static <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### ServiceProvider<a name="miscellaneous_plugin_serviceprovider"></a>

Service provider for plugins


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>addGlobalMiddleware</strong>(<a target="_blank" href="http://php.net/string">string</a> $middleware):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Add a new middleware to end of the stack if it does not already exist.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$middleware</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getApplication</strong>():<a href="miscellaneous#miscellaneous_plugin_application">Application</a>
</pre>

    

    
<pre>public <strong>getEventDispatcher</strong>():<a href="miscellaneous#miscellaneous_events_dispatcher">Dispatcher</a>
</pre>

    

    

### Middleware<a name="miscellaneous_plugin_middleware"></a>

Middleware


#### Namespace

`Plenty\Plugin`





#### Methods

<pre>public <strong>before</strong>(<a href="miscellaneous#miscellaneous_http_request">Request</a>
 $request):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous_http_request">Request</a>
</td>
        <td>$request</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>after</strong>(<a href="miscellaneous#miscellaneous_http_request">Request</a>
 $request, <a href="miscellaneous#miscellaneous_http_response">Response</a>
 $response):<a href="miscellaneous#miscellaneous_http_response">Response</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous_http_request">Request</a>
</td>
        <td>$request</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_http_response">Response</a>
</td>
        <td>$response</td>
        <td></td>
    </tr>
</table>


## Validation<a name="miscellaneous_plenty_validation"></a>
### Validator<a name="miscellaneous_validation_validator"></a>

Base Validator Class


#### Namespace

`Plenty\Validation`




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
            <td>customMessageKey</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public static <strong>validateOrFail</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>buildCustomMessages</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getAttributeValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $attribute):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get the value of the given attribute.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attribute</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>defineAttributes</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addConditional</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addInt</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addNumeric</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addDate</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addBool</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addString</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>sometimes</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/callable">callable</a> $condition):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
Add a rule for an attribute based on the result of the condition callback.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$condition</td>
        <td></td>
    </tr>
</table>



### DummyAttribute<a name="miscellaneous_validation_dummyattribute"></a>

Dummy Attribute Class


#### Namespace

`Plenty\Validation`





#### Methods

<pre>public <strong>getAttributeName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setAttributeName</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>accepted</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be yes, on, 1, or true. This is useful for validating &quot;Terms of Service&quot; acceptance.
    
<pre>public <strong>activeUrl</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid URL according to the checkdnsrr PHP function.
    
<pre>public <strong>dateAfter</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldNameOrTimeStr):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a value after a given date. The dates will be passed into the strtotime PHP function.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldNameOrTimeStr</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>alphabetic</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be entirely alphabetic characters.
    
<pre>public <strong>alphaDash</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation may have alpha-numeric characters, as well as dashes and underscores.
    
<pre>public <strong>alphaNum</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be entirely alpha-numeric characters.
    
<pre>public <strong>isArray</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a PHP array.
    
<pre>public <strong>dateBefore</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldNameOrTimeStr):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a value preceding the given date. The dates will be passed into the PHP strtotime function.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldNameOrTimeStr</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>between</strong>(<a target="_blank" href="http://php.net/int">int</a> $min, <a target="_blank" href="http://php.net/int">int</a> $max):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have a size between the given min and max. Strings, numerics, and files are evaluated in the same fashion as the size rule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$min</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$max</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>boolean</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be able to be cast as a boolean. Accepted input are true, false, 1, 0, &quot;1&quot;, and &quot;0&quot;.
    
<pre>public <strong>confirmed</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have a matching field of foo_confirmation. For example, if the field under validation is password,
a matching password_confirmation field must be present in the input.
    
<pre>public <strong>date</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid date according to the strtotime PHP function.
    
<pre>public <strong>present</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
Validate that an attribute exists even if not filled.
    
<pre>public <strong>dateFormat</strong>(<a target="_blank" href="http://php.net/string">string</a> $format):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must match the given format. The format will be evaluated using the PHP date_parse_from_format function.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$format</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>different</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have a different value than field.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>digits</strong>(<a target="_blank" href="http://php.net/int">int</a> $count):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be numeric and must have an exact length of $count.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$count</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>digitsBetween</strong>(<a target="_blank" href="http://php.net/int">int</a> $min, <a target="_blank" href="http://php.net/int">int</a> $max):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have a length between the given min and max.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$min</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$max</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>email</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be formatted as an e-mail address.
    
<pre>public <strong>exists</strong>(<a target="_blank" href="http://php.net/string">string</a> $table, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must exist on a given database table.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$table</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>image</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The file under validation must be an image (jpeg, png, bmp, gif, or svg)
    
<pre>public <strong>in</strong>(<a target="_blank" href="http://php.net/array">array</a> $values):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be included in the given list of values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>integer</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be an integer.
    
<pre>public <strong>ip</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be an IP address.
    
<pre>public <strong>json</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must a valid JSON string.
    
<pre>public <strong>max</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be less than or equal to a maximum value. Strings, numerics, and files are evaluated in the same fashion as the size rule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>mimeTypes</strong>(<a target="_blank" href="http://php.net/array">array</a> $types):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The file under validation must have a MIME type corresponding to one of the listed extensions.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$types</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>min</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have a minimum value. Strings, numerics, and files are evaluated in the same fashion as the size rule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>notIn</strong>($values):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must not be included in the given list of values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>numeric</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be numeric.
    
<pre>public <strong>regex</strong>(<a target="_blank" href="http://php.net/string">string</a> $pattern):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must match the given regular expression.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pattern</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>required</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be present in the input data and not empty. A field is considered &quot;empty&quot; is one of the following conditions are true:
The value is null.
    
<pre>public <strong>requiredIf</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, $value):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be present if the anotherfield field is equal to any value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredUnless</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $value):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be present unless the anotherfield field is equal to any value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWith</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be present only if any of the other specified fields are present.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWithAll</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
required_with_all
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWithout</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be present only when any of the other specified fields are not present.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWithoutAll</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be present only when all of the other specified fields are not present.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>notLike</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be not like the specified name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>same</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The given field must match the field under validation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>size</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have a size matching the given value. For string data, value corresponds to the number of characters.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>string</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a string.
    
<pre>public <strong>timezone</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid timezone identifier according to the timezone_identifiers_list PHP function.
    
<pre>public <strong>unique</strong>(<a target="_blank" href="http://php.net/string">string</a> $table, <a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $except = null, <a target="_blank" href="http://php.net/string">string</a> $idColumn = null):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be unique on a given database table. If the column option is not specified, the field name will be used.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$table</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$except</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$idColumn</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>url</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid URL according to PHP&#039;s filter_var function.
    
<pre>public <strong>sometimes</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
In some situations, you may wish to run validation checks against a field only if that field is present in the input array. To quickly accomplish this, add the sometimes rule.
    
<pre>public <strong>nullable</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation may be null. This is particularly useful when validating primitive such as strings
and integers that can contain null values.
    
<pre>public <strong>generateRulesContent</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>dateW3C</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $allowTimestamps = false):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid w3c formated date time string.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$allowTimestamps</td>
        <td>Allow timestamps as a valid format as well.</td>
    </tr>
</table>


<pre>public <strong>customRule</strong>(<a target="_blank" href="http://php.net/string">string</a> $rule, <a target="_blank" href="http://php.net/array">array</a> $params):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
Add custom Role
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$rule</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>validPlentyId</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid plentyId.
    
<pre>public <strong>typeFromDb</strong>(<a target="_blank" href="http://php.net/string">string</a> $table, <a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $attribute, <a target="_blank" href="http://php.net/string">string</a> $comparisonKey = &quot;id&quot;):<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must have the type specified in the database.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$table</td>
        <td>The table with the data type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td>The column with the data type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attribute</td>
        <td>The attribute in the validator with the key</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$comparisonKey</td>
        <td>The column to in $table to compare $attribute to. Default is 'id'.</td>
    </tr>
</table>


<pre>public <strong>hexColor</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>rgbColor</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>cssColor</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>color</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>uuid5</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>validDbType</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid data type used by the validation rule &#039;typeFromDb&#039;.
    
<pre>public <strong>validCurrency</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid currency string (e.g. &#039;EUR&#039;).
    
<pre>public <strong>validBoardTaskReferenceValue</strong>():<a href="miscellaneous#miscellaneous_plenty_validation">Validation</a>
</pre>

    
The field under validation must be a valid board task reference type (e.g. {@link BoardTaskReferenceType::CONTACT}).
    

### RulesCollection<a name="miscellaneous_validation_rulescollection"></a>

RulesCollection


#### Namespace

`Plenty\Validation`





#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addConditional</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addInt</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addNumeric</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addDate</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addBool</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addString</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/bool">bool</a> $required = false):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$required</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>sometimes</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName, <a target="_blank" href="http://php.net/callable">callable</a> $condition):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
Add a rule for an attribute based on the result of the condition callback.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$condition</td>
        <td></td>
    </tr>
</table>


## Exceptions<a name="miscellaneous_plenty_exceptions"></a>
### ValidationException<a name="miscellaneous_exceptions_validationexception"></a>




#### Namespace

`Plenty\Exceptions`




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
            <td>messageBag</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>getMessageBag</strong>():<a href="miscellaneous#miscellaneous_support_messagebag">MessageBag</a>
</pre>

    

    
<pre>public <strong>setMessageBag</strong>(<a href="miscellaneous#miscellaneous_support_messagebag">MessageBag</a>
 $messageBag):<a href="miscellaneous#miscellaneous_plenty_exceptions">Exceptions</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous_support_messagebag">MessageBag</a>
</td>
        <td>$messageBag</td>
        <td></td>
    </tr>
</table>


# ExternalAuth<a name="miscellaneous_externalauth"></a>
    
## Contracts<a name="miscellaneous_externalauth_contracts"></a>
### ExternalAccessRepositoryContract<a name="miscellaneous_contracts_externalaccessrepositorycontract"></a>

Find and create ExternalAccess-datasets


#### Namespace

`Plenty\Plugin\ExternalAuth\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_externalaccess">ExternalAccess</a>
</pre>

    
Create a new ExternalAccess record
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data for the ExternalAccess record to be created with. Must be an associative array with
the keys 'contactId', 'accessType', 'externalContactId' and optionally
an external 'accessToken'.</td>
    </tr>
</table>


<pre>public <strong>findForTypeAndExternalId</strong>(<a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/string">string</a> $externalId):<a href="miscellaneous#miscellaneous_models_externalaccess">ExternalAccess</a>
</pre>

    
Find
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of the external access</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$externalId</td>
        <td>The external ID of the contact</td>
    </tr>
</table>


<pre>public <strong>findForTypeAndContactId</strong>(<a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="miscellaneous#miscellaneous_models_externalaccess">ExternalAccess</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of the external access</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The (internal) ID of the contact</td>
    </tr>
</table>


## Models<a name="miscellaneous_externalauth_models"></a>
### ExternalAccess<a name="miscellaneous_models_externalaccess"></a>

Information on a contact&#039;s external access tokens


#### Namespace

`Plenty\Plugin\ExternalAuth\Models`




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
            <td>contactId</td>
            <td>The ID of the contact in question. Must be unique in combination with $accessType.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accessType</td>
            <td>The type/provider of external access. Must be unique in combination with $contactId.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalContactId</td>
            <td>The ID of the contact at the external provider.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accessToken</td>
            <td>The token for the external access.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>lastUpdate</td>
            <td>The Date when this record was updated the last time.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="miscellaneous_externalauth_services"></a>
### ExternalAuthService<a name="miscellaneous_services_externalauthservice"></a>

Log in users with external auth


#### Namespace

`Plenty\Plugin\ExternalAuth\Services`





#### Methods

<pre>public <strong>logInWithExternalUserId</strong>(<a target="_blank" href="http://php.net/string">string</a> $externalId, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$externalId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


# Plugin<a name="miscellaneous_plugin"></a>
    
## Translation<a name="miscellaneous_plugin_translation"></a>
### Translator<a name="miscellaneous_translation_translator"></a>

translation service


#### Namespace

`Plenty\Plugin\Translation`





#### Methods

<pre>public <strong>trans</strong>(<a target="_blank" href="http://php.net/string">string</a> $id, <a target="_blank" href="http://php.net/array">array</a> $parameters = [], <a target="_blank" href="http://php.net/string">string</a> $locale = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get the translation for a given key.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$locale</td>
        <td></td>
    </tr>
</table>


## Http<a name="miscellaneous_plugin_http"></a>
### Response<a name="miscellaneous_http_response"></a>

Class to create different types of http response.


#### Namespace

`Plenty\Plugin\Http`





#### Methods

<pre>public <strong>status</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the status code for the response.
    
<pre>public <strong>content</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the content of the response.
    
<pre>public <strong>make</strong>(<a target="_blank" href="http://php.net/string">string</a> $content = &quot;&quot;, <a target="_blank" href="http://php.net/int">int</a> $status = 200, <a target="_blank" href="http://php.net/array">array</a> $headers = []):<a href="miscellaneous#miscellaneous_http_response">Response</a>
</pre>

    
Return a new response from the application.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$content</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>view</strong>(<a target="_blank" href="http://php.net/string">string</a> $view, <a target="_blank" href="http://php.net/array">array</a> $data = [], <a target="_blank" href="http://php.net/int">int</a> $status = 200, <a target="_blank" href="http://php.net/array">array</a> $headers = []):<a href="miscellaneous#miscellaneous_http_response">Response</a>
</pre>

    
Return a new view response from the application.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$view</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>json</strong>($data = [], <a target="_blank" href="http://php.net/int">int</a> $status = 200, <a target="_blank" href="http://php.net/array">array</a> $headers = [], <a target="_blank" href="http://php.net/int">int</a> $options):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Return a new JSON response from the application.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>jsonp</strong>(<a target="_blank" href="http://php.net/string">string</a> $callback, $data = [], <a target="_blank" href="http://php.net/int">int</a> $status = 200, <a target="_blank" href="http://php.net/array">array</a> $headers = [], <a target="_blank" href="http://php.net/int">int</a> $options):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Return a new JSONP response from the application.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>stream</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback, <a target="_blank" href="http://php.net/int">int</a> $status = 200, <a target="_blank" href="http://php.net/array">array</a> $headers = []):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Return a new streamed response from the application.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>redirectTo</strong>(<a target="_blank" href="http://php.net/string">string</a> $path, <a target="_blank" href="http://php.net/int">int</a> $status = 302, <a target="_blank" href="http://php.net/array">array</a> $headers = [], <a target="_blank" href="http://php.net/bool">bool</a> $secure = null):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Create a new redirect response to the given path.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$secure</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>redirectToRoute</strong>(<a target="_blank" href="http://php.net/string">string</a> $route, <a target="_blank" href="http://php.net/array">array</a> $parameters = [], <a target="_blank" href="http://php.net/int">int</a> $status = 302, <a target="_blank" href="http://php.net/array">array</a> $headers = []):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Create a new redirect response to a named route.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$route</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>redirectToAction</strong>(<a target="_blank" href="http://php.net/string">string</a> $action, <a target="_blank" href="http://php.net/array">array</a> $parameters = [], <a target="_blank" href="http://php.net/int">int</a> $status = 302, <a target="_blank" href="http://php.net/array">array</a> $headers = []):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Create a new redirect response to a controller action.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$action</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>redirectGuest</strong>(<a target="_blank" href="http://php.net/string">string</a> $path, <a target="_blank" href="http://php.net/int">int</a> $status = 302, <a target="_blank" href="http://php.net/array">array</a> $headers = [], <a target="_blank" href="http://php.net/bool">bool</a> $secure = null):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Create a new redirect response, while putting the current URL in the session.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$secure</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>redirectToIntended</strong>(<a target="_blank" href="http://php.net/string">string</a> $default = &quot;/&quot;, <a target="_blank" href="http://php.net/int">int</a> $status = 302, <a target="_blank" href="http://php.net/array">array</a> $headers = [], <a target="_blank" href="http://php.net/bool">bool</a> $secure = null):<a href="miscellaneous#miscellaneous_httpfoundation_response">Response</a>
</pre>

    
Create a new redirect response to the previously intended location.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$default</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$headers</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$secure</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>sendHeaders</strong>():<a href="miscellaneous#miscellaneous_plugin_http">Http</a>
</pre>

    
Send the HTTP headers without sending the whole response.
    
<pre>public <strong>forceStatus</strong>(<a target="_blank" href="http://php.net/int">int</a> $status = 200):<a href="miscellaneous#miscellaneous_plugin_http">Http</a>
</pre>

    
Force sending response with defined status instead of falling back to default handlers in case of 40* status codes.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$status</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isStatusForced</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Check if response should be send instead of falling back to default handlers in case of 40* status codes.
    

### Request<a name="miscellaneous_http_request"></a>

http request


#### Namespace

`Plenty\Plugin\Http`





#### Methods

<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all of the input and files for the request.
    
<pre>public <strong>merge</strong>(<a target="_blank" href="http://php.net/array">array</a> $input):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Merge new input into the current request&#039;s input array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$input</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>replace</strong>(<a target="_blank" href="http://php.net/array">array</a> $input):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Replace the input for the current request.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$input</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null, <a target="_blank" href="http://php.net/bool">bool</a> $deep = false):<a href="miscellaneous#miscellaneous__void">void</a>
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
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$deep</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getContent</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the request body content.
    
<pre>public <strong>getRequestUri</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the requested URI (path and query string).
    
<pre>public <strong>exists</strong>($key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the request contains a given input item key.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>has</strong>($key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the request contains a non-empty value for an input item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>input</strong>(<a target="_blank" href="http://php.net/string">string</a> $key = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Retrieve an input item from the request.
    
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


<pre>public <strong>only</strong>($keys):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a subset of the items from the input data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$keys</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>except</strong>($keys):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all of the input except for a specified array of items.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$keys</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>query</strong>(<a target="_blank" href="http://php.net/string">string</a> $key = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Retrieve a query string item from the request.
    
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


<pre>public <strong>hasHeader</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if a header is set on the request.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>header</strong>(<a target="_blank" href="http://php.net/string">string</a> $key = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Retrieve a header from the request.
    
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


<pre>public <strong>isJson</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the request is sending JSON.
    
<pre>public <strong>wantsJson</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the current request is asking for JSON in return.
    
<pre>public <strong>accepts</strong>($contentTypes):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determines whether the current requests accepts a given content type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$contentTypes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>prefers</strong>($contentTypes):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Return the most suitable content type from the given array based on content negotiation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$contentTypes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>acceptsJson</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determines whether a request accepts JSON.
    
<pre>public <strong>acceptsHtml</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determines whether a request accepts HTML.
    
<pre>public <strong>format</strong>(<a target="_blank" href="http://php.net/string">string</a> $default = &quot;html&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the data format expected in the response.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getUserInfo</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the user info.
    
<pre>public <strong>getHttpHost</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the HTTP host being requested.
    
<pre>public <strong>getSchemeAndHttpHost</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the scheme and HTTP host.
    
<pre>public <strong>getUri</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Generates a normalized URI (URL) for the Request.
    
<pre>public <strong>getUriForPath</strong>(<a target="_blank" href="http://php.net/string">string</a> $path):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Generates a normalized URI for the given path.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td>A path to use instead of the current one</td>
    </tr>
</table>


<pre>public <strong>getQueryString</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Generates the normalized query string for the Request.
    
<pre>public <strong>getMethod</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the request &quot;intended&quot; method.
    
<pre>public <strong>getLocale</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the locale.
    
## Templates<a name="miscellaneous_plugin_templates"></a>
### Markdown<a name="miscellaneous_templates_markdown"></a>

A simple markdown converter.


#### Namespace

`Plenty\Plugin\Templates`





#### Methods

<pre>public <strong>renderToHtml</strong>(<a target="_blank" href="http://php.net/string">string</a> $markdownContent):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$markdownContent</td>
        <td></td>
    </tr>
</table>



### View<a name="miscellaneous_templates_view"></a>

view support


#### Namespace

`Plenty\Plugin\Templates`





#### Methods

<pre>public <strong>render</strong>(<a target="_blank" href="http://php.net/string">string</a> $templatePath, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$templatePath</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>exists</strong>(<a target="_blank" href="http://php.net/string">string</a> $templatePath):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$templatePath</td>
        <td></td>
    </tr>
</table>



### Twig<a name="miscellaneous_templates_twig"></a>

Twig engine


#### Namespace

`Plenty\Plugin\Templates`





#### Methods

<pre>public <strong>render</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/array">array</a> $context = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Renders a template.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The template name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$context</td>
        <td>An array of parameters to pass to the template</td>
    </tr>
</table>


<pre>public <strong>renderString</strong>(<a target="_blank" href="http://php.net/string">string</a> $templateContent, <a target="_blank" href="http://php.net/array">array</a> $context = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Renders a template from a string.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$templateContent</td>
        <td>The template to render</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$context</td>
        <td>An array of parameters to pass to the template</td>
    </tr>
</table>


<pre>public <strong>addExtension</strong>(<a target="_blank" href="http://php.net/string">string</a> $extension):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Registers an extension.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$extension</td>
        <td>A Twig_ExtensionInterface instance</td>
    </tr>
</table>


## Log<a name="miscellaneous_plugin_log"></a>
### LoggerFactory<a name="miscellaneous_log_loggerfactory"></a>

Logger factory


#### Namespace

`Plenty\Plugin\Log`





#### Methods

<pre>public <strong>getLogger</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginNamespace, <a target="_blank" href="http://php.net/string">string</a> $identifier):<a href="miscellaneous#miscellaneous_contracts_loggercontract">LoggerContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginNamespace</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$identifier</td>
        <td></td>
    </tr>
</table>


## Routing<a name="miscellaneous_plugin_routing"></a>
### Route<a name="miscellaneous_routing_route"></a>

Route


#### Namespace

`Plenty\Plugin\Routing`





#### Methods

<pre>public <strong>addMiddleware</strong>(<a target="_blank" href="http://php.net/array">array</a> $middleware):<a href="miscellaneous#miscellaneous_plugin_routing">Routing</a>
</pre>

    
Add middlewares attached to the route.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$middleware</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>middleware</strong>(<a target="_blank" href="http://php.net/array">array</a> $middleware = []):<a href="miscellaneous#miscellaneous_plugin_routing">Routing</a>
</pre>

    
Get or set the middlewares attached to the route.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$middleware</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMiddleware</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>where</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $expression = null):<a href="miscellaneous#miscellaneous_plugin_routing">Routing</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$expression</td>
        <td></td>
    </tr>
</table>



### Router<a name="miscellaneous_routing_router"></a>

Router service


#### Namespace

`Plenty\Plugin\Routing`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new GET route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>post</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new POST route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>put</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new PUT route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>patch</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new PATCH route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new DELETE route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>options</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new OPTIONS route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>any</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new route responding to all verbs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>match</strong>(<a target="_blank" href="http://php.net/array">array</a> $methods, <a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new route with the given verbs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$methods</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>middleware</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $class):<a href="miscellaneous#miscellaneous_plugin_routing">Routing</a>
</pre>

    
Register a short-hand name for a middleware.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>prepareResponse</strong>(<a href="miscellaneous#miscellaneous_http_request">Request</a>
 $request, <a href="miscellaneous#miscellaneous_http_response">Response</a>
 $response):<a href="miscellaneous#miscellaneous_http_response">Response</a>
</pre>

    
Create a response instance from the given value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous_http_request">Request</a>
</td>
        <td>$request</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_http_response">Response</a>
</td>
        <td>$response</td>
        <td></td>
    </tr>
</table>



### ApiRouter<a name="miscellaneous_routing_apirouter"></a>

Api router service


#### Namespace

`Plenty\Plugin\Routing`





#### Methods

<pre>public <strong>version</strong>(<a target="_blank" href="http://php.net/array">array</a> $version, $second, $third = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$version</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$second</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$third</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new GET route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>post</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new POST route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>put</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new PUT route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>patch</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new PATCH route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new DELETE route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>options</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new OPTIONS route with the router.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>any</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new route responding to all verbs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>resource</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $controller, <a target="_blank" href="http://php.net/array">array</a> $options = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Route a resource to a controller.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$controller</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>match</strong>(<a target="_blank" href="http://php.net/array">array</a> $methods, <a target="_blank" href="http://php.net/string">string</a> $uri, $action):<a href="miscellaneous#miscellaneous_routing_route">Route</a>
</pre>

    
Register a new route with the given verbs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$methods</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$action</td>
        <td></td>
    </tr>
</table>


## Build<a name="miscellaneous_plugin_build"></a>
### CheckProcess<a name="miscellaneous_build_checkprocess"></a>

check process


#### Namespace

`Plenty\Plugin\Build`





#### Methods

<pre>public <strong>addError</strong>(<a target="_blank" href="http://php.net/string">string</a> $message):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
</table>


## Events<a name="miscellaneous_plugin_events"></a>
### Event<a name="miscellaneous_events_event"></a>

Event


#### Namespace

`Plenty\Plugin\Events`





### Dispatcher<a name="miscellaneous_events_dispatcher"></a>

Dispatcher


#### Namespace

`Plenty\Plugin\Events`





#### Methods

<pre>public <strong>isPublicEvent</strong>(<a target="_blank" href="http://php.net/string">string</a> $event):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$event</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listen</strong>($event, $listener, <a target="_blank" href="http://php.net/int">int</a> $priority):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register an event listener with the dispatcher.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$event</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$listener</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$priority</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasListeners</strong>($event):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if a given event has listeners.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$event</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>fire</strong>($event, <a target="_blank" href="http://php.net/array">array</a> $payload = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Fire an event and call the listeners.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$event</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$payload</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>forget</strong>($event):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Remove a set of listeners from the dispatcher.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$event</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getPrefix</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### ShouldQueue<a name="miscellaneous_events_shouldqueue"></a>

Class that allows plugin event listeners to be queued.


#### Namespace

`Plenty\Plugin\Events`




## Error<a name="miscellaneous_plugin_error"></a>
### HTTPException<a name="miscellaneous_error_httpexception"></a>

Created by ptopczewski, 29.12.15 13:48
Class HTTPException


#### Namespace

`Plenty\Plugin\Error`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $statusCode, <a target="_blank" href="http://php.net/string">string</a> $message, <a href="miscellaneous#miscellaneous__exception">Exception</a>
 $previous = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
HTTPException constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$statusCode</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__exception">Exception</a>
</td>
        <td>$previous</td>
        <td></td>
    </tr>
</table>


# Mail<a name="miscellaneous_mail"></a>
    
## Contracts<a name="miscellaneous_mail_contracts"></a>
### MailerContract<a name="miscellaneous_contracts_mailercontract"></a>

Plugin Mailer Service


#### Namespace

`Plenty\Plugin\Mail\Contracts`





#### Methods

<pre>public <strong>sendHtml</strong>(<a target="_blank" href="http://php.net/string">string</a> $html, $recipients, <a target="_blank" href="http://php.net/string">string</a> $subject = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $cc = [], <a target="_blank" href="http://php.net/array">array</a> $bcc = [], <a href="miscellaneous#miscellaneous_models_replyto">ReplyTo</a>
 $replyTo = null, <a target="_blank" href="http://php.net/array">array</a> $attachments = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Send an email containing html
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$html</td>
        <td>The HTML-String for the email body</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$recipients</td>
        <td>Either a string containing a single email address or an array of strings containing multiple email addresses</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$subject</td>
        <td>Optional. The subject of the message</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$cc</td>
        <td>Optional. Array of strings containing email addresses which the message should be sent to as cc</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$bcc</td>
        <td>Optional. Array of strings containing email addresses which the message should be sent to as bcc</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_models_replyto">ReplyTo</a>
</td>
        <td>$replyTo</td>
        <td>Optional. ReplyToRecipient model with mailaddress and name attributes</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attachments</td>
        <td>Optional. A list of StorageObject objects ( see Plenty\Modules\Plugin\Storage\Contracts\StorageRepositoryContract )</td>
    </tr>
</table>


<pre>public <strong>sendFromTwig</strong>(<a target="_blank" href="http://php.net/string">string</a> $twigPath, <a target="_blank" href="http://php.net/array">array</a> $data, $recipients, <a target="_blank" href="http://php.net/string">string</a> $subject = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $altConfig = [], <a target="_blank" href="http://php.net/array">array</a> $cc = [], <a target="_blank" href="http://php.net/array">array</a> $bcc = [], <a href="miscellaneous#miscellaneous_models_replyto">ReplyTo</a>
 $replyTo = null, <a target="_blank" href="http://php.net/array">array</a> $attachments = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Send an email that will get rendered by twig
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$twigPath</td>
        <td>The path to the twig template file that should be used to render the mail. E.g.: 'PluginNamespace::mail.my_mail'</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>An associative array of data that will be available to the twig template</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$recipients</td>
        <td>Either a string containing a single email address or an array of strings containing multiple email addresses</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$subject</td>
        <td>Optional. The subject of the message</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$altConfig</td>
        <td>Optional. Alternative email config. If present MUST be an associative array with the keys 'host', 'port',
'username', 'password' and 'encryption'. It CAN optionally have a key 'from' to set the sender-address
to something else than specified in the system config. If 'from' is missing, the system-wide configured
sender-address is used.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$cc</td>
        <td>Optional. Array of strings containing email addresses which the message should be sent to as cc</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$bcc</td>
        <td>Optional. Array of strings containing email addresses which the message should be sent to as bcc</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_models_replyto">ReplyTo</a>
</td>
        <td>$replyTo</td>
        <td>Optional. ReplyToRecipient model with mailaddress and name attributes</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attachments</td>
        <td>Optional. A list of StorageObject objects ( see Plenty\Modules\Plugin\Storage\Contracts\StorageRepositoryContract )</td>
    </tr>
</table>


<pre>public <strong>sendFromMime</strong>(<a target="_blank" href="http://php.net/string">string</a> $mimeMessage, $recipients, <a target="_blank" href="http://php.net/array">array</a> $altConfig = [], <a target="_blank" href="http://php.net/array">array</a> $cc = [], <a target="_blank" href="http://php.net/array">array</a> $bcc = [], <a href="miscellaneous#miscellaneous_models_replyto">ReplyTo</a>
 $replyTo = null, <a target="_blank" href="http://php.net/array">array</a> $attachments = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Send given message as email
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeMessage</td>
        <td>Complete email mime source header included</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$recipients</td>
        <td>Either a string containing a single email address or an array of strings containing multiple email addresses</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$altConfig</td>
        <td>Optional. Alternative email config. If present MUST be an associative array with the keys 'host', 'port',
'username', 'password' and 'encryption'. It CAN optionally have a key 'from' to set the sender-address
to something else than specified in the system config. If 'from' is missing, the system-wide configured
sender-address is used.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$cc</td>
        <td>Optional. Array of strings containing email addresses which the message should be sent to as cc</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$bcc</td>
        <td>Optional. Array of strings containing email addresses which the message should be sent to as bcc</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_models_replyto">ReplyTo</a>
</td>
        <td>$replyTo</td>
        <td>Optional. ReplyToRecipient model with mailaddress and name attributes</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attachments</td>
        <td>Optional. A list of StorageObject objects ( see Plenty\Modules\Plugin\Storage\Contracts\StorageRepositoryContract )</td>
    </tr>
</table>



### AwsSesContract<a name="miscellaneous_contracts_awssescontract"></a>

Plugin AWS Simple Email Service


#### Namespace

`Plenty\Plugin\Mail\Contracts`





#### Methods

<pre>public <strong>sendEmail</strong>(<a href="miscellaneous#miscellaneous_models_email">Email</a>
 $email, <a href="miscellaneous#miscellaneous_models_awssescredentials">AwsSesCredentials</a>
 $credentials):<a href="miscellaneous#miscellaneous_models_emailsenderresult">EmailSenderResult</a>
</pre>

    
Composes an email message and immediately queues it for sending via AWS SES
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous_models_email">Email</a>
</td>
        <td>$email</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_models_awssescredentials">AwsSesCredentials</a>
</td>
        <td>$credentials</td>
        <td></td>
    </tr>
</table>


## Models<a name="miscellaneous_mail_models"></a>
### Email<a name="miscellaneous_models_email"></a>

the email model.


#### Namespace

`Plenty\Plugin\Mail\Models`




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
            <td>bccAddresses</td>
            <td>BCC email address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>ccAddresses</td>
            <td>CC email address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>toAddresses</td>
            <td>To email address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>senderAddress</td>
            <td>Sender email address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>replyToAddresses</td>
            <td>Reply to email address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>subject</td>
            <td>Email subject</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>htmlBody</td>
            <td>HTML email body</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plainTextBody</td>
            <td>Plain text email body</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>rawMessage</td>
            <td>MIME message, if set subject, html and plainText are ignored</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AwsSesCredentials<a name="miscellaneous_models_awssescredentials"></a>

the credential model for AWS SES client.


#### Namespace

`Plenty\Plugin\Mail\Models`




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
            <td>region</td>
            <td>AWS region e.g. eu-west-1</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accessKeyId</td>
            <td>User access key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>secretAccessKey</td>
            <td>User secret access key</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### EmailSenderResult<a name="miscellaneous_models_emailsenderresult"></a>

the email sender result model.


#### Namespace

`Plenty\Plugin\Mail\Models`




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
            <td>messageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>message</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>errorCode</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ReplyTo<a name="miscellaneous_models_replyto"></a>

ReplyTo


#### Namespace

`Plenty\Plugin\Mail\Models`




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
            <td>mailAddress</td>
            <td>The mail address to reply.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name to reply.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Templates<a name="miscellaneous_templates"></a>
    
## Extensions<a name="miscellaneous_templates_extensions"></a>
### Twig_Extension<a name="miscellaneous_extensions_twig_extension"></a>

Twig extension


#### Namespace

`Plenty\Plugin\Templates\Extensions`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### Twig_SimpleFilter<a name="miscellaneous_extensions_twig_simplefilter"></a>

Twig SimpleFilter


#### Namespace

`Plenty\Plugin\Templates\Extensions`





### Twig_SimpleFunction<a name="miscellaneous_extensions_twig_simplefunction"></a>

Twig SimpleFunction


#### Namespace

`Plenty\Plugin\Templates\Extensions`




## Factories<a name="miscellaneous_templates_factories"></a>
### TwigFactory<a name="miscellaneous_factories_twigfactory"></a>

Twig Factory


#### Namespace

`Plenty\Plugin\Templates\Factories`





#### Methods

<pre>public <strong>register</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>createSimpleFunction</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $callable, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="miscellaneous#miscellaneous_extensions_twig_simplefunction">Twig_SimpleFunction</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$callable</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>An array of parameters</td>
    </tr>
</table>


<pre>public <strong>createSimpleFilter</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $callable, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="miscellaneous#miscellaneous_extensions_twig_simplefilter">Twig_SimpleFilter</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$callable</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>An array of parameters</td>
    </tr>
</table>


# Data<a name="miscellaneous_data"></a>
    
## Contracts<a name="miscellaneous_data_contracts"></a>
### PropertyDescriptor<a name="miscellaneous_contracts_propertydescriptor"></a>

describes properties of a Model


#### Namespace

`Plenty\Plugin\Data\Contracts`





#### Methods

<pre>public <strong>getPropertyInformation</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
        <td></td>
    </tr>
</table>



### Resources<a name="miscellaneous_contracts_resources"></a>

Resource


#### Namespace

`Plenty\Plugin\Data\Contracts`





#### Methods

<pre>public <strong>load</strong>(<a target="_blank" href="http://php.net/string">string</a> $resourceName, <a target="_blank" href="http://php.net/array">array</a> $options = []):<a href="miscellaneous#miscellaneous_model_resourceinformation">ResourceInformation</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$resourceName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$options</td>
        <td>[optional]</td>
    </tr>
</table>


<pre>public <strong>exists</strong>(<a target="_blank" href="http://php.net/string">string</a> $resourceName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$resourceName</td>
        <td></td>
    </tr>
</table>


## Model<a name="miscellaneous_data_model"></a>
### ResourceInformation<a name="miscellaneous_model_resourceinformation"></a>

resource information


#### Namespace

`Plenty\Plugin\Data\Model`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getContentUrl</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getData</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### PropertyInformation<a name="miscellaneous_model_propertyinformation"></a>

property information


#### Namespace

`Plenty\Plugin\Data\Model`





#### Methods

<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDescription</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
# Item<a name="miscellaneous_item"></a>
    
## SalesPrice<a name="miscellaneous_item_salesprice"></a>
### SalesPriceSearchRepository<a name="miscellaneous_salesprice_salespricesearchrepository"></a>

foo


#### Namespace

`Plenty\Legacy\Repositories\Item\SalesPrice`





#### Methods

<pre>public <strong>search</strong>(<a href="item#item_models_salespricesearchrequest">SalesPriceSearchRequest</a>
 $request):<a href="item#item_models_salespricesearchresponse">SalesPriceSearchResponse</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_salespricesearchrequest">SalesPriceSearchRequest</a>
</td>
        <td>$request</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>searchAll</strong>(<a href="item#item_models_salespricesearchrequest">SalesPriceSearchRequest</a>
 $request):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_salespricesearchrequest">SalesPriceSearchRequest</a>
</td>
        <td>$request</td>
        <td></td>
    </tr>
</table>


## Variation<a name="miscellaneous_item_variation"></a>
### SalesPriceService<a name="miscellaneous_variation_salespriceservice"></a>

To be written...


#### Namespace

`Plenty\Legacy\Services\Item\Variation`





#### Methods

<pre>public <strong>getUnitPrice</strong>(<a target="_blank" href="http://php.net/float">float</a> $lot, <a target="_blank" href="http://php.net/float">float</a> $price, <a target="_blank" href="http://php.net/string">string</a> $unit):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$lot</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$price</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$unit</td>
        <td></td>
    </tr>
</table>



### DetectSalesPriceService<a name="miscellaneous_variation_detectsalespriceservice"></a>

To be written...


#### Namespace

`Plenty\Legacy\Services\Item\Variation`





#### Methods

<pre>public <strong>getQuantity</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setQuantity</strong>($quantity):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$quantity</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCurrency</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setCurrency</strong>($currency):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$currency</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPlentyId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setPlentyId</strong>($plentyId):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrderReferrer</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setOrderReferrer</strong>($orderReferrer):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$orderReferrer</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCustomerClass</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setCustomerClass</strong>($customerClass):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$customerClass</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getType</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setType</strong>($type):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCountryOfDelivery</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setCountryOfDelivery</strong>($countryOfDelivery):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$countryOfDelivery</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAccountType</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setAccountType</strong>($accountType):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$accountType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAccountId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setAccountId</strong>($accountId):<a href="miscellaneous#miscellaneous_variation_detectsalespriceservice">DetectSalesPriceService</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$accountId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>detect</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
# Models<a name="miscellaneous_models"></a>
    
## Item<a name="miscellaneous_models_item"></a>
### ItemImageSettings<a name="miscellaneous_item_itemimagesettings"></a>

Configuration of item images


#### Namespace

`Plenty\Legacy\Models\Item`




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
            <td>cdnUrl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxAge</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>imageExportPos</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultExport</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ftpImport</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ftpImportMatching</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannExport</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeImageWidth</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeImageHeight</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>placeholder</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>sizes</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>aliases</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>legacyPreviousSizes</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Repositories<a name="miscellaneous_repositories"></a>
    
## Contracts<a name="miscellaneous_repositories_contracts"></a>
### DeleteResponseContract<a name="miscellaneous_contracts_deleteresponsecontract"></a>

DeleteResponse Interface


#### Namespace

`Plenty\Repositories\Contracts`





#### Methods

<pre>public <strong>getAffectedRows</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setAffectedRows</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>increment</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>decrement</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    

### PaginationResponseContract<a name="miscellaneous_contracts_paginationresponsecontract"></a>

Contract for PaginationResponse


#### Namespace

`Plenty\Repositories\Contracts`





#### Methods

<pre>public <strong>getTotal</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setTotal</strong>($total):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$total</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setPage</strong>($page):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getEntriesPerPage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setEntriesPerPage</strong>($epp):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$epp</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getResult</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setResult</strong>($entries):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$entries</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toJson</strong>(<a target="_blank" href="http://php.net/int">int</a> $options):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Convert the object to its JSON representation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
## Models<a name="miscellaneous_repositories_models"></a>
### DeleteResponse<a name="miscellaneous_models_deleteresponse"></a>

Delete Response


#### Namespace

`Plenty\Repositories\Models`




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
            <td>affectedRows</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaginatedResult<a name="miscellaneous_models_paginatedresult"></a>

paginated result


#### Namespace

`Plenty\Repositories\Models`





#### Methods

<pre>public <strong>getPage</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Returns the page number as received
    
<pre>public <strong>getCurrentPage</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Returns the normalized page number - checked if out of logical bounds
( not below 0, not greater than the last page ) and adjusted
    
<pre>public <strong>getTotalCount</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>isLastPage</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getItemIndexFrom</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getItemIndexTo</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getLastPage</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getResult</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setResult</strong>($result):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$result</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
<pre>public <strong>toJson</strong>(<a target="_blank" href="http://php.net/int">int</a> $options):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Convert the object to its JSON representation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>jsonSerialize</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Specify data which should be serialized to JSON
    

### FilteredPaginatedResult<a name="miscellaneous_models_filteredpaginatedresult"></a>

Filtered paginated result


#### Namespace

`Plenty\Repositories\Models`





#### Methods

<pre>public <strong>getFilters</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the instance as an array.
    
<pre>public <strong>getPage</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Returns the page number as received
    
<pre>public <strong>getCurrentPage</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Returns the normalized page number - checked if out of logical bounds
( not below 0, not greater than the last page ) and adjusted
    
<pre>public <strong>getTotalCount</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>isLastPage</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getItemIndexFrom</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getItemIndexTo</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getLastPage</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getResult</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setResult</strong>($result):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$result</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toJson</strong>(<a target="_blank" href="http://php.net/int">int</a> $options):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Convert the object to its JSON representation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>jsonSerialize</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Specify data which should be serialized to JSON
    
## Criteria<a name="miscellaneous_repositories_criteria"></a>
### PluginCriteria<a name="miscellaneous_criteria_plugincriteria"></a>

The contract for defining criteria.


#### Namespace

`Plenty\Repositories\Criteria`





#### Methods

<pre>public <strong>comparisons</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>apply</strong>($builder, <a href="miscellaneous#miscellaneous_contracts_criteriablecontract">CriteriableContract</a>
 $repository):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$builder</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous_contracts_criteriablecontract">CriteriableContract</a>
</td>
        <td>$repository</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>allowedComparators</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### Comparison<a name="miscellaneous_criteria_comparison"></a>

comparison class


#### Namespace

`Plenty\Repositories\Criteria`





#### Methods

<pre>public <strong>getOperator</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getTerm</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>isOperator</strong>(<a target="_blank" href="http://php.net/string">string</a> $comparison):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$comparison</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>castTerm</strong>(<a target="_blank" href="http://php.net/string">string</a> $castTo):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$castTo</td>
        <td></td>
    </tr>
</table>


# Criteria<a name="miscellaneous_criteria"></a>
    
## Contracts<a name="miscellaneous_criteria_contracts"></a>
### CriteriableContract<a name="miscellaneous_contracts_criteriablecontract"></a>

Interface which provides the possibility to use Criteria filters.


#### Namespace

`Plenty\Repositories\Criteria\Contracts`





#### Methods

<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### ExtendsCriteriaContract<a name="miscellaneous_contracts_extendscriteriacontract"></a>

Interface which provides the possibility to extends repositories with new Criteria filters.


#### Namespace

`Plenty\Repositories\Criteria\Contracts`




## Containers<a name="miscellaneous_criteria_containers"></a>
### CriteriaContainer<a name="miscellaneous_containers_criteriacontainer"></a>

Register repository criteria


#### Namespace

`Plenty\Repositories\Criteria\Containers`





#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/string">string</a> $repository, <a target="_blank" href="http://php.net/string">string</a> $criteria, <a target="_blank" href="http://php.net/string">string</a> $key):<a href="miscellaneous#miscellaneous_criteria_containers">Containers</a>
</pre>

    
Use this method to add criteria to a existing repository.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$repository</td>
        <td>The repository that should use the criteria</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$criteria</td>
        <td>The criteria class name that should be used.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>The key that should match the given criteria.</td>
    </tr>
</table>


# Log<a name="miscellaneous_log"></a>
    
## Contracts<a name="miscellaneous_log_contracts"></a>
### LoggerContract<a name="miscellaneous_contracts_loggercontract"></a>

The contract for the logger.


#### Namespace

`Plenty\Log\Contracts`





#### Methods

<pre>public <strong>report</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Report information.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>debug</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Detailed debug information.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>info</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Interesting events.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>notice</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Normal but significant events.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>warning</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Exceptional occurrences that are not errors.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>error</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Runtime errors that do not require immediate action but should typically
be logged and monitored.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>critical</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Critical conditions.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>alert</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Action must be taken immediately.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>emergency</strong>($code, $additionalInfo = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
System is unusable.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$additionalInfo</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>logException</strong>(<a href="miscellaneous#miscellaneous__exception">Exception</a>
 $exception, <a target="_blank" href="http://php.net/int">int</a> $traceDepth = 3):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Log exceptions.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__exception">Exception</a>
</td>
        <td>$exception</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$traceDepth</td>
        <td>The depth of the stack trace to be logged. Default is 3.</td>
    </tr>
</table>


<pre>public <strong>setReferenceType</strong>(<a target="_blank" href="http://php.net/string">string</a> $referenceType):<a href="miscellaneous#miscellaneous_contracts_loggercontract">LoggerContract</a>
</pre>

    
The reference type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setReferenceValue</strong>($referenceValue):<a href="miscellaneous#miscellaneous_contracts_loggercontract">LoggerContract</a>
</pre>

    
The reference value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$referenceValue</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addReference</strong>(<a target="_blank" href="http://php.net/string">string</a> $referenceType, <a target="_blank" href="http://php.net/int">int</a> $referenceValue):<a href="miscellaneous#miscellaneous_contracts_loggercontract">LoggerContract</a>
</pre>

    
Add reference.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$referenceValue</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPlaceholder</strong>(<a target="_blank" href="http://php.net/string">string</a> $placeholderName, $placeholderValue):<a href="miscellaneous#miscellaneous_contracts_loggercontract">LoggerContract</a>
</pre>

    
Add code placeholder.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$placeholderName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$placeholderValue</td>
        <td></td>
    </tr>
</table>


## Models<a name="miscellaneous_log_models"></a>
### Log<a name="miscellaneous_models_log"></a>

The log entity model


#### Namespace

`Plenty\Log\Models`




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
            <td>The ID of the log entry</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The date when the log entry was created</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>integration</td>
            <td>The integration key used for the log entry. Used as a first level allocation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>identifier</td>
            <td>The identifier used for the log entry. Used as a second level allocation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>code</td>
            <td>The code for this current log entry. For log entries with level "debug", "info", "notice", "warning" and "report" this needs to have an translation in order to be stored.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceType</td>
            <td>Deprecated field, see the <code>references</code> field instead.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>referenceValue</td>
            <td>Deprecated field, see the <code>references</code> field instead.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>level</td>
            <td>The level this current log entry belongs to. Notice! When storing log entries with level "report" the entries will actually be stored as level "info". The difference between "report" and "info" is that log entries with level "report" do not need prior activation.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>additionalInfo</td>
            <td>Additional information that need to also be stored. Can be an int, string or object.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>callerFunction</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>callerLine</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>references</td>
            <td>All the reference types and values correlated with this log entry.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Exceptions<a name="miscellaneous_log_exceptions"></a>
### ReferenceTypeException<a name="miscellaneous_exceptions_referencetypeexception"></a>

Class ReferenceTypeException


#### Namespace

`Plenty\Log\Exceptions`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $message, <a target="_blank" href="http://php.net/int">int</a> $code, <a href="miscellaneous#miscellaneous__exception">Exception</a>
 $previous = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__exception">Exception</a>
</td>
        <td>$previous</td>
        <td></td>
    </tr>
</table>


## Services<a name="miscellaneous_log_services"></a>
### ReferenceContainer<a name="miscellaneous_services_referencecontainer"></a>

Register log reference types.


#### Namespace

`Plenty\Log\Services`





#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/array">array</a> $referenceTypes):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Use this method to add reference types.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$referenceTypes</td>
        <td></td>
    </tr>
</table>


# Search<a name="miscellaneous_search"></a>
    
## Contracts<a name="miscellaneous_search_contracts"></a>
### LogRepositoryContract<a name="miscellaneous_contracts_logrepositorycontract"></a>

Contract for logs.


#### Namespace

`Plenty\Log\Search\Contracts`





#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/string">string</a> $sortBy = &quot;createdAt&quot;, <a target="_blank" href="http://php.net/string">string</a> $sortOrder = &quot;desc&quot;, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_filteredpaginatedresult">FilteredPaginatedResult</a>
</pre>

    
Search logs with the given filters.
    
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
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sortBy</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sortOrder</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>($id):<a href="miscellaneous#miscellaneous_models_log">Log</a>
</pre>

    
Get log entry by id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


# Validation<a name="miscellaneous_validation"></a>
    
## Contracts<a name="miscellaneous_validation_contracts"></a>
### Attribute<a name="miscellaneous_contracts_attribute"></a>

Attribute Interface


#### Namespace

`Plenty\Validation\Contracts`





#### Methods

<pre>public <strong>getAttributeName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setAttributeName</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeName):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>accepted</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be yes, on, 1, or true. This is useful for validating &quot;Terms of Service&quot; acceptance.
    
<pre>public <strong>customRule</strong>(<a target="_blank" href="http://php.net/string">string</a> $rule, <a target="_blank" href="http://php.net/array">array</a> $params):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
Add custom Role
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$rule</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>activeUrl</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid URL according to the checkdnsrr PHP function.
    
<pre>public <strong>dateAfter</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldNameOrTimeStr):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a value after a given date. The dates will be passed into the strtotime PHP function. Instead of passing a date string to be evaluated by strtotime, you may specify another field to compare against the date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldNameOrTimeStr</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>alphabetic</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be entirely alphabetic characters.
    
<pre>public <strong>alphaDash</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation may have alpha-numeric characters, as well as dashes and underscores.
    
<pre>public <strong>alphaNum</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be entirely alpha-numeric characters.
    
<pre>public <strong>isArray</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a PHP array.
    
<pre>public <strong>dateBefore</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldNameOrTimeStr):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a value preceding the given date. The dates will be passed into the PHP strtotime function.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldNameOrTimeStr</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>between</strong>(<a target="_blank" href="http://php.net/int">int</a> $min, <a target="_blank" href="http://php.net/int">int</a> $max):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have a size between the given min and max. Strings, numerics, and files are evaluated in the same fashion as the size rule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$min</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$max</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>boolean</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be able to be cast as a boolean. Accepted input are true, false, 1, 0, &quot;1&quot;, and &quot;0&quot;.
    
<pre>public <strong>confirmed</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have a matching field of foo_confirmation. For example, if the field under validation is password, a matching password_confirmation field must be present in the input.
    
<pre>public <strong>present</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
Validate that an attribute exists even if not filled.
    
<pre>public <strong>date</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid date according to the strtotime PHP function.
    
<pre>public <strong>dateFormat</strong>(<a target="_blank" href="http://php.net/string">string</a> $format):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must match the given format. The format will be evaluated using the PHP date_parse_from_format function. You should use either date or date_format when validating a field, not both.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$format</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>dateW3C</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $allowTimestamps = false):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid w3c formated date time string.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$allowTimestamps</td>
        <td>Allow timestamps as a valid format as well.</td>
    </tr>
</table>


<pre>public <strong>validPlentyId</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid plentyId.
    
<pre>public <strong>typeFromDb</strong>(<a target="_blank" href="http://php.net/string">string</a> $table, <a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $attribute, <a target="_blank" href="http://php.net/string">string</a> $comparisonKey = &quot;id&quot;):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have the type specified in the database.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$table</td>
        <td>The table with the data type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td>The column with the data type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attribute</td>
        <td>The attribute in the validator with the key</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$comparisonKey</td>
        <td>The column to in $table to compare $attribute to. Default is 'id'.</td>
    </tr>
</table>


<pre>public <strong>hexColor</strong>():<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
The field under validation must be a valid HEX color (like &quot;#a3d&quot; or &quot;#a0787c&quot;).
    
<pre>public <strong>rgbColor</strong>():<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
The field under validation must be a valid RGB or RGBA color (like &quot;rgb(0, 200, 150)&quot; or &quot;rgba(0, 200, 150, 0.52)&quot;).
    
<pre>public <strong>cssColor</strong>():<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
The field under validation must be a valid predefined CSS color (like &quot;aquamarine&quot; or &quot;skyblue&quot;).
    
<pre>public <strong>color</strong>():<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
The field under validation must be a valid color (HEX like &quot;#a0787c&quot;, RGB like &quot;rgb(0, 200, 150)&quot; or CSS like &quot;aquamarine&quot;)
    
<pre>public <strong>uuid5</strong>():<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    
The field under validation must be a valid UUID version 5.
    
<pre>public <strong>validDbType</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid data type used by the validation rule &#039;typeFromDb&#039;.
    
<pre>public <strong>validCurrency</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid currency string (e.g. &#039;EUR&#039;).
    
<pre>public <strong>different</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have a different value than field.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>digits</strong>(<a target="_blank" href="http://php.net/int">int</a> $count):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be numeric and must have an exact length of $count.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$count</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>digitsBetween</strong>(<a target="_blank" href="http://php.net/int">int</a> $min, <a target="_blank" href="http://php.net/int">int</a> $max):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have a length between the given min and max.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$min</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$max</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>email</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be formatted as an e-mail address.
    
<pre>public <strong>exists</strong>(<a target="_blank" href="http://php.net/string">string</a> $table, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must exist on a given database table.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$table</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>image</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The file under validation must be an image (jpeg, png, bmp, gif, or svg)
    
<pre>public <strong>in</strong>(<a target="_blank" href="http://php.net/array">array</a> $values):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be included in the given list of values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>integer</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be an integer.
    
<pre>public <strong>ip</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be an IP address.
    
<pre>public <strong>json</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must a valid JSON string.
    
<pre>public <strong>max</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be less than or equal to a maximum value. Strings, numerics, and files are evaluated in the same fashion as the size rule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>mimeTypes</strong>(<a target="_blank" href="http://php.net/array">array</a> $types):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The file under validation must have a MIME type corresponding to one of the listed extensions.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$types</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>min</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have a minimum value. Strings, numerics, and files are evaluated in the same fashion as the size rule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>notIn</strong>($values):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must not be included in the given list of values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>numeric</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be numeric.
    
<pre>public <strong>regex</strong>(<a target="_blank" href="http://php.net/string">string</a> $pattern):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must match the given regular expression.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pattern</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>required</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be present in the input data and not empty. A field is considered &quot;empty&quot; is one of the following conditions are true: The value is null. The value is an empty string. The value is an empty array or empty Countable object. The value is an uploaded file with no path.
    
<pre>public <strong>requiredIf</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, $value):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be present if the anotherfield field is equal to any value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredUnless</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $value):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be present unless the anotherfield field is equal to any value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWith</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be present only if any of the other specified fields are present.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWithAll</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
required_with_all
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWithout</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be present only when any of the other specified fields are not present.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>requiredWithoutAll</strong>(<a target="_blank" href="http://php.net/array">array</a> $fieldNames):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be present only when all of the other specified fields are not present.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fieldNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>notLike</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be not like the specified name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>same</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The given field must match the field under validation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>size</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must have a size matching the given value. For string data, value corresponds to the number of characters. For numeric data, value corresponds to a given integer value. For files, size corresponds to the file size in kilobytes.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>string</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a string.
    
<pre>public <strong>timezone</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid timezone identifier according to the timezone_identifiers_list PHP function.
    
<pre>public <strong>unique</strong>(<a target="_blank" href="http://php.net/string">string</a> $table, <a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $except = null, <a target="_blank" href="http://php.net/string">string</a> $idColumn = null):<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be unique on a given database table. If the column option is not specified, the field name will be used.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$table</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$except</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$idColumn</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>url</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid URL according to PHP&#039;s filter_var function.
    
<pre>public <strong>sometimes</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
In some situations, you may wish to run validation checks against a field only if that field is present in the input array. To quickly accomplish this, add the sometimes rule.
    
<pre>public <strong>nullable</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation may be null. This is particularly useful when validating primitive such as strings and integers that can contain null values.
    
<pre>public <strong>validBoardTaskReferenceValue</strong>():<a href="miscellaneous#miscellaneous_validation_contracts">Contracts</a>
</pre>

    
The field under validation must be a valid board task reference type (e.g. {@link BoardTaskReferenceType::CONTACT}).
    
## Service<a name="miscellaneous_validation_service"></a>
### ValidatorFactory<a name="miscellaneous_service_validatorfactory"></a>

Instantiates Validator Classes


#### Namespace

`Plenty\Validation\Service`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $validatorClass):<a href="miscellaneous#miscellaneous_validation_validator">Validator</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$validatorClass</td>
        <td>The fully qualified classname of the validator to create (including namespace)</td>
    </tr>
</table>



### AttributeFactory<a name="miscellaneous_service_attributefactory"></a>

Instantiates Attribute Classes


#### Namespace

`Plenty\Validation\Service`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $which):<a href="miscellaneous#miscellaneous_contracts_attribute">Attribute</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$which</td>
        <td></td>
    </tr>
</table>


# Illuminate<a name="miscellaneous_illuminate"></a>
    
## Support<a name="miscellaneous_illuminate_support"></a>
### MessageBag<a name="miscellaneous_support_messagebag"></a>




#### Namespace

`Illuminate\Support`





### Collection<a name="miscellaneous_support_collection"></a>




#### Namespace

`Illuminate\Support`





#### Methods

<pre>public <strong>where</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $operator, $value = null):<a href="miscellaneous#miscellaneous_illuminate_support">Support</a>
</pre>

    
Filter items by the given key value pair.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$operator</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>first</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callback = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get the first item from the collection.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$default</td>
        <td></td>
    </tr>
</table>



### ServiceProvider<a name="miscellaneous_support_serviceprovider"></a>




#### Namespace

`Illuminate\Support`




# <a name="miscellaneous_"></a>
    
## Carbon<a name="miscellaneous__carbon"></a>
### Carbon<a name="miscellaneous_carbon_carbon"></a>




#### Namespace

`Carbon`




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
            <td>year</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>yearIso</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>month</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>day</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>hour</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>minute</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>second</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>timestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>timezone</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>tz</td>
            <td></td>
        </tr></tbody>
</table>

# Database<a name="miscellaneous_database"></a>
    
## Eloquent<a name="miscellaneous_database_eloquent"></a>
### Model<a name="miscellaneous_eloquent_model"></a>

Abstract Model class


#### Namespace

`Illuminate\Database\Eloquent`





### Collection<a name="miscellaneous_eloquent_collection"></a>




#### Namespace

`Illuminate\Database\Eloquent`




# Component<a name="miscellaneous_component"></a>
    
## HttpFoundation<a name="miscellaneous_component_httpfoundation"></a>
### Response<a name="miscellaneous_httpfoundation_response"></a>




#### Namespace

`Symfony\Component\HttpFoundation`




