

# Accounting<a name="accounting_accounting"></a>
    
## Contracts<a name="accounting_accounting_contracts"></a>
### AccountingLocationRepositoryContract<a name="accounting_contracts_accountinglocationrepositorycontract"></a>

The repository to get, create, update and delete accounting locations.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="accounting#accounting_models_accountinglocation">AccountingLocation</a>
</pre>

    
Get an accounting location. The ID of the location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listByPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List accounting locations for a client. The plenty ID of the client must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="accounting#accounting_models_accountinglocation">AccountingLocation</a>
</pre>

    
Create an accounting location.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="accounting#accounting_models_accountinglocation">AccountingLocation</a>
</pre>

    
Update an accounting location. The ID of the location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an accounting location. The ID of the location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>



### AccountingServiceContract<a name="accounting_contracts_accountingservicecontract"></a>

Provides methods to detect a location ID.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>detectLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get a location ID for a country of delivery. The plenty ID must be specified and the ID of the country of delivery can be specified. If the ID of a country is not specified, the ID of the standard location of the specified client will be returned.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of the client (store). The default client will be used if the plenty ID is not specified.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country of delivery. The standard location of the specified client will be returned, if no ID of a country of delivery is specified.</td>
    </tr>
</table>


<pre>public <strong>detectLocationIdByClientId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId = null, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the location ID for a country of delivery. The ID of the client and the ID of the country of delivery can be specified. If neither the client ID nor the ID of a country are specified, the ID of the standard location of the default client will be returned.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The ID of the client. The default client (ID 0) will be used if the ID of client is not specified.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country of delivery. The standard location of the specified client will be returned, if no ID of a country of delivery is specified.</td>
    </tr>
</table>


<pre>public <strong>getAccountingLocations</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List accounting locations. The plenty ID must be specified and the ID of a country of delivery can be specified. If the ID of the country is specified, only one accounting location will be returned. If the ID of the country is not specified, all accounting locations of the client will be returned.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of the client (store).</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country of delivery.</td>
    </tr>
</table>


<pre>public <strong>getAccountingLocationsByClient</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId = null, <a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List accounting locations. The ID of the client and the ID of the country of delivery can be specified. If neither the client ID nor the ID of a country are specified, all accounting locations of the default client will be returned.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The ID of the client. The default client (ID 0) will be used if the ID of client is not specified.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country of delivery.</td>
    </tr>
</table>



### DebtorAccountRepositoryContract<a name="accounting_contracts_debtoraccountrepositorycontract"></a>

The DebtorAccountRepositoryContract is the interface for the DebtorAccountRepository. This interface allows you to either list debtor accounts by locationId or by locationId and mode. The mode describes the criteria that is used to assign pending amounts to debtor accounts.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>findByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a href="accounting#accounting_models_debtoraccountconfiguration">DebtorAccountConfiguration</a>
</pre>

    
Get debtor account configuration of an accounting location. The ID of the accounting location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location.</td>
    </tr>
</table>


<pre>public <strong>listByLocationIdAndMode</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/string">string</a> $mode):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Lists debtor accounts by mode for an accounting location . The mode and the accounting location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mode</td>
        <td>Specifies the mode of the debtor accounts. There are 4 different modes available. These modes are:
<ul>
    <li>character</li>
    <li>country</li>
    <li>payment</li>
    <li>country_payment</li>
</ul>
The modes are described in detail in the DebtorAccountConfiguration model as well as DebtorAccount model.</td>
    </tr>
</table>



### DetermineShopCountryContract<a name="accounting_contracts_determineshopcountrycontract"></a>

This interface provides methods to initialise the country of a location or the country of an order as well as methods to get the ID of a client, the plenty ID of a client, the country or the ID of country.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>initByClientId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initialise the country of the standard location of a client. The ID of the client must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The ID of the client [optional, default=0]</td>
    </tr>
</table>


<pre>public <strong>initByPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initialise the country of the standard location of a client. The plenty ID of the client can be specified. If no plenty ID is specified, the standard client will be used.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of the client [optional]</td>
    </tr>
