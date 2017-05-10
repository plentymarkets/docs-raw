

# Accounting<a name="accounting_accounting"></a>
    
## Contracts<a name="accounting_accounting_contracts"></a>
### AccountingServiceContract<a name="accounting_contracts_accountingservicecontract"></a>

Provides methods for location ID detection.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>detectLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the location ID for the given plenty ID and delivery country ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of the system.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The country ID for delivery.</td>
    </tr>
</table>


<pre>public <strong>detectLocationIdByClientId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId = null, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the location ID for the given client ID and delivery country ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The client ID of the system. If client ID is not given, the default client (ID 0) will be used.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The country ID for delivery.</td>
    </tr>
</table>


<pre>public <strong>getAccountingLocations</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List accounting locations for given plenty ID and country ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of the system.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The country ID for delivery.</td>
    </tr>
</table>


<pre>public <strong>getAccountingLocationsByClient</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId = null, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List accounting locations for given client ID and country ID. If client ID is not given, the default client (ID 0) will be used.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The client ID of the system.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The country ID for delivery.</td>
    </tr>
</table>



### DetermineShopCountryContract<a name="accounting_contracts_determineshopcountrycontract"></a>

Provides methods for system country initialization depending the client id.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>initByClientId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Init the system country by the client ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The client ID. [optional, default=0]</td>
    </tr>
</table>


<pre>public <strong>initByPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Init the system country by the plenty ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID. [optional, default=0]</td>
    </tr>
</table>


<pre>public <strong>initByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Init the system country by the location ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The location ID.</td>
    </tr>
</table>


<pre>public <strong>initByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Init the system country by an order ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The order ID.</td>
    </tr>
</table>


<pre>public <strong>getCountryId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the current system country ID (headquarters). One of the init-Methods should be called first!
    
<pre>public <strong>getClientId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the current client ID. One of the init-Methods should be called first!
    
<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the current plenty ID. One of the init-Methods should be called first!
    
<pre>public <strong>getCountryIdByClientId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the shop country (headquarters) for the given client ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The client ID. [optional, default=0]</td>
    </tr>
</table>


<pre>public <strong>getCountryIdByPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the shop country (headquarters) for the given plenty ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID.</td>
    </tr>
</table>


<pre>public <strong>getCountryIdByClientIdAndCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId, <a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the shop country (headquarters) for the given client ID and country ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The client ID.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The country ID.</td>
    </tr>
</table>


<pre>public <strong>getCountryIdByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the shop country (headquarters) for the given location ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The location ID.</td>
    </tr>
</table>


## Exceptions<a name="accounting_accounting_exceptions"></a>
### AccountingException<a name="accounting_exceptions_accountingexception"></a>

Class AccountingException


#### Namespace

`Plenty\Modules\Accounting\Exceptions`


## Models<a name="accounting_accounting_models"></a>
### AccountingLocation<a name="accounting_models_accountinglocation"></a>

The Accounting Location model it is always associated with a client and country and contains the vat configuration, which is displayed in the Vat model.


#### Namespace

`Plenty\Modules\Accounting\Models`


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
            <td>The id of the accounting location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The country Id of the accounting location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the accounting location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>clientId</td>
            <td>The Id of the client, the accounting location belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The plenty id of the client, the accounting location belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>vats</td>
            <td>A collection of vat configurations this accounting location is associated with</td>
        </tr><tr>
            <td><a href="order#order_models_country">Country</a>
</td>
            <td>country</td>
            <td>The country this accounting location belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Vat<a name="accounting_vat"></a>
    
## Contracts<a name="accounting_vat_contracts"></a>
### VatInitContract<a name="accounting_contracts_vatinitcontract"></a>

This interface provides methods to initialize the detection of a VAT configuration and to actually detect VAT rates or VAT fields.


#### Namespace

`Plenty\Modules\Accounting\Vat\Contracts`



#### Methods

