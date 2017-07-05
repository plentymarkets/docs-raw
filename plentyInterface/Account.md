

# Address<a name="account_address"></a>
    
## Contracts<a name="account_address_contracts"></a>
### AddressContactRelationRepositoryContract<a name="account_contracts_addresscontactrelationrepositorycontract"></a>

The AddressContactRelationRepositoryContract is the interface for the address contact relation repository.


#### Namespace

`Plenty\Modules\Account\Address\Contracts`



#### Methods

<pre>public <strong>createAddressContactRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Creates address contact relations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateAddressContactRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Updates address contact relations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data as associative array</td>
    </tr>
</table>


<pre>public <strong>findAddressContactRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressContactRelationId):<a href="account#account_models_addresscontactrelation">AddressContactRelation</a>
</pre>

    
Gets address contact relation by ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressContactRelationId</td>
        <td>The ID of the address contact relation</td>
    </tr>
</table>


<pre>public <strong>deleteAddressContactRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressContactRelationId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an address contact relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressContactRelationId</td>
        <td>The ID of the address contact relation</td>
    </tr>
</table>


<pre>public <strong>listAddressContactRelations</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists address contact relations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td>Filter that restricts the search result</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>An array with child instances to be loaded</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
</table>



### AddressPosRelationRepositoryContract<a name="account_contracts_addressposrelationrepositorycontract"></a>

The AddressPosRelationRepositoryContract is the interface for the address POS relation repository.


#### Namespace

`Plenty\Modules\Account\Address\Contracts`



#### Methods

<pre>public <strong>createAddressPosRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_addressposrelation">AddressPosRelation</a>
</pre>

    
Creates an address POS relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateAddressPosRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressPosRelationId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_addressposrelation">AddressPosRelation</a>
</pre>

    
Updates an address POS relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressPosRelationId</td>
        <td>The ID of the address POS relation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data as associative array</td>
    </tr>
</table>


<pre>public <strong>findAddressPosRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressPosRelationId):<a href="account#account_models_addressposrelation">AddressPosRelation</a>
</pre>

    
Lists address POS relations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressPosRelationId</td>
        <td>The ID of the address POS relation</td>
    </tr>
</table>


<pre>public <strong>deleteAddressPosRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressPosRelationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes an address POS relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressPosRelationId</td>
        <td>The ID of the address POS relation</td>
    </tr>
</table>


<pre>public <strong>listAddressPosRelations</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists address POS relations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td>Filter that restricts the search result</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>An array with child instances to be loaded</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
</table>



### AddressRepositoryContract<a name="account_contracts_addressrepositorycontract"></a>

The AddressRepositoryContract is the interface for the address repository contract. This interface allows to get, update, create and delete addresses and address options.


#### Namespace

`Plenty\Modules\Account\Address\Contracts`



#### Methods

<pre>public <strong>findAddressById</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId):<a href="account#account_models_address">Address</a>
</pre>

    
Gets an address. The ID of the address must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
</table>


<pre>public <strong>updateAddress</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $addressId):<a href="account#account_models_address">Address</a>
</pre>

    
Updates an address. The ID of the address must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
</table>


<pre>public <strong>createAddress</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_address">Address</a>
</pre>

    
Creates an address.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data as associative array</td>
    </tr>
</table>


<pre>public <strong>deleteAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an address. The ID of the address must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
</table>


<pre>public <strong>getAddressesOfWarehouse</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/int">int</a> $relationTypeId = null, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Returns a collection of addresses linked with a warehouse.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The ID of the warehouse</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationTypeId</td>
        <td>The ID of the relation type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The quantity of the result</td>
    </tr>
</table>


<pre>public <strong>createAddressOfWarehouse</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_address">Address</a>
</pre>

    
Creates an address and immediately links it with a warehouse.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data to save</td>
    </tr>
</table>


<pre>public <strong>findAddressOptions</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Returns a collection of address options of an address.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>(Optional) The ID of an address option type</td>
    </tr>
</table>


<pre>public <strong>createAddressOptions</strong>(<a target="_blank" href="http://php.net/array">array</a> $addressData, <a target="_blank" href="http://php.net/int">int</a> $addressId):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Creates address options for an address and returns all options of the address.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$addressData</td>
        <td>The address option data as associative array. Multiple options are possible.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address
@MapParam(name="addressData", keyType="string", valueType="mixed")</td>
    </tr>
</table>


<pre>public <strong>updateAddressOptions</strong>(<a target="_blank" href="http://php.net/array">array</a> $addressData, <a target="_blank" href="http://php.net/int">int</a> $addressId):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Updates address options for an address and returns all options of the address.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$addressData</td>
        <td>The address option data as associative array. Multiple options are possible.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
</table>


<pre>public <strong>deleteAddressOptions</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes all address options of an address. The ID of the address must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
</table>


<pre>public <strong>getAddressOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId):<a href="account#account_models_addressoption">AddressOption</a>
</pre>

    
Gets an address option. The ID of the option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td>The ID of the address option</td>
    </tr>
</table>


<pre>public <strong>updateAddressOption</strong>(<a target="_blank" href="http://php.net/array">array</a> $optionData, <a target="_blank" href="http://php.net/int">int</a> $optionId):<a href="account#account_models_addressoption">AddressOption</a>
</pre>

    
Updates an address option. The ID of the address option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$optionData</td>
        <td>The option data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td>The ID of the address option</td>
    </tr>
</table>


<pre>public <strong>deleteAddressOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an address option. The ID of the option must be specified. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td>The ID of the address option</td>
    </tr>
</table>


