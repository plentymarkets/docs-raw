

# Helper<a name="helper_helper"></a>
    
## Configuration<a name="helper_helper_configuration"></a>
### GetApiCallLimits<a name="helper_configuration_getapicalllimits"></a>

GetApiCallLimits reads the values for the API call limits from the config and returns them as an array.


#### Namespace

`Plenty\Modules\Helper\Configuration`





#### Methods

<pre>public <strong>get</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
## Contracts<a name="helper_helper_contracts"></a>
### UrlBuilderRepositoryContract<a name="helper_contracts_urlbuilderrepositorycontract"></a>

Repository Contract for UrlBuilder


#### Namespace

`Plenty\Modules\Helper\Contracts`





#### Methods

<pre>public <strong>getImageUrl</strong>(<a target="_blank" href="http://php.net/string">string</a> $path, <a target="_blank" href="http://php.net/int">int</a> $plentyId = null, <a target="_blank" href="http://php.net/string">string</a> $size = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $fileType = &quot;&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $isExternalImage = false):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$size</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fileType</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isExternalImage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getItemUrl</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/string">string</a> $urlContent = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $useHttpsDomain = true):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$urlContent</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$useHttpsDomain</td>
        <td></td>
    </tr>
</table>


## Models<a name="helper_helper_models"></a>
### KeyValue<a name="helper_models_keyvalue"></a>

key value data


#### Namespace

`Plenty\Modules\Helper\Models`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $default = null):<a target="_blank" href="http://php.net/mixed">mixed</a></pre>

    

    
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


## Exceptions<a name="helper_helper_exceptions"></a>
### EncryptionException<a name="helper_exceptions_encryptionexception"></a>

Class EncryptionException


#### Namespace

`Plenty\Modules\Helper\Exceptions`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $message, <a target="_blank" href="http://php.net/int">int</a> $code):<a href="miscellaneous#miscellaneous__void">void</a>
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
</table>


## Services<a name="helper_helper_services"></a>
### StringEncodingService<a name="helper_services_stringencodingservice"></a>

Service for encoding strings


#### Namespace

`Plenty\Modules\Helper\Services`





#### Methods

<pre>public <strong>toDatabase</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to self::DATABASE_ENCODING coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toEmail</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to self::EMAIL_ENCODING coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toWebshop</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString, <a target="_blank" href="http://php.net/string">string</a> $sTargetEncoding = self::WEBSHOP_ENCODING):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to self::WEBSHOP_ENCODING coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sTargetEncoding</td>
        <td>[optional default=PlentyCoding::WEBSHOP_ENCODING]</td>
    </tr>
</table>


<pre>public <strong>toAdmin</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString, <a target="_blank" href="http://php.net/string">string</a> $sTargetEncoding = self::ADMIN_ENCODING):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to the sended coding. Default will be self::ADMIN_ENCODING coding used
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sTargetEncoding</td>
        <td>[optional default=PlentyCoding::ADMIN_ENCODING]</td>
    </tr>
</table>


<pre>public <strong>toGwt</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to the sended coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toExport</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString, <a target="_blank" href="http://php.net/string">string</a> $sTargetEncoding = self::EXPORT_ENCODING):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to the sended coding. Default will be self::EXPORT_ENCODING coding used
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sTargetEncoding</td>
        <td>[optional default=PlentyCoding::EXPORT_ENCODING]</td>
    </tr>
</table>


<pre>public <strong>toLegacy</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to self::LEGACY_ENCODING coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toPDF</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString, <a target="_blank" href="http://php.net/string">string</a> $sTargetEncoding = self::PDF_ENCODING):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to self::PDF_ENCODING coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td>The string to be encoded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sTargetEncoding</td>
        <td>The target encoding (since plentymarkets version 5.100). [optional, default=PlentyCoding::PDF_ENCODING]</td>
    </tr>
</table>