<pre>public <strong>init</strong>(<a target="_blank" href="http://php.net/int">int</a> $billingCountryId, <a target="_blank" href="http://php.net/string">string</a> $taxIdNumber, <a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/int">int</a> $shippingCountryId, <a target="_blank" href="http://php.net/string">string</a> $startedAt = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initialize the VAT system data
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$billingCountryId</td>
        <td>The ID of the country of the invoice address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taxIdNumber</td>
        <td>The tax identification number</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the location</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingCountryId</td>
        <td>The ID of the country of the shipping address. [optional, default=0]</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startedAt</td>
        <td>The date when the VAT configuration went into effect. If no date is set, the current date will be used.
[optional, default=null]</td>
    </tr>
</table>


<pre>public <strong>isInitialized</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Get whether the VAT system is already initialized or not
    
<pre>public <strong>getVatField</strong>(<a target="_blank" href="http://php.net/float">float</a> $vatRate, <a target="_blank" href="http://php.net/bool">bool</a> $restrictedToDigitalItems = false):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the VAT field for a VAT rate
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$vatRate</td>
        <td>The VAT rate to be used to find the VAT field</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$restrictedToDigitalItems</td>
        <td>Flag that indicates if the VAT is restricted to digital items or not.
<br />True = the VAT is restricted to digital items
<br />False = the VAT is used for all items</td>
    </tr>
</table>


<pre>public <strong>getVatRate</strong>(<a target="_blank" href="http://php.net/int">int</a> $vatField, <a target="_blank" href="http://php.net/bool">bool</a> $restrictedToDigitalItems = false):<a target="_blank" href="http://php.net/float">float</a></pre>

    
Get the VAT rate of a VAT field
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$vatField</td>
        <td>The VAT field (0-3).</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$restrictedToDigitalItems</td>
        <td>Flag that indicates if the VAT is restricted to digital items or not.
<br />True = the VAT is restricted to digital items
<br />False = the VAT is used for all items</td>
    </tr>
</table>


<pre>public <strong>getUsingVat</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $restrictedToDigitalItems = false):<a href="accounting#accounting_models_vat">Vat</a>
</pre>

    
Get the VAT configuration to be used for VAT calculation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$restrictedToDigitalItems</td>
        <td>Flag that indicates if the VAT is restricted to digital items or not.
<br />True = the VAT is restricted to digital items
<br />False = the VAT is used for all items</td>
    </tr>
</table>


<pre>public <strong>getUsingVatRates</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $restrictedToDigitalItems = false):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the VAT rates to be used for VAT calculation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$restrictedToDigitalItems</td>
        <td>Flag that indicates if the VAT is restricted to digital items or not.
<br />True = the VAT is restricted to digital items
<br />False = the VAT is used for all items</td>
    </tr>
</table>


<pre>public <strong>getStandardVatByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/string">string</a> $startedAt = null):<a href="accounting#accounting_models_vat">Vat</a>
</pre>

    
Get a standard VAT configuration of an accounting location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startedAt</td>
        <td>The date when the VAT configuration went into effect. The date is in W3C format.</td>
    </tr>
</table>



### VatRepositoryContract<a name="accounting_contracts_vatrepositorycontract"></a>

The VatRepositoryContract is the interface for the VAT functionality. This interface allows you to get the VAT configuration for an accounting location and a country of delivery.


#### Namespace

`Plenty\Modules\Accounting\Vat\Contracts`



#### Methods

<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="accounting#accounting_models_vat">Vat</a>
</pre>

    
Get a VAT configuration
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the VAT configuration</td>
    </tr>
</table>


<pre>public <strong>getStandardVat</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId = null, <a target="_blank" href="http://php.net/string">string</a> $startedAt = null):<a href="accounting#accounting_models_vat">Vat</a>
</pre>

    
Get the standard VAT configuration for a plenty ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The ID of the client (store)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startedAt</td>
        <td>The date when the VAT configuration went into effect. The date is given in W3C format.</td>
    </tr>
</table>


<pre>public <strong>findVat</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = \Plenty\Modules\Accounting\Vat\Models\Vat::ITEMS_PER_PAGE, <a target="_blank" href="http://php.net/array">array</a> $relations = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List VAT configurations
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to be returned. If no page is specified, the first page will be returned.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items per page. If not given, the model's default number will be used.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$relations</td>
        <td>The relations to load with the VAT object. The relations available are "location" and "country".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to load in the response</td>
    </tr>
</table>


<pre>public <strong>findVatByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/array">array</a> $relations = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List VAT configurations for an accounting location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$relations</td>
        <td>The relations to load with the VAT object. The relations available are "location" and "country".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to load in the response</td>
    </tr>
</table>