<pre>public <strong>findAddressRelationTypes</strong>(<a target="_blank" href="http://php.net/string">string</a> $application, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Returns a collection of address relation types by a specific application and language. The collection may be empty.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$application</td>
        <td>The application type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language as ISO 639-1 code (e.g. `en` for english).</td>
    </tr>
</table>


## Models<a name="account_address_models"></a>
### Address<a name="account_models_address"></a>

The address model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name1</td>
            <td>The name 1 field (default: company name)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td>The name 2 field (default: first name)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td>The name 3 field (default: last name)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name4</td>
            <td>The name 4 field (default: c/o)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>companyName</td>
            <td>The company name (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>firstName</td>
            <td>The first name (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastName</td>
            <td>The last name (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>careOf</td>
            <td>The c/o (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>address1</td>
            <td>The address 1 field (street|PACKSTATION|POSTFILIALE)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>address2</td>
            <td>The address 2 field (house no|packstation id)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>address3</td>
            <td>The address 3 field (additional)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>address4</td>
            <td>The address 4 field is currently undefined and can be freely used.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>street</td>
            <td>The street (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>houseNumber</td>
            <td>The house number (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>additional</td>
            <td>The additional address information (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>postalCode</td>
            <td>The postcode</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>town</td>
            <td>The town</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The ID of the country</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stateId</td>
            <td>The ID of the state</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>readOnly</td>
            <td>Flag that indicates if the data record is read only</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sessionId</td>
            <td>The session ID that was used when the address was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>checkedAt</td>
            <td>The time the address was checked as unix timestamp</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The time the address was created as unix timestamp</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The time the address was last updated as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>taxIdNumber</td>
            <td>The taxIdNumber option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td>The externalId option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>entryCertificate</td>
            <td>The entryCertificate option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>phone</td>
            <td>The phone option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td>The email option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>postident</td>
            <td>The PostIdent option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fsk</td>
            <td>The age rating option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>birthday</td>
            <td>The birthday option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>personalNumber</td>
            <td>The personal number option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>packstationNo</td>
            <td>The packstation number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPackstation</td>
            <td>Flag that indicates if the address is a packstation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPostfiliale</td>
            <td>Flag that indicates if the address is a postfiliale (post office)</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>options</td>
            <td>A collection of address options</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>contacts</td>
            <td>A collection of contacts that are linked with the address record</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>orders</td>
            <td>A collection of orders that are linked with the address record</td>
        </tr><tr>
            <td><a href="order#order_models_country">Country</a>
</td>
            <td>country</td>
            <td>The address country</td>
        </tr><tr>
            <td><a href="order#order_models_countrystate">CountryState</a>
</td>
            <td>state</td>
            <td>The address state</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>contactRelations</td>
            <td>A collection of relations to linked contacts</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>orderRelations</td>
            <td>A collection of relations to linked orders</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>warehouseRelations</td>
            <td>A collection of relations to linked warehouses</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>reorderRelations</td>
            <td>A collection of relations to linked reorders</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>schedulerRelations</td>
            <td>A collection of relations to linked schedulers</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressContactRelation<a name="account_models_addresscontactrelation"></a>

The address contact relation model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address contact relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type ID of the address. Possible values:
<ul>
<li>Invoice address = 1</li>
<li>Delivery address = 2</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressId</td>
            <td>The ID of the address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPrimary</td>
            <td>Flag that indicates if the address is primary</td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>address</td>
            <td>The address of the relation</td>
        </tr><tr>
            <td><a href="account#account_models_contact">Contact</a>
</td>
            <td>contact</td>
            <td>The contact of the relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressOption<a name="account_models_addressoption"></a>

The address options model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressId</td>
            <td>The ID of the address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the address option type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The option value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>address</td>
            <td>The address the option belongs to</td>
        </tr><tr>
            <td><a href="account#account_models_addressoptiontype">AddressOptionType</a>
</td>
            <td>type</td>
            <td>The option type of the address option</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressOptionType<a name="account_models_addressoptiontype"></a>

The AddressOptionType model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address option type. It is possible to define individual types. The following types are available by default:
<ul>
<li>1 = VAT number</li>
<li>2 = External address ID</li>
<li>3 = Entry certificate</li>
<li>4 = Telephone</li>
<li>5 = Email</li>
<li>6 = Post number</li>
<li>7 = Personal id</li>
<li>8 = BBFC</li>
<li>9 = Birthday</li>
<li>10 = Session ID</li>
<li>11 = Title</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>nonErasable</td>
            <td>Flag that indicates if the type can be deleted</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>names</td>
            <td>A collection of address option type names</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>options</td>
            <td>A collection of all address options of the type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressOptionTypeName<a name="account_models_addressoptiontypename"></a>

The AddressOptionTypeName model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address option type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the address option type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name</td>
        </tr><tr>
            <td><a href="account#account_models_addressoptiontype">AddressOptionType</a>
</td>
            <td>type</td>
            <td>The address option type that belongs to the name</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressOrderRelation<a name="account_models_addressorderrelation"></a>

address order relation model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address order relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the address type
<ul>
		<li>Billing address = 1</li>
		<li>Delivery address = 2</li>
		<li>Sender address = 3</li>
		<li>Return address = 4</li>
		<li>Client address = 5</li>
		<li>Contractor address = 6</li>
		<li>Warehouse address = 7</li>
	</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressId</td>
            <td>The ID of the address</td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>address</td>
            <td>The address of the relation</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order of the relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressPosRelation<a name="account_models_addressposrelation"></a>

The address POS relation model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address POS relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>posBaseId</td>
            <td>The ID of the POS base</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>addressId</td>
            <td>The ID of the address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the relation type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressRelationType<a name="account_models_addressrelationtype"></a>

The contact address type model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address relation type. The following types are available by default and cannot be deleted:
<ul>
<li>1 = Billing address</li>
<li>2 = Delivery address</li>
<li>3 = Sender address</li>
<li>4 = Return address</li>
<li>5 = Client address</li>
<li>6 = Contractor address</li>
<li>7 = Warehouse address</li>
<li>8 = POS address</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>nonErasable</td>
            <td>Flag that indicates if the type can be deleted</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>names</td>
            <td>A collection of AddressRelationTypeName objects</td>
        </tr><tr>
            <td><a href="account#account_models_addressrelationtypeapplication">AddressRelationTypeApplication</a>
</td>
            <td>application</td>
            <td>The address relation type application</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressRelationTypeApplication<a name="account_models_addressrelationtypeapplication"></a>

The AddressRelationTypeApplication model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address relation type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>application</td>
            <td>The application type. Allowed values: contact, order, warehouse.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a href="account#account_models_addressrelationtype">AddressRelationType</a>
</td>
            <td>type</td>
            <td>The type of the address relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressRelationTypeName<a name="account_models_addressrelationtypename"></a>

The AddressRelationTypeName model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address relation type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name</td>
        </tr><tr>
            <td><a href="account#account_models_addressrelationtype">AddressRelationType</a>
</td>
            <td>type</td>
            <td>The type of the address relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressSchedulerRelation<a name="account_models_addressschedulerrelation"></a>

The AddressSchedulerRelation model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address order relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerId</td>
            <td>The ID of the scheduler</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the address type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressId</td>
            <td>The ID of the address</td>
        </tr><tr>
            <td><a href="order#order_models_orderscheduler">OrderScheduler</a>
</td>
            <td>scheduler</td>
            <td>The scheduler of the order</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AddressWarehouseRelation<a name="account_models_addresswarehouserelation"></a>

The AddressWarehouseRelation model


#### Namespace

`Plenty\Modules\Account\Address\Models`


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
            <td>The ID of the address warehouse relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The ID of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressId</td>
            <td>The ID of the address</td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>address</td>
            <td>The address of the relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ContactEvent<a name="account_contactevent"></a>
    
## Contracts<a name="account_contactevent_contracts"></a>
### ContactEventRepositoryContract<a name="account_contracts_contacteventrepositorycontract"></a>

The ContactEventRepositoryContract is the interface for the contact event repository. This interface allows to list contact events.


#### Namespace

`Plenty\Modules\Account\Contact\ContactEvent\Contracts`



#### Methods

<pre>public <strong>listEvents</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists contact events identified by the contact that is currently logged into the system.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
</table>


## Models<a name="account_contactevent_models"></a>
### ContactEvent<a name="account_models_contactevent"></a>

The contact event model


#### Namespace

`Plenty\Modules\Account\Contact\ContactEvent\Models`


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
            <td>eventId</td>
            <td>The ID of the event</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact this event belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the user this event belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>eventDuration</td>
            <td>The duration of the event in seconds</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>eventType</td>
            <td>The type of the event</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderRowId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>eventInfo</td>
            <td>Informational text about the event</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>billable</td>
            <td>Billable if set to 1</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>eventInsertedAt</td>
            <td>The date the event was created at as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>eventBilledAt</td>
            <td>The date the event was billed at as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>eventProvisionPaidAt</td>
            <td>The date the provision was paid at as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>eventCreditValue</td>
            <td>The credit value of the event</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Contact<a name="account_contact"></a>
    
## Contracts<a name="account_contact_contracts"></a>
### ContactAccountRepositoryContract<a name="account_contracts_contactaccountrepositorycontract"></a>

The ContactAccountRepositoryContract is the interface for the contact account repository. This interface allows to get, create, update and delete accounts. An account contains company-related data.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>findAccount</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="account#account_models_account">Account</a>
</pre>

    
Returns an account by an ID only if it is associated with the given contact ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>createAccount</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="account#account_models_account">Account</a>
</pre>

    
Creates an account and associates it immediately with the given ID of the contact.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The account data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact to associate this to</td>
    </tr>
</table>


<pre>public <strong>updateAccount</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="account#account_models_account">Account</a>
</pre>

    
Updates an account. If not already associated, it will associate the account with the given contact ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The account data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>deleteAccount</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes the given account of the given contact ID. Returns `true` if the deletion was successful. Returns `false` if the deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>



### ContactAddressRepositoryContract<a name="account_contracts_contactaddressrepositorycontract"></a>

The ContactAddressRepositoryContract is the interface for the contact address repository. This interface allows to list, get, create, update, add and delete addresses of the contact.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>findContactAddressByTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/bool">bool</a> $last = true):<a href="account#account_models_address">Address</a>
</pre>

    
Returns an address of a given contact for the given type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$last</td>
        <td>Return the last created billing address</td>
    </tr>
</table>


<pre>public <strong>createAddress</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Creates an address, associates it immediately with the given contact ID with the given type and returns the new address.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>updateAddress</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Updates the existing address of a given contact and type and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address to update</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>getAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Returns the address of a given contact and type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>getAddresses</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets all addresses for the given contact of the given type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The address type (default: all / null)</td>
    </tr>
</table>


<pre>public <strong>addAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Adds the address to the given contact as the given type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>setPrimaryAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $addressTypeId):<a href="account#account_models_addresscontactrelation">AddressContactRelation</a>
</pre>

    
Sets a contact address per address type as the primary address.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressTypeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>deleteAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an existing address of a given contact and type. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>



### ContactClassRepositoryContract<a name="account_contracts_contactclassrepositorycontract"></a>

The ContactClassRepositoryContract is the interface for the contact class repository. This interface allows to list all contact classes or to get a contact class by the ID.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>findContactClassById</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactClassId):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets a contact class. The ID of the contact class must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactClassId</td>
        <td>The ID of the contact class</td>
    </tr>
</table>


<pre>public <strong>allContactClasses</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists contact classes.
    

### ContactOptionRepositoryContract<a name="account_contracts_contactoptionrepositorycontract"></a>

The ContactOptionRepositoryContract is the interface for the contact option repository. This interface allows to get, create, update and delete contact options.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>findContactOptions</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/int">int</a> $subTypeId):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Lists options of the contact. The ID of the contact must be specified. The ID of the option type and the ID of the option sub-type can be optionally used.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>Optional: The ID of the option type (default: 0)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$subTypeId</td>
        <td>Optional: The ID of the option sub-type (default: 0)</td>
    </tr>
</table>


<pre>public <strong>createContactOptions</strong>(<a target="_blank" href="http://php.net/array">array</a> $optionData, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Creates an option for the given contact and returns them.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$optionData</td>
        <td>The option data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>updateContactOptions</strong>(<a target="_blank" href="http://php.net/array">array</a> $optionData, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Updates options of the given contact and returns them. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$optionData</td>
        <td>The option data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>deleteContactOptionsByContactId</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes all options of the given contact. The ID of the contact must be specified. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>findContactOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId):<a href="account#account_models_contactoption">ContactOption</a>
</pre>

    
Gets a contact option. The ID of the option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td>The ID of the option</td>
    </tr>
</table>


<pre>public <strong>updateContactOption</strong>(<a target="_blank" href="http://php.net/array">array</a> $optionData, <a target="_blank" href="http://php.net/int">int</a> $optionId):<a href="account#account_models_contactoption">ContactOption</a>
</pre>

    
Updates an option with the given id and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$optionData</td>
        <td>The option data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td>The ID of the option</td>
    </tr>
</table>


<pre>public <strong>deleteContactOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $optionId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a contact option. The ID of the option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$optionId</td>
        <td>The ID of the option</td>
    </tr>
</table>



### ContactPaymentRepositoryContract<a name="account_contracts_contactpaymentrepositorycontract"></a>

The ContactPaymentRepositoryContract is the interface for the contact payment repository. This interface allows to list, get, create, update and delete bank details of the contact.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>getBanksOfContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets a collection of bank accounts of a contact. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to retrieve (Default: '[*]')</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>Optional: The number of bank accounts per page (Default: 50)</td>
    </tr>
</table>


<pre>public <strong>getBankByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Returns bank details of an order. The ID of the order must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to retrieve (Default: '[*]')</td>
    </tr>
</table>


<pre>public <strong>createContactBank</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Creates a bank account for a contact and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The bank account data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateContactBank</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $contactBankId):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Updates a bank account. The ID of the bank account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The bank data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactBankId</td>
        <td>The ID of the bank account entry</td>
    </tr>
</table>


<pre>public <strong>deleteContactBank</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactBankId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a bank account. The ID of the bank account must be specified. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactBankId</td>
        <td>The ID of the bank account entry</td>
    </tr>
</table>


<pre>public <strong>findContactBankById</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactBankId):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Gets a bank account. The ID of the bank account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactBankId</td>
        <td>The ID of the bank account entry</td>
    </tr>
</table>



### ContactRepositoryContract<a name="account_contracts_contactrepositorycontract"></a>

The ContactRepositoryContract is the interface for the contact repository. This interface allows to list, get, create, update and delete contacts. A contact is equivalent to a person.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>createContact</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_contact">Contact</a>
</pre>

    
Creates a contact and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The contact data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateContact</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="account#account_models_contact">Contact</a>
</pre>

    
Updates a contact and returns it. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The contact data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>deleteContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/bool">bool</a> $checkExistingOrders = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a contact. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$checkExistingOrders</td>
        <td>Flag that checks if the contact is linked to orders. If the contact is linked to orders, CustomerDeleteException is thrown and the contact will not be deleted.</td>
    </tr>
</table>


<pre>public <strong>findContactById</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="account#account_models_contact">Contact</a>
</pre>

    
Gets a contact. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relationships that should be eager loaded</td>
    </tr>
</table>


<pre>public <strong>getContactList</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List contacts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td>Filter that restrict the search result</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relationships that should be eager loaded</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
</table>


<pre>public <strong>getContactByOptionValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $value, <a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/int">int</a> $subTypeId):<a href="account#account_models_contact">Contact</a>
</pre>

    
Returns an existing contact by a contact option information.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td>The value of the contact option</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The type ID of the contact option</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$subTypeId</td>
        <td>The sub-type ID of the contact option</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### ContactTypeRepositoryContract<a name="account_contracts_contacttyperepositorycontract"></a>

The ContactTypeRepositoryContract is the interface for the contact type repository. This interface allows to list, get, create, update and delete contact types.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>createContactType</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_contacttype">ContactType</a>
</pre>

    
Creates a contact type and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The contact type data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateContactType</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $contactTypeId):<a href="account#account_models_contacttype">ContactType</a>
</pre>

    
Updates a contact type and returns it. The ID of the contact type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The contact type data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactTypeId</td>
        <td>The ID of the contact type</td>
    </tr>
</table>


<pre>public <strong>deleteContactType</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactTypeId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a contact type. The ID of the contact type must be specified. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactTypeId</td>
        <td>The ID of the contact type</td>
    </tr>
</table>


<pre>public <strong>findContactTypeById</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactTypeId):<a href="account#account_models_contacttype">ContactType</a>
</pre>

    
Gets a contact type. The ID of the contact type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactTypeId</td>
        <td>The ID of the contact type</td>
    </tr>
</table>


<pre>public <strong>allContactTypes</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns a collection of contact types.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to return as an array (Default: '[*]')</td>
    </tr>
</table>



### InternalContactPaymentRepositoryContract<a name="account_contracts_internalcontactpaymentrepositorycontract"></a>

The contract for the contact payment repository.


#### Namespace

`Plenty\Modules\Account\Contact\Contracts`



#### Methods

<pre>public <strong>getBanksOfContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets a collection of bank accounts of a contact. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to retrieve (Default: '[*]')</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>Optional: The number of bank accounts per page (Default: 50)</td>
    </tr>
</table>


<pre>public <strong>getBankByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Returns bank details of an order. The ID of the order must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to retrieve (Default: '[*]')</td>
    </tr>
</table>


<pre>public <strong>createContactBank</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Creates a bank account for a contact and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The bank account data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateContactBank</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $contactBankId):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Updates a bank account. The ID of the bank account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The bank data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactBankId</td>
        <td>The ID of the bank account entry</td>
    </tr>
</table>


<pre>public <strong>deleteContactBank</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactBankId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a bank account. The ID of the bank account must be specified. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactBankId</td>
        <td>The ID of the bank account entry</td>
    </tr>
</table>


<pre>public <strong>findContactBankById</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactBankId):<a href="account#account_models_contactbank">ContactBank</a>
</pre>

    
Gets a bank account. The ID of the bank account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactBankId</td>
        <td>The ID of the bank account entry</td>
    </tr>
</table>


## Models<a name="account_contact_models"></a>
### Contact<a name="account_models_contact"></a>

The contact model.


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td>The external ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>number</td>
            <td>The number of the contact (previous customer number)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the contact type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>firstName</td>
            <td>The first name of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastName</td>
            <td>The last name of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fullName</td>
            <td>The full name of the contact. A concatenation of first and last name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td>The private email address of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>secondaryEmail</td>
            <td>The secondary private email address of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>gender</td>
            <td>The gender of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the contact, e.g. a doctorate</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>formOfAddress</td>
            <td>The form of address for the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>newsletterAllowanceAt</td>
            <td>The time the contact registered for the newsletter as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>classId</td>
            <td>The ID of the contact class</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blocked</td>
            <td>The blocked status of the contact. Contacts can be blocked for a specific client (store). Possible values:
<ul>
<li> 0 = not blocked</li>
<li> 1 = blocked</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rating</td>
            <td>The rating of the contact. This rating is for internal use only. 5 red stars are for the worst and 5 yellow stars for the best rating. Possible values:
<ul>
<li>-5 = 5 red stars (worst rating)</li>
<li>-4 = 4 red stars</li>
<li>-3 = 3 red stars</li>
<li>-2 = 2 red stars</li>
<li>-1 = 1 red star</li>
<li>0 = 5 grey stars, no rating saved for the contact</li>
<li>1 = 1 yellow star</li>
<li>2 = 2 yellow stars</li>
<li>3 = 3 yellow stars</li>
<li>4 = 4 yellow stars</li>
<li>5 = 5 yellow stars (best rating)</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bookAccount</td>
            <td>The book account (debtor account) of the contact. An additional, separate number that generally corresponds to the customer number or the debtor number in your financial accounting.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The origin of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The client (store) that is assigned to the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The owner ID of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>birthdayAt</td>
            <td>The date of birth of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastLoginAt</td>
            <td>The date of the last login of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastLoginAtTimestamp</td>
            <td>The date of the last login of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastOrderAt</td>
            <td>The date of the last order</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date the contact was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date the contact was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>privatePhone</td>
            <td>The private phone number of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>privateFax</td>
            <td>The private fax number of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>privateMobile</td>
            <td>The private mobile phone number of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ebayName</td>
            <td>The eBay account name of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paypalEmail</td>
            <td>The email address of the PayPal account of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paypalPayerId</td>
            <td>The PayPal payer id of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>klarnaPersonalId</td>
            <td>The Klarna personal id of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>dhlPostIdent</td>
            <td>The DHL PostIdent of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forumUsername</td>
            <td>The user name of the contact in the forum</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forumGroupId</td>
            <td>The ID of the forum group that is assigned to the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>singleAccess</td>
            <td>The access type of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contactPerson</td>
            <td>The contact person of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketplacePartner</td>
            <td>The marketplace partner status of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>addresses</td>
            <td>A collection of linked addresses</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>accounts</td>
            <td>A collection of linked accounts</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>orders</td>
            <td>A collection of orders of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>banks</td>
            <td>A collection of bank accounts of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>reorders</td>
            <td>A collection of reorders of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>orderSchedulers</td>
            <td>A collection of order schedulers of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>options</td>
            <td>A collection of options of the contact</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>allowedMethodsOfPayment</td>
            <td>A collection of allowed payment methods for the contact.*</td>
        </tr><tr>
            <td><a href="account#account_models_contacttype">ContactType</a>
</td>
            <td>type</td>
            <td>The type of the contact</td>
        </tr><tr>
            <td><a href="account#account_models_ordersummary">OrderSummary</a>
</td>
            <td>orderSummary</td>
            <td>The order summary of the contact</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactAllowedMethodOfPayment<a name="account_models_contactallowedmethodofpayment"></a>

The model of the allowed payment method for the contact


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the payment method allowed for the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>methodOfPaymentId</td>
            <td>The ID of the payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>allowed</td>
            <td>Allowed payment method for the contact. Possible values are:
<ul>
<li>0 = not allowed</li>
<li>1 = allowed</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>Timestamp when the payment method was created</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>Timestamp when the payment method was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPaymentActive</td>
            <td>Flag that indicates if the current payment method is active</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactBank<a name="account_models_contactbank"></a>

The contact bank model.


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the bank account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact the bank account belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order the bank account belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountOwner</td>
            <td>The owner of the bank account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bankName</td>
            <td>The name of the bank</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bankAddress</td>
            <td>The address of the bank</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bankPostalCodeTown</td>
            <td>The postcode and town of the bank</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bankCountry</td>
            <td>The country of the bank</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>iban</td>
            <td>The IBAN of the bank account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bic</td>
            <td>The BIC of the bank account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountNumber</td>
            <td>The account number of the bank account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sortCode</td>
            <td>The sort code of the bank account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateBy</td>
            <td>The source of the last change (possible values: `customer`, `backend`, `import`)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directDebitMandateAvailable</td>
            <td>Flag that indicates if a direct debit mandate is available</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>directDebitMandateAt</td>
            <td>The time the direct debit mandate was created as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>directDebitMethod</td>
            <td>The direct debit method (possible values: `sepaDirectDebit`, `sepaB2bDirectDebit`)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>directDebitType</td>
            <td>The direct debit type (possible values: `first`, `next`)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paymentMethod</td>
            <td>The payment method (possible values: `recurrent`, `onOff`)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the bank account was created as  unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the bank account was last updated as  unix timestamp</td>
        </tr><tr>
            <td><a href="account#account_models_contact">Contact</a>
</td>
            <td>contact</td>
            <td>The contact the bank account belongs to</td>
        </tr><tr>
            <td><a href="order#order_legacy_order">Order</a>
</td>
            <td>order</td>
            <td>The order the bank account belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactDepartment<a name="account_models_contactdepartment"></a>

contact department model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact department. It is possible to define individual departments. The following departments are available by default.
<ul>
<li>1 = Management</li>
<li>2 = Purchasing Department</li>
<li>3 = Sales Department</li>
<li>4 = Research & Development Team</li>
<li>5 = Production</li>
<li>6 = Quality Assurance</li>
<li>7 = Public Relations</li>
<li>8 = Marketing Department</li>
<li>9 = IT Department</li>
<li>10 = EDP Team</li>
<li>11 = Logistics</li>
<li>12 = Warehousing Department</li>
<li>13 = Export Department</li>
<li>14 = Import Department</li>
<li>15 = Customer Service</li>
<li>16 = Technical Support Team</li>
<li>17 = Human Resources</li>
<li>18 = Accounting Department</li>
<li>19 = Financial Department</li>
<li>20 = Legal Department</li>
<li>21 = Secretary's Office</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>List of contact department names</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactDepartmentName<a name="account_models_contactdepartmentname"></a>

contact department name model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact department name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>departmentId</td>
            <td>The ID of the department</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactOption<a name="account_models_contactoption"></a>

The contact options model.


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact the option belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type ID of the contact option. It is possible to define individual contact option types. The following types are available by default and cannot be deleted:
<ul>
<li>1 = Telephone</li>
<li>2 = Email</li>
<li>3 = Telefax</li>
<li>4 = Web page</li>
<li>5 = Marketplace</li>
<li>6 = Identification number</li>
<li>7 = Payment</li>
<li>8 = User name</li>
<li>9 = Group</li>
<li>10 = Access</li>
<li>11 = Additional</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>subTypeId</td>
            <td>The sub-type ID of the contact option. It is possible to define individual contact option sub-types. The following types are available by default and cannot be deleted:
<ul>
<li>1 = Work</li>
<li>2 = Mobile private</li>
<li>3 = Mobile work</li>
<li>4 = Private</li>
<li>5 = PayPal</li>
<li>6 = Ebay</li>
<li>7 = Amazon</li>
<li>8 = Klarna</li>
<li>9 = DHL</li>
<li>10 = Forum</li>
<li>11 = Guest</li>
<li>12 = Contact person</li>
<li>13 = Marketplace partner</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the option. Depends on the type/sub-type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priority</td>
            <td>The priority for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the option was created as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the option was last updated as unix timestamp</td>
        </tr><tr>
            <td><a href="account#account_models_contact">Contact</a>
</td>
            <td>contact</td>
            <td>The contact the option belongs to</td>
        </tr><tr>
            <td><a href="account#account_models_contactoptiontype">ContactOptionType</a>
</td>
            <td>type</td>
            <td>The type of the option</td>
        </tr><tr>
            <td><a href="account#account_models_contactoptionsubtype">ContactOptionSubType</a>
</td>
            <td>subType</td>
            <td>The sub-type of the option</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactOptionSubType<a name="account_models_contactoptionsubtype"></a>

contact options sub type model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact option sub-type. It is possible to define individual option sub-types. The following types are available by default and cannot be deleted.
<ul>
<li>1 = Work</li>
<li>2 = Mobile private</li>
<li>3 = Mobile work</li>
<li>4 = Private</li>
<li>5 = PayPal</li>
<li>6 = Ebay</li>
<li>7 = Amazon</li>
<li>8 = Klarna</li>
<li>9 = DHL</li>
<li>10 = Forum</li>
<li>11 = Guest</li>
<li>12 = Contact person</li>
<li>13 = Marketplace partner</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>nonErasable</td>
            <td>Flag that indicates if the option sub-type can be deleted</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>names</td>
            <td>A collection of names in different languages for the option sub-type.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactOptionSubTypeName<a name="account_models_contactoptionsubtypename"></a>

contact options sub type name model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact option sub type name entry</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>subTypeId</td>
            <td>The ID of the option sub-type the name entry belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>lang      The language of the sub-type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>name      The name of the sub-type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactOptionType<a name="account_models_contactoptiontype"></a>

contact options type model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact option type. It is possible to define individual option types. The following types are available by default and cannot be deleted.
<ul>
<li>1 = Telephone</li>
<li>2 = Email</li>
<li>3 = Telefax</li>
<li>4 = Web page</li>
<li>5 = Marketplace</li>
<li>6 = Identification number</li>
<li>7 = Payment</li>
<li>8 = User name</li>
<li>9 = Group</li>
<li>10 = Access</li>
<li>11 = Additional</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>nonErasable</td>
            <td>Flag that indicates if the option type can be deleted</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>names</td>
            <td>A collection of names in different languages for the option type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactOptionTypeName<a name="account_models_contactoptiontypename"></a>

The ContactOptionTypeName model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact option type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the option type the name belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the option type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the option type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactPosition<a name="account_models_contactposition"></a>

The ContactPosition model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact position. It is possible to define individual contact positions. The following positions are available by default:
<ul>
<li>1 = Analyst</li>
<li>2 = Director of Boards</li>
<li>3 = CEO</li>
<li>4 = Buyer</li>
<li>5 = Purchasing Manager</li>
<li>6 = CFO</li>
<li>7 = Director General</li>
<li>8 = Managing Director</li>
<li>9 = Codirector</li>
<li>10 = Commercial Agent</li>
<li>11 = Assistant</li>
<li>12 = Service Engineer</li>
<li>13 = Warehouse Manager</li>
<li>14 = Warehouse Worker</li>
<li>15 = Senior Executive</li>
<li>16 = Assistent</li>
<li>17 = Purchasing Assistent</li>
<li>18 = Software Developer</li>
<li>19 = Sales Representative</li>
<li>20 = Sales Manager</li>
<li>21 = Export Sales Manager</li>
<li>22 = Wholesale Distributing Manager</li>
<li>23 = Secretary</li>
<li>24 = Economist</li>
<li>25 = Management Board</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>The list of contact position names</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactPositionName<a name="account_models_contactpositionname"></a>

The ContactPositionName model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact position name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>positionId</td>
            <td>The ID of the position</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactType<a name="account_models_contacttype"></a>

The ContactType model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact type. It is possible to define individual contact types. The following types are available by default and cannot be deleted.
<ul>
<li>1 = Customer</li>
<li>2 = Sales lead/Interested party</li>
<li>3 = Sales representative</li>
<li>4 = Supplier</li>
<li>5 = Producer/Manufacturer</li>
<li>6 = Partner</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>nonErasable</td>
            <td>Flag that indicates if the type can be deleted</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>names</td>
            <td>A collection of contact type names in different languages</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>contacts</td>
            <td>A collection of contacts with the type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContactTypeName<a name="account_models_contacttypename"></a>

contact type name model


#### Namespace

`Plenty\Modules\Account\Contact\Models`


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
            <td>The ID of the contact type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The contact type ID. See also {@link ContactType::id}.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language ot the contact type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The contact type name</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Search<a name="account_search"></a>
    
## Contracts<a name="account_search_contracts"></a>
### ContactElasticSearchAvailibilityRepositoryContract<a name="account_contracts_contactelasticsearchavailibilityrepositorycontract"></a>

ContactElasticSearchAvailibilityRepositoryContract


#### Namespace

`Plenty\Modules\Account\Contact\Search\Contracts`



#### Methods

<pre>public <strong>isReady</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### ContactElasticSearchScrollRepositoryContract<a name="account_contracts_contactelasticsearchscrollrepositorycontract"></a>

kommt noch


#### Namespace

`Plenty\Modules\Account\Contact\Search\Contracts`



#### Methods

<pre>public <strong>hasNext</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setIndex</strong>(<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
 $index):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSearch</strong>(<a href="cloud#cloud_search_searchinterface">SearchInterface</a>
 $search):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_search_searchinterface">SearchInterface</a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### IndexContactRepositoryContract<a name="account_contracts_indexcontactrepositorycontract"></a>

The contract for the search repository


#### Namespace

`Plenty\Modules\Account\Contact\Search\Contracts`



#### Methods

<pre>public <strong>index</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Index a contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/array">array</a> $contactIds):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Delete contact from index
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$contactIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>bulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $contactIds):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$contactIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setOutput</strong>(<a href="cloud#cloud_output_outputinterface">OutputInterface</a>
 $output):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_output_outputinterface">OutputInterface</a>
