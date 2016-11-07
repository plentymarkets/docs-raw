

# Accounting<a name="accounting_accounting"></a>
    
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
            <td>The Id of the client, the accounting location belongs to</td>
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
    
returns this model as an array
    
# Newsletter<a name="accounting_newsletter"></a>
    
## Contracts<a name="accounting_newsletter_contracts"></a>
### NewsletterRepositoryContract<a name="accounting_contracts_newsletterrepositorycontract"></a>

Repository for Newsletter

#### Namespace

`Plenty\Modules\Accounting\Newsletter\Contracts`



#### Methods

<pre>public <strong>addToNewsletterList</strong>(<a target="_blank" href="http://php.net/string">string</a> $email, <a target="_blank" href="http://php.net/string">string</a> $forename = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $surname = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $emailDirIds = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    
Add a subscriber to newsletter list
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$email</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$forename</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$surname</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$emailDirIds</td>
        <td></td>
    </tr>
</table>


## Models<a name="accounting_newsletter_models"></a>
### NewsletterEmail<a name="accounting_models_newsletteremail"></a>

NewsletterEmail

#### Namespace

`Plenty\Modules\Accounting\Newsletter\Models`


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
            <td>newsletter email id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directory</td>
            <td>directory id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forename</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>surname</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>gender</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>birthday</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>timestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>templateLang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>confirmedTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>confirmAuthString</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Vat<a name="accounting_vat"></a>
    
## Contracts<a name="accounting_vat_contracts"></a>
### VatRepositoryContract<a name="accounting_contracts_vatrepositorycontract"></a>

The VatRepositoryContract is the interface for the VAT functionality. This interface allows you to get the VAT configuration for an accounting location and a country of delivery.

#### Namespace

`Plenty\Modules\Accounting\Vat\Contracts`



#### Methods

<pre>public <strong>getStandardCountryVat</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId = null):<a href="accounting#accounting_models_vat">Vat</a>
</pre>
    
Get a standard VAT configuration
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The ID of the client (store)</td>
    </tr>
</table>


<pre>public <strong>findVatByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/array">array</a> $relations = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>
    
List VAT configurations for an accounting location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The Id of the accounting location, whose vat configuration is supposed to be loaded</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$relations</td>
        <td>The relations, that are supposed to load with the Vat object. Either "location" or "country" is available.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns, that are supposed to be loaded in the response</td>
    </tr>
</table>


<pre>public <strong>findVatByLocationIdAndCountry</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/int">int</a> $countryId, <a target="_blank" href="http://php.net/array">array</a> $relations = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="accounting#accounting_models_vat">Vat</a>
</pre>
    
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
        <td>The relations, that are supposed to load with the VAT object. The relations available are "location" and "country".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns, that are supposed to be loaded in the response.</td>
    </tr>
</table>


<pre>public <strong>getVatId</strong>(<a href="accounting#accounting_models_vat">Vat</a>
 $vat, <a target="_blank" href="http://php.net/float">float</a> $vatPercentage):<a target="_blank" href="http://php.net/int">int</a></pre>
    
Get vat id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="accounting#accounting_models_vat">Vat</a>
</td>
        <td>$vat</td>
        <td>The Vat object, whose id is searched for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$vatPercentage</td>
        <td>The percentage rate, whose Id is searched for</td>
    </tr>
</table>


<pre>public <strong>determineCountryVat</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $isRestricted, <a target="_blank" href="http://php.net/int">int</a> $contactCountryId, <a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/int">int</a> $deliveryCountryId, <a target="_blank" href="http://php.net/string">string</a> $taxIdNumber = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $date = null):<a href="accounting#accounting_models_vat">Vat</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isRestricted</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactCountryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$deliveryCountryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taxIdNumber</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$date</td>
        <td></td>
    </tr>
</table>


## Models<a name="accounting_vat_models"></a>
### Vat<a name="accounting_models_vat"></a>

The VAT model contains the complete VAT configuration in plentymarkets. The VAT configuration is based on 4 VAT rates. A VAT configuration always belongs to an accounting location. The accounting location is in specified country and is assigne to a client. One accounting location can have several VAT configurations, but only one is active at a time. Which one is active depends on the startDate. This also means that only one VAT number is active per accounting location.

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
            <td>vatNumber</td>
            <td>The VAT number of VAT configuration.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>startDate</td>
            <td>The date when the VAT configuration went into effect</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marginScheme</td>
            <td>Specifies the tax rate that is used, when the margin scheme is applied</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
            <td>digitalRestriction</td>
            <td>Specifies, if the VAT configuration is applied only to digital goods or not. True= The VAT set is only applied to digital goods. False = The VAT set is applied to all types of goods.</td>
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
    
returns this model as an array
    

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
    
returns this model as an array
    