</table>


<pre>public <strong>initByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initialise the country of a location. The ID of the location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the location</td>
    </tr>
</table>


<pre>public <strong>initByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initialise the country for an order. The ID of the order must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>getCountryId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the ID of the country of the current standard location. One of the initialise methods must be called first. The client that was initialised with the initialise method is your current client.
    
<pre>public <strong>getClientId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the ID of the current client. One of the initialise methods must be called first. The client that was initialised with the initialise method is your current client.
    
<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the plenty ID of the current client. One of the initialise methods must be called first. The client that was initialised with the initialise method is your current client.
    
<pre>public <strong>getCountryIdByClientId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the ID of the country of a client&#039;s standard location. The ID of the client must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The ID of the client. The ID of the default client will be used if no ID is specified [optional, default=0].</td>
    </tr>
</table>


<pre>public <strong>getCountryIdByPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the ID of the country of a client&#039;s standard location. The plenty ID of the client must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of a client</td>
    </tr>
</table>


<pre>public <strong>getCountryIdByClientIdAndCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId, <a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the country of a client&#039;s standard location. The ID of the client and the ID of the country must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The ID of the client.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country.</td>
    </tr>
</table>


<pre>public <strong>getCountryIdByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the country of a location. The ID of the location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the location.</td>
    </tr>
</table>



### PostingKeyRepositoryContract<a name="accounting_contracts_postingkeyrepositorycontract"></a>

The PostingKeyRepositoryContract is the interface for the PostingKeyRepository. This interface provides the functionality to find the posting keys for an accounting location.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>findByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a href="accounting#accounting_models_postingkeyconfiguration">PostingKeyConfiguration</a>
</pre>

    
Get the posting key configuration of an accounting location. The ID of the accounting location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location</td>
    </tr>
</table>



### RevenueAccountRepositoryContract<a name="accounting_contracts_revenueaccountrepositorycontract"></a>

The RevenueAccountRepositoryContract is the interface for the RevenueAccountRepository. This interface allows you to either list revenue accounts by locationId, find by locationId and countryId or to least all for an accounting location.


#### Namespace

`Plenty\Modules\Accounting\Contracts`



#### Methods

<pre>public <strong>listRevenueAccounts</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List revenue account configurations for all accounting locations. Each accounting location has one revenue account configuration.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of revenue accounts to be displayed per page. The default number of revenue accounts is 50.</td>
    </tr>
</table>


<pre>public <strong>findByLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a href="accounting#accounting_models_revenueaccountlocationconfiguration">RevenueAccountLocationConfiguration</a>
</pre>

    
Get the revenue account configuration of an accounting location. The ID of the accounting location must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location</td>
    </tr>
</table>


<pre>public <strong>findByLocationIdAndCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/int">int</a> $countryId):<a href="accounting#accounting_models_revenueaccountcountryconfiguration">RevenueAccountCountryConfiguration</a>
</pre>

    
Get the revenue account configuration of a country. The country account configuration is associated with an accounting location. The ID of the accounting location that the country is associated with as well as the ID of the country must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the accounting location</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The ID of the country</td>
    </tr>
</table>


## Exceptions<a name="accounting_accounting_exceptions"></a>
### AccountingException<a name="accounting_exceptions_accountingexception"></a>

Class AccountingException


#### Namespace

`Plenty\Modules\Accounting\Exceptions`


## Models<a name="accounting_accounting_models"></a>
### AccountingLocation<a name="accounting_models_accountinglocation"></a>

The accounting location model. An accounting location always has a country and belongs to a client. An accounting location contains the VAT configurations. The VAT model contains the VAT configuration.


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
            <td>The ID of the accounting location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The ID of the country of the accounting location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the accounting location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>clientId</td>
            <td>The ID of the client that the accounting location belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The plenty ID of the client that the accounting location belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>vats</td>
            <td>A collection of VAT configurations that are related to the accounting location</td>
        </tr><tr>
            <td><a href="order#order_models_country">Country</a>