</td>
        <td>$output</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>execute</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
# Account<a name="account_account"></a>
    
## Contracts<a name="account_account_contracts"></a>
### AccountRepositoryContract<a name="account_contracts_accountrepositorycontract"></a>

The AccountRepositoryContract is the interface for the account repository. This interface allows to list, get, create, update and delete accounts. An account contains company-related data. It is also possible to list all contacts of an account.


#### Namespace

`Plenty\Modules\Account\Contracts`



#### Methods

<pre>public <strong>createAccount</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_account">Account</a>
</pre>

    
Creates a new account and returns it.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The account data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateAccount</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="account#account_models_account">Account</a>
</pre>

    
Updates an existing account and returns it. The ID of the account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The account data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
</table>


<pre>public <strong>deleteAccount</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an account. The ID of the account must be specified. Returns `true` if deletion was successful. Returns `false` if deletion was not successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
</table>


<pre>public <strong>findAccountById</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="account#account_models_account">Account</a>
</pre>

    
Gets an account. The ID of the account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
</table>


<pre>public <strong>allAccounts</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Returns a collection of all accounts.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to retrieve (Default: '[*]').</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>Optional: The number of objects per page (Default: 50).</td>
    </tr>
</table>


<pre>public <strong>getContactsOfAccount</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Returns a collection of contacts that belong to the account.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the account</td>
    </tr>