<pre>public <strong>toXML</strong>(<a target="_blank" href="http://php.net/string">string</a> $string, <a target="_blank" href="http://php.net/string">string</a> $targetEncoding = self::XML_ENCODING):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method converts a string to self::XML_ENCODING coding.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$string</td>
        <td>The string to be encoded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$targetEncoding</td>
        <td>The target encoding (since plentymarkets version 5.100). [optional, default=PlentyCoding::XML_ENCODING]</td>
    </tr>
</table>


<pre>public <strong>detect_encoding</strong>(<a target="_blank" href="http://php.net/string">string</a> $sString):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Method returns the encoding of one string
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sString</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>convertArray</strong>(<a target="_blank" href="http://php.net/array">array</a> $array, <a target="_blank" href="http://php.net/string">string</a> $sTargetEncoding = self::UTF8_ENCODING, <a target="_blank" href="http://php.net/bool">bool</a> $convertKey = false):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Method converts a multidimensional array to the desired coding
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$array</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sTargetEncoding</td>
        <td>[optional, default=PlentyCoding::UTF8_ENCODING]</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$convertKey</td>
        <td>[optional, default=false]</td>
    </tr>
</table>


<pre>public <strong>cutTextForDB</strong>(<a target="_blank" href="http://php.net/string">string</a> $text, <a target="_blank" href="http://php.net/int">int</a> $lenghtIntoDB):<a target="_blank" href="http://php.net/string">string</a></pre>

    
cut the given text to fit for db insert.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$text</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$lenghtIntoDB</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isValidUtf8</strong>(<a target="_blank" href="http://php.net/string">string</a> $string):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Checks whether the given string is valid utf-8.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$string</td>
        <td></td>
    </tr>
</table>



### WebstoreHelper<a name="helper_services_webstorehelper"></a>

Webstore Helper Service


#### Namespace

`Plenty\Modules\Helper\Services`





#### Methods

<pre>public <strong>getCurrentWebstoreConfiguration</strong>():<a href="system#system_models_webstoreconfiguration">WebstoreConfiguration</a>
</pre>

    

    

### ArrayHelper<a name="helper_services_arrayhelper"></a>

helper class for arrays


#### Namespace

`Plenty\Modules\Helper\Services`





#### Methods

<pre>public <strong>buildMapFromObjectList</strong>($list, <a target="_blank" href="http://php.net/string">string</a> $keyField, <a target="_blank" href="http://php.net/string">string</a> $valueField):<a href="helper#helper_models_keyvalue">KeyValue</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$list</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$keyField</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$valueField</td>
        <td></td>
    </tr>
</table>


# AutomaticEmail<a name="helper_automaticemail"></a>
    
## Contracts<a name="helper_automaticemail_contracts"></a>
### AutomaticEmailContract<a name="helper_contracts_automaticemailcontract"></a>

This service provides a method to initiate the automatic email delivery.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Contracts`





#### Methods

<pre>public <strong>sendAutomatic</strong>(<a href="helper#helper_models_automaticemail">AutomaticEmail</a>
 $email):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Send the automatic email.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="helper#helper_models_automaticemail">AutomaticEmail</a>
</td>
        <td>$email</td>
        <td></td>
    </tr>
</table>


## Models<a name="helper_automaticemail_models"></a>
### AutomaticEmail<a name="helper_models_automaticemail"></a>

A container with all needed data to initiate the automatic email delivery.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AutomaticEmailContact<a name="helper_models_automaticemailcontact"></a>

The automatic email data for contact type emails.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AutomaticEmailData<a name="helper_models_automaticemaildata"></a>

The abstract base class for all automatic email data. Provides constants for the email type to be used.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AutomaticEmailNewsletter<a name="helper_models_automaticemailnewsletter"></a>

The automatic email data for newsletter type emails.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AutomaticEmailTemplate<a name="helper_models_automaticemailtemplate"></a>

Provides constants for the automatic email template names.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AutomaticEmailOrder<a name="helper_models_automaticemailorder"></a>

The automatic email data for order type emails.


#### Namespace

`Plenty\Modules\Helper\AutomaticEmail\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
