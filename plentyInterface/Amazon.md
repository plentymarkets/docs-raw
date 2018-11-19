

# Amazon<a name="amazon_amazon"></a>
    
## Contracts<a name="amazon_amazon_contracts"></a>
### AmazonClientFactory<a name="amazon_contracts_amazonclientfactory"></a>




#### Namespace

`Plenty\Modules\Amazon\Contracts`





#### Methods

<pre>public <strong>getClient</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/string">string</a> $endpointPath):<a href="amazon#amazon_contracts_amazonclient">AmazonClient</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$endpointPath</td>
        <td></td>
    </tr>
</table>



### AmazonClientResponse<a name="amazon_contracts_amazonclientresponse"></a>




#### Namespace

`Plenty\Modules\Amazon\Contracts`





#### Methods

<pre>public <strong>getResponseContent</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getResponseMetaData</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### AmazonClient<a name="amazon_contracts_amazonclient"></a>

The amazon client


#### Namespace

`Plenty\Modules\Amazon\Contracts`





#### Methods

<pre>public <strong>sendRequest</strong>(<a href="amazon#amazon_contracts_amazonclientrequest">AmazonClientRequest</a>
 $request, <a target="_blank" href="http://php.net/string">string</a> $serviceVersion):<a href="amazon#amazon_contracts_amazonclientresponse">AmazonClientResponse</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="amazon#amazon_contracts_amazonclientrequest">AmazonClientRequest</a>
</td>
        <td>$request</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$serviceVersion</td>
        <td></td>
    </tr>
</table>



### AmazonClientRequest<a name="amazon_contracts_amazonclientrequest"></a>




#### Namespace

`Plenty\Modules\Amazon\Contracts`





#### Methods

<pre>public <strong>getRequestData</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>requiresSellerId</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getSellerIdFieldName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAction</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### AmazonClientRequestPayload<a name="amazon_contracts_amazonclientrequestpayload"></a>




#### Namespace

`Plenty\Modules\Amazon\Contracts`





#### Methods

<pre>public <strong>getPayload</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Exceptions<a name="amazon_amazon_exceptions"></a>
### AmazonClientException<a name="amazon_exceptions_amazonclientexception"></a>

Created by ptopczewski, 01.02.18 11:41
Class AmazonClientException


#### Namespace

`Plenty\Modules\Amazon\Exceptions`





### AmazonClientRequestException<a name="amazon_exceptions_amazonclientrequestexception"></a>

Created by ptopczewski, 07.02.18 10:34
Class AmazonClientRequestException


#### Namespace

`Plenty\Modules\Amazon\Exceptions`





#### Methods

<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getRequestId</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getErrorCode</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