</table>


<pre>public <strong>saveAccount</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Creates a new or updates an existing account.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The account data as associative array</td>
    </tr>
</table>


## Events<a name="account_account_events"></a>
### FrontendUpdateCustomerSettings<a name="account_events_frontendupdatecustomersettings"></a>

frontend customer settings event


#### Namespace

`Plenty\Modules\Account\Events`



#### Methods

<pre>public <strong>getDeliveryCountryId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setDeliveryCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $deliveryCountryId):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$deliveryCountryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getShowNetPrice</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setShowNetPrice</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $showNetPrice):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$showNetPrice</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getEbaySellerAccount</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setEbaySellerAccount</strong>(<a target="_blank" href="http://php.net/string">string</a> $ebaySellerAccount):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$ebaySellerAccount</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAccountContactSign</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setAccountContactSign</strong>(<a target="_blank" href="http://php.net/string">string</a> $accountContactSign):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$accountContactSign</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAccountContactClassId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setAccountContactClassId</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountContactClassId):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountContactClassId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSalesAgent</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setSalesAgent</strong>(<a target="_blank" href="http://php.net/string">string</a> $salesAgent):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$salesAgent</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAccountContractClassId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setAccountContractClassId</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountContractClassId):<a href="account#account_events_frontendupdatecustomersettings">FrontendUpdateCustomerSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountContractClassId</td>
        <td></td>
    </tr>