<pre>public <strong>findVatByLocationIdAndCountry</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/int">int</a> $countryId, <a target="_blank" href="http://php.net/array">array</a> $relations = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List VAT configuration for a country of delivery
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country of delivery</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$relations</td>
        <td>The relations to load with the VAT object. The relations available are "location" and "country".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to load in the response.</td>
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
    

### VatServiceContract<a name="accounting_contracts_vatservicecontract"></a>

Provides methods for a quick search of VAT fields, VAT rates and VAT names of a specific VAT configuration.


#### Namespace

`Plenty\Modules\Accounting\Vat\Contracts`



#### Methods

<pre>public <strong>getVatField</strong>(<a href="accounting#accounting_models_vat">Vat</a>
 $vat, <a target="_blank" href="http://php.net/float">float</a> $vatRate):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the VAT field for a VAT rate.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="accounting#accounting_models_vat">Vat</a>
</td>
        <td>$vat</td>
        <td>The VAT configuration of a country</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$vatRate</td>
        <td>The VAT rate</td>
    </tr>
</table>


<pre>public <strong>getVatRate</strong>(<a href="accounting#accounting_models_vat">Vat</a>
 $vat, <a target="_blank" href="http://php.net/int">int</a> $vatField):<a target="_blank" href="http://php.net/float">float</a></pre>

    
Get the VAT rate for a VAT field.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="accounting#accounting_models_vat">Vat</a>
</td>
        <td>$vat</td>
        <td>The VAT configuration of a country</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$vatField</td>
        <td>The VAT field</td>
    </tr>
</table>


<pre>public <strong>getVatName</strong>(<a href="accounting#accounting_models_vat">Vat</a>
 $vat, <a target="_blank" href="http://php.net/int">int</a> $vatField):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the name of a VAT field.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="accounting#accounting_models_vat">Vat</a>
</td>
        <td>$vat</td>
        <td>The VAT configuration of a country</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$vatField</td>
        <td>The VAT field</td>
    </tr>
</table>


## Exceptions<a name="accounting_vat_exceptions"></a>
### VatException<a name="accounting_exceptions_vatexception"></a>

Class VatException


#### Namespace

`Plenty\Modules\Accounting\Vat\Exceptions`


## Models<a name="accounting_vat_models"></a>
### Vat<a name="accounting_models_vat"></a>

The VAT model contains the complete VAT configuration in plentymarkets. The VAT configuration is based on 4 VAT rates. A VAT configuration always belongs to an accounting location. The accounting location is in specified country and is assigne to a client. One accounting location can have several VAT configurations, but only one is active at a time. Which one is active depends on the startedAt date. This also means that only one VAT number is active per accounting location.


#### Namespace

`Plenty\Modules\Accounting\Vat\Models`


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
            <td>The ID of the VAT configuration. A VAT configuration includes 4 VAT rates</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The ID of the country that the VAT configuration belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>taxIdNumber</td>
            <td>The tax id number of VAT configuration.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>startedAt</td>
            <td>The date when the VAT configuration went into effect</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>locationId</td>
            <td>The ID of the location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marginScheme</td>
            <td>Specifies the tax rate that is used, when the margin scheme is applied</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isRestrictedToDigitalItems</td>
            <td>Flag that indicates if the VAT configuration is used only applied to digital goods or not. True= The VAT set is only applied to digital goods. False = The VAT set is applied to all types of goods.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isStandard</td>
            <td>Flag that indicates if the VAT configuration is the standard VAT configuration for the location</td>
        </tr><tr>
            <td><a href="accounting#accounting_models_accountinglocation">AccountingLocation</a>
</td>
            <td>location</td>
            <td>The accounting location that the VAT configuration belongs to. Each accounting location is assigned to a country and only one accounting location is allowed per country.</td>
        </tr><tr>
            <td><a href="order#order_models_country">Country</a>
</td>
            <td>country</td>
            <td>The country that the VAT configuration belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>vatRates</td>
            <td>The VAT rates of a VAT configuration</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VatRate<a name="accounting_models_vatrate"></a>

The VAT rate model is always associated with a VAT configuration and contains the id, name and percentage of a VAT rate. Each VAT configuration can have 4 rates.


#### Namespace

`Plenty\Modules\Accounting\Vat\Models`


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
            <td>The ID of the VAT rate</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatRate</td>
            <td>The percentage of the VAT rate, e.g. 19.00 for 19 %</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of a VAT rate</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