</td>
            <td>country</td>
            <td>The country that the accounting location belongs to</td>
        </tr><tr>
            <td><a href="system#system_models_webstore">Webstore</a>
</td>
            <td>client</td>
            <td>The client (store) this accounting location belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### DebtorAccount<a name="accounting_models_debtoraccount"></a>

The DebtorAccountValue Model which contains the actual configured debtor accounts by character, payment and country.


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
            <td>accountId</td>
            <td>The ID of the debtor account configuration that the debtor account belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>mode</td>
            <td>The mode describes the criteria based on which pending amounts are assigned to a debtor account. The following modes are available:
<ul>
<li>character        = The debtor accounts are selected based on the first character of customer information. The information and the order of the information that will be used are defined with the sequence. There are 3 different sequences available.</li>
<li>payment          = The debtor accounts are selected based on the payment method.</li>
<li>country          = The debtor accounts are selected based on the country of delivery.</li>
<li>country_payment  = The debtor accounts are selected based on two criteria. The first criteria is the country and if the country is same as the country of the accounting location then the payment method is used to select the deptor account.</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>The key depends on the debtor account mode.
<ul>
<li>For the character mode the keys are letters. The letters indicate the first letter of the customer information that was used to assign the pending amounts.</li>
<li>For the payment mode the key is the ID of payment method.</li>
<li>For the country mode the key is the ID of the country.</li>
<li>For the country_payment mode the key is either the ID of the country or the ID of payment method. If the country is the same as the country of the accounting location then the payment methods are used to select the deptor account.</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The actual debtor account.</td>
        </tr><tr>
            <td><a href="accounting#accounting_models_debtoraccountconfiguration">DebtorAccountConfiguration</a>
</td>
            <td>account</td>
            <td>The debtor account configuration this account is associated with.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### DebtorAccountConfiguration<a name="accounting_models_debtoraccountconfiguration"></a>

The debtor account configuration model. The configuration is a set of debtor accounts. The actual number of debtor accounts within the configuration depends on the mode used to assign pending amounts to debtor accounts.


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
            <td>The ID of the debtor account configuration</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>locationId</td>
            <td>The ID of the accounting location that the debtor account is associated with.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>mode</td>
            <td>The mode describes the criteria based on which pending amounts are assigned to a debtor account. The following modes are available:
<ul>
<li>character        = The debtor accounts are selected based on the first character of customer information. The information and the order of the information that will be used are defined with the sequence. There are 3 different sequences available.</li>
<li>payment          = The debtor accounts are selected based on the payment method.</li>
<li>country          = The debtor accounts are selected based on the country of delivery.</li>
<li>country_payment  = The debtor accounts are selected based on two criteria. The first criteria is the country and if the country is same as the country of the accounting location then the payment method is used to select the deptor account.</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sequence</td>
            <td>The sequence defines the order in which customer information will be used for the debtor account assignment if the character made has been chosen. The following sequences are available:
<ul>
<li>FNV = stands for the sequence: company, lastname, firstname</li>
<li>NVF = stands for the sequence: lastname, firstname, company</li>
<li>NFV = stands for the sequence: lastname, company, firstname</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>standard</td>
            <td>The standard debtor account that will be used if no matching debtor account can be found.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>save</td>
            <td>Flag that indicates if the debtor account shall be saved within the contact data.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>accounts</td>
            <td>The actual debtor accounts</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PostingKey<a name="accounting_models_postingkey"></a>

The Posting Key Model. A posting key is always associated with an accounting location and holds an posting key for each configured vat rate.


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
            <td>The Id posting key in relation to the vatrate.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The actual posting key for the vat rate.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PostingKeyConfiguration<a name="accounting_models_postingkeyconfiguration"></a>

The posting key configuration model. A posting key configuration is a set of 4 posting keys. A posting key configuration is always associated with an accounting location and can have a posting key per VAT rate. A posting key defines how line items are booked to accounts.


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
            <td>locationId</td>
            <td>The ID of the accounting location that the configuration belongs to</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>postingKeys</td>
            <td>The posting keys for this configuration</td>
        </tr><tr>
            <td><a href="accounting#accounting_models_accountinglocation">AccountingLocation</a>