</table>


## Models<a name="account_account_models"></a>
### Account<a name="account_models_account"></a>

the account model.


#### Namespace

`Plenty\Modules\Account\Models`


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
            <td>The ID of the account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>number</td>
            <td>The number of the account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>companyName</td>
            <td>The company name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>taxIdNumber</td>
            <td>The ID of the tax number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>valuta</td>
            <td>The valuta date in days specified for the account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>discountDays</td>
            <td>The early payment discount period in days specified for the account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>discountPercent</td>
            <td>The early payment discount in percent specified for the account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>timeForPaymentAllowedDays</td>
            <td>The payment due date in days specified for the account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>salesRepresentativeContactId</td>
            <td>The contact ID of the sales representative</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the account owner</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deliveryTime</td>
            <td>The delivery time for the supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>dealerMinOrderValue</td>
            <td>The minimum order value for the supplier</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The time the account was created as unix timestamp</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The time the account was last updated as unix timestamp</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>contacts</td>
            <td>A list of contacts that belong to the account</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AccountContactRelation<a name="account_models_accountcontactrelation"></a>

account contact relation model


#### Namespace

`Plenty\Modules\Account\Models`


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
            <td>The ID of the account contact relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountId</td>
            <td>The ID of the foreign key account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the foreign key contact</td>
        </tr><tr>
            <td><a href="account#account_models_account">Account</a>
</td>
            <td>account</td>
            <td>The account of the relation</td>
        </tr><tr>
            <td><a href="account#account_models_contact">Contact</a>
</td>
            <td>contact</td>
            <td>The contact of the relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Newsletter<a name="account_newsletter"></a>
    
## Contracts<a name="account_newsletter_contracts"></a>
### NewsletterRepositoryContract<a name="account_contracts_newsletterrepositorycontract"></a>

The NewsletterRepositoryContract is the interface for the newsletter repository. This interface allows to assign email addresses of recipients to email folders. Depending on the settings selected for each email folder, different newsletters can be sent to different target groups.


#### Namespace

`Plenty\Modules\Account\Newsletter\Contracts`



#### Methods

<pre>public <strong>createEntry</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="account#account_models_entry">Entry</a>
</pre>

    
Creates an entry.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createRecipient</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Creates a recipient for an existing folder.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createFolder</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="account#account_models_folder">Folder</a>
</pre>

    
Creates a folder.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteAllEntries</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Delete all entries
    
<pre>public <strong>deleteAllFolders</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Delete all folders
    
<pre>public <strong>deleteAllRecipients</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Delete all recipients
    
<pre>public <strong>deleteEntryById</strong>(<a target="_blank" href="http://php.net/int">int</a> $entryId):<a href="account#account_models_entry">Entry</a>
</pre>

    
Deletes an entry. The ID of the entry must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$entryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteFolderById</strong>(<a target="_blank" href="http://php.net/int">int</a> $folderId):<a href="account#account_models_folder">Folder</a>
</pre>

    
Deletes a folder. The ID of the folder must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$folderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteRecipientById</strong>(<a target="_blank" href="http://php.net/int">int</a> $recipientId):<a href="account#account_models_recipient">Recipient</a>
</pre>

    
Deletes a recipient. The ID of the recipient must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$recipientId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listAllEntries</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all newsletter entries
    