</td>
            <td>location</td>
            <td>The name of the accounting location that the configuration belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RevenueAccount<a name="accounting_models_revenueaccount"></a>

The revenue account model provides information on a single revenue account. The ID of an account matches the ID of a VAT rate.


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
            <td>The ID of the account. The account IDs are always 0,1,2 or 3. This way the IDs indicate the VAT rate that the account is used for. The revenues that were made with items that have the VAT rate with the ID 0 are assigned to the account with the ID 0.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>account</td>
            <td>The actual account number that was entered in the entry field.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RevenueAccountCountryConfiguration<a name="accounting_models_revenueaccountcountryconfiguration"></a>

The revenue account country configuration model. The revenue account country configuration is a set of up to 4 revenue accounts for one country. Each country that you need to pay VAT in needs a configuration. The 4 revenue account included in the configuration are associated with VAT rates. The VAT rate that one revenue account is associated with can be identified by the ID of the VAT rate. The ID of the VAT rate is included in the account name. Furthermore, each revenue account country configuration is part of a revenue account location configuration. A revenue account country configuration is only available if a VAT configuration for the country exists.


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
            <td>countryId</td>
            <td>The ID of the country that the account configuration belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>revenueAccountLocationId</td>
            <td>The ID configuration of the revenue account that these accounts are for.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>revenueAccounts</td>
            <td>A list of the actual revenue accounts. The accounts are associated with VAT rate. The association can be identified by</td>
        </tr><tr>
            <td><a href="order#order_models_country">Country</a>
</td>
            <td>country</td>
            <td>The country these accounts are associated with.</td>
        </tr><tr>
            <td><a href="accounting#accounting_models_revenueaccountlocationconfiguration">RevenueAccountLocationConfiguration</a>
</td>
            <td>locationConfiguration</td>
            <td>The revenue account configuration these accounts are associated with</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RevenueAccountLocationConfiguration<a name="accounting_models_revenueaccountlocationconfiguration"></a>

The revenue account location configuration model. A revenue account location configuration is the set of all revenue accounts that belong to one accounting location.


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
            <td>The ID of the revenue account configuration</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>locationId</td>
            <td>The ID of the accounting location that the configuration belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountEu</td>
            <td>The account used for revenues that are exempt from VAT and that were sold within the European Union</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountExport</td>
            <td>The account used for revenues that are exempt from VAT and that were sold to outside the European Union</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>revenueAccountCountryConfigurations</td>
            <td>The set of revenue accounts of one country</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Vat<a name="accounting_vat"></a>
    
## Contracts<a name="accounting_vat_contracts"></a>
### VatInitContract<a name="accounting_contracts_vatinitcontract"></a>

This interface provides methods to initialise the detection of a VAT configuration and to actually detect VAT rates or VAT fields.


#### Namespace

`Plenty\Modules\Accounting\Vat\Contracts`



#### Methods

<pre>public <strong>init</strong>(<a target="_blank" href="http://php.net/int">int</a> $billingCountryId, <a target="_blank" href="http://php.net/string">string</a> $taxIdNumber, <a target="_blank" href="http://php.net/int">int</a> $locationId, <a target="_blank" href="http://php.net/int">int</a> $shippingCountryId, <a target="_blank" href="http://php.net/string">string</a> $startedAt = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Initialise the VAT system data
    
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

    
Get whether the VAT system is already initialised or not
    
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

The VAT model contains the complete VAT configuration in plentymarkets. The VAT configuration is based on 4 VAT rates. A VAT configuration always belongs to an accounting location. The accounting location is in a specified country and is assigned to a client. One accounting location can have several VAT configurations, but only one is active at a time. Which one is active depends on the startedAt date. This also means that only one VAT number is active per accounting location.


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

The VAT rate model is always associated with a VAT configuration and contains the ID, name and percentage of a VAT rate. Each VAT configuration can have 4 rates.


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
    