<pre>public <strong>listAllFolders</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all newsletter folders
    
<pre>public <strong>listAllRecipients</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all recipients
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listEntryById</strong>(<a target="_blank" href="http://php.net/int">int</a> $entryId):<a href="account#account_models_entry">Entry</a>
</pre>

    
Shows details from entry
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$entryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listFolderById</strong>(<a target="_blank" href="http://php.net/int">int</a> $folderId):<a href="account#account_models_folder">Folder</a>
</pre>

    
Shows details from folder
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$folderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listRecipientById</strong>(<a target="_blank" href="http://php.net/int">int</a> $recipientId):<a href="account#account_models_recipient">Recipient</a>
</pre>

    
Shows details from recipient
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$recipientId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateEntryById</strong>(<a target="_blank" href="http://php.net/int">int</a> $entryId, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="account#account_models_entry">Entry</a>
</pre>

    
Updates an entry. The ID of the entry must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$entryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateFolderById</strong>(<a target="_blank" href="http://php.net/int">int</a> $folderId, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="account#account_models_folder">Folder</a>
</pre>

    
Updates a folder. The ID of the folder must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$folderId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateRecipientById</strong>(<a target="_blank" href="http://php.net/int">int</a> $recipientId, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="account#account_models_recipient">Recipient</a>
</pre>

    
Updates a recipient. The ID of the recipient must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$recipientId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addToNewsletterList</strong>(<a target="_blank" href="http://php.net/string">string</a> $email, <a target="_blank" href="http://php.net/string">string</a> $forename = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $surname = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $emailDirIds = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

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
    
Adds the email address of a contact or an interested party to an email folder for the newsletter list.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$email</td>
        <td>The email address of the contact or interested party who subscribed to the newsletter</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$forename</td>
        <td>The first name of the contact or interested party</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$surname</td>
        <td>The last name of the contact or interested party</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$emailDirIds</td>
        <td>The IDs of the email folders. The email addresses of the contacts and interested parties must be saved in the folders. This will allow to send different newsletters to different target groups.</td>
    </tr>
</table>


## Models<a name="account_newsletter_models"></a>
### Entry<a name="account_models_entry"></a>

The newsletter entry model.


#### Namespace

`Plenty\Modules\Account\Newsletter\Models`


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
            <td>subject</td>
            <td>The subject of the newsletter entry</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>body</td>
            <td>The body of the newsletter entry</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>kind</td>
            <td>The type of the newsletter entry</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>log</td>
            <td>The log of the newsletter entry</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Folder<a name="account_models_folder"></a>

The newsletter folder model.


#### Namespace

`Plenty\Modules\Account\Newsletter\Models`


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
            <td>The ID of the newsletter folder</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the newsletter folder</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isDeletable</td>
            <td>Flag that indicates if the newsletter folder can be deleted. The folders 'Customers' and 'Interested parties' are available by default and cannot be deleted.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the newsletter folder</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSelectable</td>
            <td>Flag that indicates if the newsletter folder can be selected by customers in the online store. If this is allowed, the folder will be displayed in the My account area of the online store. Customers will then be able to subscribe to the newsletters that are included in this folder.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### NewsletterEmail<a name="account_models_newsletteremail"></a>

NewsletterEmail


#### Namespace

`Plenty\Modules\Account\Newsletter\Models`


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
            <td>The ID of the newsletter email</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directory</td>
            <td>The ID of the directory</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forename</td>
            <td>The first name of the contact or interested party</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>surname</td>
            <td>The last name of the contact or interested party</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td>The email address The email address of the contact or interested party</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>gender</td>
            <td>The gender of the contact or interested party</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>birthday</td>
            <td>The birthday of the contact or interested party</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>timestamp</td>
            <td>The timestamp when the newsletter email was sent to the contact or interested party</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>templateLang</td>
            <td>The language of the newsletter's email template</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>confirmedTimestamp</td>
            <td>The timestamp when the contact or interested party confirmed the newsletter subscription</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>confirmAuthString</td>
            <td>The key that is automatically generated by the system. This key recognises the user regardless whether the user is logged in to the system and will then set the confirmation timestamp.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Recipient<a name="account_models_recipient"></a>

The newsletter recipient


#### Namespace

`Plenty\Modules\Account\Newsletter\Models`


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
            <td>The ID of the newsletter recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>folderId</td>
            <td>The ID of the newsletter folder</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>firstName</td>
            <td>The first name of the recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastName</td>
            <td>The last name of the recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td>The email address of the recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>gender</td>
            <td>The gender of the recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>birthday</td>
            <td>The birthday of the recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>timestamp</td>
            <td>The timestamp when the newsletter email was sent to the recipient</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>templateLang</td>
            <td>The language of the newsletter email template</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>confirmedTimestamp</td>
            <td>The timestamp when the recipient confirmed the newsletter subscription</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>confirmAuthString</td>
            <td>The key that is automatically generated by the system. This key recognises the user regardless whether the user is logged in to the system and will then set the confirmation timestamp.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# OrderSummary<a name="account_ordersummary"></a>
    
## Contracts<a name="account_ordersummary_contracts"></a>
### OrderSummaryRepositoryContract<a name="account_contracts_ordersummaryrepositorycontract"></a>

The OrderSummaryRepositoryContract is the interface for the order summary repository. This interface allows to list, get, update, create and delete order summaries.


#### Namespace

`Plenty\Modules\Account\OrderSummary\Contracts`



#### Methods

<pre>public <strong>findOrderSummaryById</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderSummaryId):<a href="account#account_models_ordersummary">OrderSummary</a>
</pre>

    
Gets an order summary. The ID of the order summary must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderSummaryId</td>
        <td>The ID of the order summary</td>
    </tr>
</table>


<pre>public <strong>updateOrderSummary</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderSummaryId):<a href="account#account_models_ordersummary">OrderSummary</a>
</pre>

    
Updates an order summary. The ID of the order summary must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order summary data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderSummaryId</td>
        <td>The ID of the order summary</td>
    </tr>
</table>


<pre>public <strong>createOrderSummary</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="account#account_models_ordersummary">OrderSummary</a>
</pre>

    
Creates an order summary.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order summary data as associative array</td>
    </tr>
</table>


<pre>public <strong>deleteOrderSummary</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderSummaryId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an order summary. The ID of the order summary must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderSummaryId</td>
        <td>The ID of the order summary</td>
    </tr>
</table>


<pre>public <strong>allOrderSummaries</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Returns a collection of all order summaries.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Optional: The columns to retrieve (Default: '[*]').</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>Optional: The number of objects per page (Default: 50).</td>
    </tr>
</table>


<pre>public <strong>findOrderSummaryByContactId</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="account#account_models_ordersummary">OrderSummary</a>
</pre>

    
Gets an order summary. The ID of the contact must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>findOrderSummaryByAddressId</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId):<a href="account#account_models_ordersummary">OrderSummary</a>
</pre>

    
Gets an order summary. The ID of the address must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
</table>


## Models<a name="account_ordersummary_models"></a>
### OrderSummary<a name="account_models_ordersummary"></a>

The order summary model.


#### Namespace

`Plenty\Modules\Account\OrderSummary\Models`


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
            <td>The ID of the order summary</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressId</td>
            <td>The address ID of the order summary</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unpaidOrdersCount</td>
            <td>The number of unpaid orders</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unpaidOrderTotalAmount</td>
            <td>The total amount of unpaid orders</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderCount</td>
            <td>The number of all orders of the associated model</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the order summary was created as unix timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the order summary was last updated as unix timestamp</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
