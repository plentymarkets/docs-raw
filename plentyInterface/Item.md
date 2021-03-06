

# Manufacturer<a name="item_manufacturer"></a>
    
## Contracts<a name="item_manufacturer_contracts"></a>
### ManufacturerCommissionRepositoryContract<a name="item_contracts_manufacturercommissionrepositorycontract"></a>

The contract for the manufacturer commission repository


#### Namespace

`Plenty\Modules\Item\Manufacturer\Contracts`





#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_manufacturercommission">ManufacturerCommission</a>
</pre>

    
Gets a manufacturer commission. The ID of the manufacturer commission must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the manufacturer</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_manufacturercommission">ManufacturerCommission</a>
</pre>

    
Creates a manufacturer commission.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The manufacturer commission data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_manufacturercommission">ManufacturerCommission</a>
</pre>

    
Updates a manufacturer commission. The ID of the manufacturer commission must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The manufacturer commission data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the manufacturer</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a manufacturer commission. The ID of the manufacturer commission must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the manufacturer</td>
    </tr>
</table>


<pre>public <strong>findByManufacturerId</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists manufacturer commissions. The ID of the manufacturer must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
</table>



### ManufacturerRepositoryContract<a name="item_contracts_manufacturerrepositorycontract"></a>

The contract for the manufacturer repository


#### Namespace

`Plenty\Modules\Item\Manufacturer\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_manufacturer">Manufacturer</a>
</pre>

    
Creates a manufacturer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The manufacturer data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="item#item_models_manufacturer">Manufacturer</a>
</pre>

    
Updates a manufacturer. The ID of the manufacturer must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The manufacturer data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a manufacturer. The ID of the manufacturer must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="item#item_models_manufacturer">Manufacturer</a>
</pre>

    
Gets a manufacturer. The ID of the manufacturer must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all manufacturers.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of manufacturers shown per page. Default value is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $params = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists manufacturers by filter
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>The filter array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
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
    

### ManufacturerExternalRepositoryContract<a name="item_contracts_manufacturerexternalrepositorycontract"></a>

The contract for the manufacturer external repository


#### Namespace

`Plenty\Modules\Item\Manufacturer\Contracts`





#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId, <a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="item#item_models_manufacturerexternal">ManufacturerExternal</a>
</pre>

    
Gets a manufacturer external. The ID of the manufacturer and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td>The ID of the market</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_manufacturerexternal">ManufacturerExternal</a>
</pre>

    
Creates a manufacturer external.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The manufacturer external data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $manufacturerId, <a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="item#item_models_manufacturerexternal">ManufacturerExternal</a>
</pre>

    
Updates a manufacturer external. The ID of the manufacturer and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The manufacturer external data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td>The ID of the market</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId, <a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a manufacturer external. The ID of the manufacturer and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td>The ID of the manufacturer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td>The ID of the market</td>
    </tr>
</table>


<pre>public <strong>search</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists manufacturer externals.
    
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
    
## Models<a name="item_manufacturer_models"></a>
### Manufacturer<a name="item_models_manufacturer"></a>

The item manufacturer model


#### Namespace

`Plenty\Modules\Item\Manufacturer\Models`




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
            <td>The unique ID of the manufacturer.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalName</td>
            <td>The external name of the manufacturer. The external name is used for the item export to external markets. If no external name is saved, the Name will be used. The external name will also be transferred to FINDOLOGIC and will be indexed for item searches.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>logo</td>
            <td>The URL of the manufacturer's logo</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>url</td>
            <td>The URL of the manufacturer's website</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>street</td>
            <td>The street of the manufacturer's address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>houseNo</td>
            <td>The house number of the manufacturer's address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>postcode</td>
            <td>The postal code of the manufacturer's address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>town</td>
            <td>The town of the manufacturer's address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>phoneNumber</td>
            <td>The phone number of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>faxNumber</td>
            <td>The fax number of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td>The email address of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The ID of the <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries" target="_blank">country</a> in which the manufacturer is based; 0 = unknown.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pixmaniaBrandId</td>
            <td>The manufacturer's ID on the market Pixmania</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannAtEpBrandId</td>
            <td>The manufacturer's ID on the market Neckermann Austria, Enterprise version</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>laRedouteBrandId</td>
            <td>The manufacturer's ID on the market La Redoute</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>comment</td>
            <td>Internal comments about the manufacturer (optional)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the manufacturer information was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>commissions</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>externals</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ManufacturerCommission<a name="item_models_manufacturercommission"></a>

The item manufacturer commission model


#### Namespace

`Plenty\Modules\Item\Manufacturer\Models`




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
            <td>The unique ID of the manufacturer commission</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>manufacturerId</td>
            <td>The unique ID of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The unique ID of the client (store) that the commission applies to. The route /rest/webstores provides access to clients (stores).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The unique ID of the referrer that the commission applies to. The route /rest/orders/referrers provides access to referrers.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>commission</td>
            <td>The manufacturer commission value in percent</td>
        </tr><tr>
            <td><a href="item#item_models_manufacturer">Manufacturer</a>
</td>
            <td>manufacturer</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ManufacturerExternal<a name="item_models_manufacturerexternal"></a>

The item manufacturer external model


#### Namespace

`Plenty\Modules\Item\Manufacturer\Models`




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
            <td>manufacturerId</td>
            <td>The unique ID of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketId</td>
            <td>The unique ID of the market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The external value</td>
        </tr><tr>
            <td><a href="item#item_models_manufacturer">Manufacturer</a>
</td>
            <td>manufacturer</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationStock<a name="item_variationstock"></a>
    
## Contracts<a name="item_variationstock_contracts"></a>
### VariationStockRepositoryContract<a name="item_contracts_variationstockrepositorycontract"></a>

The contract of the variation stock repository


#### Namespace

`Plenty\Modules\Item\VariationStock\Contracts`





#### Methods

<pre>public <strong>listStockByWarehouse</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List stock per warehouse
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The properties to be loaded</td>
    </tr>
</table>


<pre>public <strong>listStockMovements</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $columns, <a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List stock movements for a variation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The properties to be loaded</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The requested page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items per page</td>
    </tr>
</table>


<pre>public <strong>bookIncomingItems</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Book incoming stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>bookOutgoingItems</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Book outgoing stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>correctStock</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/bool">bool</a> $calcStockLater = false, <a target="_blank" href="http://php.net/bool">bool</a> $finishReceiptLater = false):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Correct stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$calcStockLater</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$finishReceiptLater</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>redistributeStock</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Redistribute stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>finishReceipt</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Finish receipt
    
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
    
## Models<a name="item_variationstock_models"></a>
### VariationStockMovement<a name="item_models_variationstockmovement"></a>

The variation stock movement model


#### Namespace

`Plenty\Modules\Item\VariationStock\Models`




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
            <td>The ID of the stock movement</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The ID of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>reasonString</td>
            <td>The reason string</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>attributeValues</td>
            <td>The attribute values of a variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>processRowId</td>
            <td>The ID is either the actual ID of an order or of an incoming item data set. Whether it is an order ID or an incoming item data set ID depends on the processRowType.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The quantity</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reason</td>
            <td>The reason for the movement</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The date and time that the movement was created. This date is in W3C format.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>processRowType</td>
            <td>The type of the stock movement
<ul>
	<li>1 = incoming item data set</li>
	<li>2 = order</li>
                                     <li>3 = deleted stock movement</li>
                                     <li>4 = new stock intake</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bestBeforeDate</td>
            <td>The best before date for the movement</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>batch</td>
            <td>The batch for the movement</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationName</td>
            <td>The name of the storage location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>warehouseName</td>
            <td>The name of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>purchasePrice</td>
            <td>The purchase price of a variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The id of the user. Can be null if the movement was not triggered by an user.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationStock<a name="item_models_variationstock"></a>

The variation stock model


#### Namespace

`Plenty\Modules\Item\VariationStock\Models`




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
            <td>itemId</td>
            <td>The ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The ID of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedListing</td>
            <td>The quantity of a variation that is reserved for listings</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedBundles</td>
            <td>The quantity of a variation that is reserved for item bundles</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>valueOfGoods</td>
            <td>The value of goods based on the physical stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td>The purchase price of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>physicalStock</td>
            <td>The physical stock of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedStock</td>
            <td>The reserved stock of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>netStock</td>
            <td>The net stock is the stock that can still be sold</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reorderLevel</td>
            <td>The quantity of a variation that triggers a reorder</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>deltaReorderLevel</td>
            <td>The quantity of a variation that is required to reach the reorder level</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Unit<a name="item_unit"></a>
    
## Contracts<a name="item_unit_contracts"></a>
### UnitNameRepositoryContract<a name="item_contracts_unitnamerepositorycontract"></a>

The contract for the unit name repository


#### Namespace

`Plenty\Modules\Item\Unit\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $unitId):<a href="item#item_models_unitname">UnitName</a>
</pre>

    
Creates a unit name. The ID of the unit must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The unit name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td>The ID of the unit</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $unitId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a unit name. The ID of the unit and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td>The ID of the unit</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the unit name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $unitId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_unitname">UnitName</a>
</pre>

    
Updates a unit name. The ID of the unit and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The unit name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td>The ID of the unit</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the unit name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $unitId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_unitname">UnitName</a>
</pre>

    
Gets a unit name. The ID of the unit and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td>The ID of the unit</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the unit name</td>
    </tr>
</table>


<pre>public <strong>findByUnitId</strong>(<a target="_blank" href="http://php.net/int">int</a> $unitId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists unit names. The ID of the unit must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td>The ID of the unit</td>
    </tr>
</table>



### UnitRepositoryContract<a name="item_contracts_unitrepositorycontract"></a>

The contract for the unit repository


#### Namespace

`Plenty\Modules\Item\Unit\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_unit">Unit</a>
</pre>

    
Creates a unit.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The unit data as an associative array</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_unit">Unit</a>
</pre>

    
Gets a unit. The ID of the unit must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the unit</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_unit">Unit</a>
</pre>

    
Updates a unit. The ID of the unit must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The unit data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the unit</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a unit. The ID of the unit must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the unit</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_unit">Unit</a>
</pre>

    
Gets a unit. The ID of the unit must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the unit</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all units.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of units shown per page. Default value is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
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
    
## Models<a name="item_unit_models"></a>
### Unit<a name="item_models_unit"></a>

The unit model including the unit name


#### Namespace

`Plenty\Modules\Item\Unit\Models`




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
            <td>The unique ID of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>unitOfMeasurement</td>
            <td>The International System of Units (ISO) <a href="https://developers.plentymarkets.com/rest-doc/introduction#units"  target="_blank">code</a> of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isDecimalPlacesAllowed</td>
            <td>Flag that indicates if decimal places are allowed for this unit of measurement. If false, only integer values are allowed for the unit.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the unit was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the unit was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### UnitName<a name="item_models_unitname"></a>

The unit name model including the unit


#### Namespace

`Plenty\Modules\Item\Unit\Models`




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
            <td>unitId</td>
            <td>The unique ID of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages"  target="_blank">language</a> of the unit name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the unit</td>
        </tr><tr>
            <td><a href="item#item_models_unit">Unit</a>
</td>
            <td>unit</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationWarehouse<a name="item_variationwarehouse"></a>
    
## Contracts<a name="item_variationwarehouse_contracts"></a>
### VariationWarehouseRepositoryContract<a name="item_contracts_variationwarehouserepositorycontract"></a>

The contract for the variation warehouse repository


#### Namespace

`Plenty\Modules\Item\VariationWarehouse\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $warehouseId):<a href="item#item_models_variationwarehouse">VariationWarehouse</a>
</pre>

    
Gets the data of a warehouse linked to a variation. The ID of the variation and the ID of the warehouse must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The unique ID of the warehouse</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationwarehouse">VariationWarehouse</a>
</pre>

    
Creates a link between a warehouse and a variation and adds warehouse data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation warehouse data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $warehouseId):<a href="item#item_models_variationwarehouse">VariationWarehouse</a>
</pre>

    
Updates the data of a warehouse linked to a variation. The ID of the variation and the ID of the warehouse must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation warehouse data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The unique ID of the warehouse</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $warehouseId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the link between a warehouse and a variation. The ID of the variation and the ID of the warehouse must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The unique ID of the warehouse</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all warehouse data of a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all warehouse data of a variation with inheritance details. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationwarehouse_models"></a>
### VariationWarehouse<a name="item_models_variationwarehouse"></a>

Variation Warehouse


#### Namespace

`Plenty\Modules\Item\VariationWarehouse\Models`




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
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The unique ID of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseZoneId</td>
            <td>The unique ID of the warehouse zone</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationType</td>
            <td>The storage location type of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reorderLevel</td>
            <td>The reorder level for the variation in this warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maximumStock</td>
            <td>The maximum stock for the variation in this warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockTurnoverInDays</td>
            <td>The stock turnover in days for the variation in this warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storageLocation</td>
            <td>The storage location of the variation in this warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockBuffer</td>
            <td>The stock buffer for the variation in this warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isBatch</td>
            <td>Is for warehouse and variation stock batch active</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isBestBeforeDate</td>
            <td>Is for warehouse and variation stock best before date active</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td>The time the warehouse data was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the warehouse data was created.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationDefaultCategory<a name="item_variationdefaultcategory"></a>
    
## Contracts<a name="item_variationdefaultcategory_contracts"></a>
### VariationDefaultCategoryRepositoryContract<a name="item_contracts_variationdefaultcategoryrepositorycontract"></a>

The contract of the variation default category repository


#### Namespace

`Plenty\Modules\Item\VariationDefaultCategory\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationdefaultcategory">VariationDefaultCategory</a>
</pre>

    
Gets the default category of a variation for the client (store) specified. The ID of the variation and the plenty ID of the client (store) must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The unique plenty ID of the client (store)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationdefaultcategory">VariationDefaultCategory</a>
</pre>

    
Creates a link between a variation and a category that designates the category as the default category for this client (store).
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation default category data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationdefaultcategory">VariationDefaultCategory</a>
</pre>

    
Updates the default category linked to a variation. The ID of the variation and the plenty ID of the client (store) must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation default category data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The unique plenty ID of the client (store)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the link between a variation and a default category. The ID of the variation and the plenty ID of the client (store) must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The unique plenty ID of the client (store)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationdefaultcategory">VariationDefaultCategory</a>
</pre>

    
Lists the default categories of a variation for all clients (stores). The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationdefaultcategory_models"></a>
### VariationDefaultCategory<a name="item_models_variationdefaultcategory"></a>

Variation Default Category


#### Namespace

`Plenty\Modules\Item\VariationDefaultCategory\Models`




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
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>branchId</td>
            <td>The unique ID of the category branch</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The unique plenty ID of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>manually</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ItemCrossSelling<a name="item_itemcrossselling"></a>
    
## Contracts<a name="item_itemcrossselling_contracts"></a>
### ItemCrossSellingRepositoryContract<a name="item_contracts_itemcrosssellingrepositorycontract"></a>

Repository for item cross-selling


#### Namespace

`Plenty\Modules\Item\ItemCrossSelling\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemcrossselling">ItemCrossSelling</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="item#item_models_itemcrossselling">ItemCrossSelling</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $crossItemId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$crossItemId</td>
        <td>The unique ID of the linked cross-selling item</td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
</table>


<pre>public <strong>findAllByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all cross-selling links where the given item ID occurs
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
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
    

### DynamicItemCrossSellingRepositoryContract<a name="item_contracts_dynamicitemcrosssellingrepositorycontract"></a>

Repository for dynamic item cross-selling


#### Namespace

`Plenty\Modules\Item\ItemCrossSelling\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_dynamicitemcrossselling">DynamicItemCrossSelling</a>
</pre>

    
Create a new dynamic cross-selling link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $crossItemId):<a href="item#item_models_dynamicitemcrossselling">DynamicItemCrossSelling</a>
</pre>

    
Get one dynamic cross-selling link of an item by item ID and cross-selling item ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$crossItemId</td>
        <td>The unique ID of the linked cross-selling item</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $crossItemId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete a dynamic cross-selling link. The ID of the item and the ID of the cross-selling item must be specified. An exception is thrown if at least one relation exists.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$crossItemId</td>
        <td>The unique ID of the linked cross-selling item</td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List dynamic cross-selling links by item ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
</table>


<pre>public <strong>findAllByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all dynamic cross-selling links where the given item ID occurs
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
</table>


## Models<a name="item_itemcrossselling_models"></a>
### DynamicItemCrossSelling<a name="item_models_dynamicitemcrossselling"></a>

The item dynamic cross-selling model including the item


#### Namespace

`Plenty\Modules\Item\ItemCrossSelling\Models`




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
            <td>itemId</td>
            <td>The unique ID of the item to which cross-selling items are linked</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>crossItemId</td>
            <td>The unique ID of the cross-selling item that is linked to the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>count</td>
            <td>The count</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lastUpdate</td>
            <td>Last update integer</td>
        </tr><tr>
            <td><a href="item#item_models_item">Item</a>
</td>
            <td>item</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemCrossSelling<a name="item_models_itemcrossselling"></a>

The item cross-selling model including the item


#### Namespace

`Plenty\Modules\Item\ItemCrossSelling\Models`




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
            <td>itemId</td>
            <td>The unique ID of the item to which cross-selling items are linked</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>crossItemId</td>
            <td>The unique ID of the cross-selling item that is linked to the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relationship</td>
            <td>The cross-selling relationship between item and cross-selling item. Possible values:<ul><li>Accessory = The cross-selling item is an accessory of the item.</li><li>ReplacementPart = The cross-selling item is a replacement part for the item.</li><li>Similar = The cross-selling item is similar to the item.</li><li>Bundle = The cross-selling item is suitable to be sold as a bundle with the item.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isDynamic</td>
            <td>Flag that indicates if the cross-selling link was generated automatically.</td>
        </tr><tr>
            <td><a href="item#item_models_item">Item</a>
</td>
            <td>item</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Attribute<a name="item_attribute"></a>
    
## Contracts<a name="item_attribute_contracts"></a>
### AttributeMapRepositoryContract<a name="item_contracts_attributemaprepositorycontract"></a>

The contract for the attribute map repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attributemap">AttributeMap</a>
</pre>

    
Creates a new attribute map.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="item#item_models_attributemap">AttributeMap</a>
</pre>

    
Gets an attribute map. The ID of the attribute and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all attribute maps.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="item#item_models_attributemap">AttributeMap</a>
</pre>

    
Updates an attribute map. The ID of the attribute and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute map. The ID of the attribute and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### AttributeValueRepositoryContract<a name="item_contracts_attributevaluerepositorycontract"></a>

The contract for the attribute value repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="item#item_models_attributevalue">AttributeValue</a>
</pre>

    
Creates an attribute value. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attributevalue">AttributeValue</a>
</pre>

    
Updates an attribute value. The ID of the attribute and the ID of the value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the value</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute value. The ID of the attribute and the ID of the value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the value</td>
    </tr>
</table>


<pre>public <strong>findByAttributeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists attribute values. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of attribute values shown per page. Default value is 50</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="item#item_models_attributevalue">AttributeValue</a>
</pre>

    
Gets a attribute value. The ID of the attribute and the ID of the value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>An array of the with params</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevalue">AttributeValue</a>
</pre>

    
Gets a attribute value. The ID of the value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all attribute values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of attribute values shown per page. Default value is 50.</td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### AttributeEbayCorrelationRepositoryContract<a name="item_contracts_attributeebaycorrelationrepositorycontract"></a>

The contract for the attribute ebay correlation repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attributeebaycorrelation">AttributeEbayCorrelation</a>
</pre>

    
Creates new ebay attribute correlation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="item#item_models_attributeebaycorrelation">AttributeEbayCorrelation</a>
</pre>

    
Gets an ebay attribute correlation. The ID of the attribute correlation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the ebay attribute correlation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attributeebaycorrelation">AttributeEbayCorrelation</a>
</pre>

    
Updates an ebay attribute correlation. The ID of the attribute correlation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the ebay attribute correlation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an ebay attribute correlation. The ID of the attribute correlation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the ebay attribute correlation</td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attributeebaycorrelation">AttributeEbayCorrelation</a>
</pre>

    
Gets an ebay attribute correlation. The ID of the attribute correlation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the ebay attribute correlation</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $perPage, <a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/array">array</a> $filters):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists ebay attribute correlations by filters.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### AttributeNameRepositoryContract<a name="item_contracts_attributenamerepositorycontract"></a>

The contract for the attribute name repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="item#item_models_attributename">AttributeName</a>
</pre>

    
Creates an attribute name. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute name data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute ID</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute name. The ID of the attribute and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributename">AttributeName</a>
</pre>

    
Updates an attribute name. The ID of the attribute and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute name data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributename">AttributeName</a>
</pre>

    
Gets an attribute name. The ID of the attribute and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute name</td>
    </tr>
</table>


<pre>public <strong>findByAttributeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="item#item_models_attributename">AttributeName</a>
</pre>

    
Lists attribute names. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td>The ID of the attribute</td>
    </tr>
</table>



### AttributeValueMarketNameRepositoryContract<a name="item_contracts_attributevaluemarketnamerepositorycontract"></a>

The contract for the attribute value market name repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attributevaluemarketname">AttributeValueMarketName</a>
</pre>

    
Creates an attribute value market name. The ID of the attribute value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value market name data as associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $referenceType):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute value market name. The ID of the attribute value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The referenceType of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $referenceType):<a href="item#item_models_attributevaluemarketname">AttributeValueMarketName</a>
</pre>

    
Updates an attribute value market name. The ID of the attribute value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value market name data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value market name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The referenceType of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $referenceType):<a href="item#item_models_attributevaluemarketname">AttributeValueMarketName</a>
</pre>

    
Gets an attribute value market name. The ID of the attribute value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The referenceType of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>findByAttributeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists attribute value market names. The ID of the attribute and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Search attribute value market names.
    
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
    

### AttributeValueSetRepositoryContract<a name="item_contracts_attributevaluesetrepositorycontract"></a>

The contract for the attribute value set repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
List attribute value sets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
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
    

### AttributeValueNameRepositoryContract<a name="item_contracts_attributevaluenamerepositorycontract"></a>

The contract for the attribute value name repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>

    
Creates an attribute value name. The ID of the attribute value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value name data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute value name. The ID of the attribute value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>

    
Updates an attribute value name. The ID of the attribute value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value name data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>

    
Gets an attribute value name. The ID of the attribute value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the attribute value name</td>
    </tr>
</table>


<pre>public <strong>findByValueId</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>

    
Lists attribute value names. The ID of the attribute value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
</table>



### AttributeValueMapRepositoryContract<a name="item_contracts_attributevaluemaprepositorycontract"></a>

The contract for the attribute value map repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attributevaluemap">AttributeValueMap</a>
</pre>

    
Creates a new attribute value map.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $attributeValueId, <a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="item#item_models_attributevaluemap">AttributeValueMap</a>
</pre>

    
Gets an attribute value map. The ID of the attribute, the ID of the attribute value and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeValueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all attribute value maps.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $attributeValueId, <a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="item#item_models_attributevaluemap">AttributeValueMap</a>
</pre>

    
Updates an attribute value map. The ID of the attribute, the ID of the attribute value and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeValueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $attributeValueId, <a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute value map. The ID of the attribute, the ID of the attribute value and the ID of the market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeValueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### AttributeValueImageRepositoryContract<a name="item_contracts_attributevalueimagerepositorycontract"></a>

The contract for the attribute value image repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>getAttributeValueImage</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevalueimage">AttributeValueImage</a>
</pre>

    
Get an attribute value image link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item ID</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The unique ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The unique ID of the attribute value</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attributevalueimage">AttributeValueImage</a>
</pre>

    
Create an attribute value image link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value image data as an associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete an attribute value image link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The ID of the attribute value</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevalueimage">AttributeValueImage</a>
</pre>

    
Updates an attribute value image link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute value image data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The unique ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The unique ID of the attribute value</td>
    </tr>
</table>


<pre>public <strong>search</strong>():<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
List attribute value image links
    
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
    

### AttributeRepositoryContract<a name="item_contracts_attributerepositorycontract"></a>

The contract for the attribute repository


#### Namespace

`Plenty\Modules\Item\Attribute\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attribute">Attribute</a>
</pre>

    
Creates new attribute
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute data as associative array</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="item#item_models_attribute">Attribute</a>
</pre>

    
Gets an attribute. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the attribute</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>An array of the with params</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attribute">Attribute</a>
</pre>

    
Updates an attribute. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The attribute data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the attribute</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an attribute. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the attribute</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attribute">Attribute</a>
</pre>

    
Gets an attribute. The ID of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the attribute</td>
    </tr>
</table>


<pre>public <strong>findByBackendName</strong>(<a target="_blank" href="http://php.net/string">string</a> $backendName):<a href="item#item_models_attribute">Attribute</a>
</pre>

    
Gets an attribute. The backend name of the attribute must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$backendName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all attributes.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The attributes shown per page. Default value is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
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
    
## Models<a name="item_attribute_models"></a>
### AttributeValueMarketName<a name="item_models_attributevaluemarketname"></a>

The AttributeValueMarketName model including AttributeValue


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>valueId</td>
            <td>The unique ID of the attribute value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries" target="_blank">language</a> of the attribute value market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute value market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceType</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_attributevalue">AttributeValue</a>
</td>
            <td>attributeValue</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeValueImage<a name="item_models_attributevalueimage"></a>

The AttributeValueImage model


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>imageId</td>
            <td>The unique ID of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The unique ID of the attribute</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>valueId</td>
            <td>The unique ID of the attribute value</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeValue<a name="item_models_attributevalue"></a>

The AttributeValue model including Attribute and AttributeValueName


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>The unique ID of the attribute value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The unique ID of the attribute associated with the attribute value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The back end name of the attribute value. This name can only be assigned once per attribute. It is not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the attribute value. Attribute values are sorted in ascending order by position.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>image</td>
            <td>The name of the image associated with the attribute value; naming pattern is attr\_\{valueId\}.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>comment</td>
            <td>Optional comment on the attribute value. Comments are not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazonValue</td>
            <td>The attribute value of the market Amazon that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the values specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ottoValue</td>
            <td>The attribute value of the market OTTO that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the attribute values specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>neckermannAtEpValue</td>
            <td>The attribute value of the market Neckermann AT EP that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the attribute values specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>laRedouteValue</td>
            <td>The attribute value of the market La Redoute that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the attribute values specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tracdelightValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>percentageDistribution</td>
            <td>The percentage for automatic stock distribution of attribute values. When reordering an item, the quantities of attribute values is automatically distributed among the total quantity.</td>
        </tr><tr>
            <td><a href="item#item_models_attribute">Attribute</a>
</td>
            <td>attribute</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>valueNames</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>valueMarketNames</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>valueMaps</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeEbayCorrelation<a name="item_models_attributeebaycorrelation"></a>

The AttributeEbayCorrelation model


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>The unique ID of the ebay attribute correlation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The ID of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebaySiteId</td>
            <td>The ID of the ebay site the attribute correlation is for.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategoryId</td>
            <td>The ID of the ebay category of an ebay site the attribute correlation is for.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ebayAttributeName</td>
            <td>The attribute of the market eBay that this attribute is linked to. Attributes can be linked to a ebay property or can have a separate correlation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>useForPictures</td>
            <td>Flag that indicates if the ebay attribute correlation is used for pictures.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeMap<a name="item_models_attributemap"></a>

The AttributeMap model


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td>The unique ID of the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The unique ID of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute map. The name must be unique and must not contain commas, colons, semicolons or quotation marks. It is not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketInformation1</td>
            <td>The information regarding the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketInformation2</td>
            <td>The information regarding the marketplace.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeValueMap<a name="item_models_attributevaluemap"></a>

The AttributeValueMap model


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td>The unique ID of the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The unique ID of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueId</td>
            <td>The unique ID of the attribute value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute value map. The name must be unique and must not contain commas, colons, semicolons or quotation marks. It is not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketInformation1</td>
            <td>The information regarding the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketInformation2</td>
            <td>The information regarding the marketplace.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeValueName<a name="item_models_attributevaluename"></a>

The AttributeValueName model including AttributeValue


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>valueId</td>
            <td>The unique ID of the attribute value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries" target="_blank">language</a> of the attribute value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute value. This attribute value name is displayed in the online store.</td>
        </tr><tr>
            <td><a href="item#item_models_attributevalue">AttributeValue</a>
</td>
            <td>attributeValue</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Attribute<a name="item_models_attribute"></a>

The Attribute model including AttributeName and AttributeValue


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>The unique ID of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The back end name of the attribute. The name must be unique and must not contain commas, colons, semicolons or quotation marks. It is not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the attribute. Attributes are displayed in the attribute overview in ascending order by position.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSurchargePercental</td>
            <td>Flag that indicates if the surcharge is percental.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isLinkableToImage</td>
            <td>Flag that indicates if an image can be linked to the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazonAttribute</td>
            <td>The attribute of the market Amazon that this attribute is liked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fruugoAttribute</td>
            <td>The attribute of the market Fruugo that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pixmaniaAttribute</td>
            <td>The attribute of the market PIXmania that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ottoAttribute</td>
            <td>The attribute of the market OTTO that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>googleShoppingAttribute</td>
            <td>The attribute of the market Google Shopping that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannAtEpAttribute</td>
            <td>The component of the market neckermann AT EP that this attribute is linked to. To list variations on this market, attributes must be linked to one of the components specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>typeOfSelectionInOnlineStore</td>
            <td>How customers can select the attribute in the front end of a client. To allow attribute selection by check mark, attribute availability must be checked on the client side.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>laRedouteAttribute</td>
            <td>The attribute of the market La Redoute that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isGroupable</td>
            <td>Flag that indicates if the attribute can be grouped in item lists. If yes, variations with this attribute can be shown in the ItemViewCategoriesList template first. Other attributes are nested and can only be selected after this attribute has been selected.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attributeNames</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>values</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>maps</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeValueSet<a name="item_models_attributevalueset"></a>

The AttributeValueSet model


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>attributeValueSetId</td>
            <td>The ID of the attribute value set</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The ID of the attribute</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>valueId</td>
            <td>The ID of the attribute value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isLinkableToImage</td>
            <td>Flag that indicates if an image can be linked to the attribute.</td>
        </tr><tr>
            <td><a href="item#item_models_attributevalue">AttributeValue</a>
</td>
            <td>attributeValue</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_attribute">Attribute</a>
</td>
            <td>attribute</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeValueSetId<a name="item_models_attributevaluesetid"></a>

The AttributeValueSetId model


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>The ID of the attribute value set id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>hash</td>
            <td>a hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazon_variation_set</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>size</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AttributeName<a name="item_models_attributename"></a>

The AttributeName model including Attribute


#### Namespace

`Plenty\Modules\Item\Attribute\Models`




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
            <td>attributeId</td>
            <td>The id of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries" target="_blank">language</a> of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute. This attribute name is displayed in the online store.</td>
        </tr><tr>
            <td><a href="item#item_models_attribute">Attribute</a>
</td>
            <td>attribute</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Variation<a name="item_variation"></a>
    
## Contracts<a name="item_variation_contracts"></a>
### VariationImageServiceContract<a name="item_contracts_variationimageservicecontract"></a>

Preload all variations linked to an image for several item IDs


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>preload</strong>(<a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getData</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $imageId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAll</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### VariationInheritanceServiceContract<a name="item_contracts_variationinheritanceservicecontract"></a>

To be written...


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>activate</strong>(<a href="item#item_models_variation">Variation</a>
 $variation, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_variation">Variation</a>
</td>
        <td>$variation</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deactivate</strong>(<a href="item#item_models_variation">Variation</a>
 $variation, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_variation">Variation</a>
</td>
        <td>$variation</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>



### VariationRepositoryContract<a name="item_contracts_variationrepositorycontract"></a>

The contract for the variation repository


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $with, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_variation">Variation</a>
</pre>

    
Gets a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variation">Variation</a>
</pre>

    
Creates a variation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation data as an associative array</td>
    </tr>
</table>


<pre>public <strong>createPrimary</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variation">Variation</a>
</pre>

    
Creates a primary variation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation data as an associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variation">Variation</a>
</pre>

    
Get a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variation">Variation</a>
</pre>

    
Update a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Updates up to 50 variations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>changePrimaryVariation</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variation">Variation</a>
</pre>

    
Change main variation. Changes the variation with the specified variation ID to the new main variation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>patchBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $rows):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$rows</td>
        <td></td>
    </tr>
</table>



### VariationMultiPackServiceContract<a name="item_contracts_variationmultipackservicecontract"></a>

The contract for the variation bundle service


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>createMultiPackBundle</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $componentId, <a target="_blank" href="http://php.net/int">int</a> $quantity):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$componentId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$quantity</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setMainVariationBundleItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateMultiPackBundle</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $quantityId, <a target="_blank" href="http://php.net/int">int</a> $quantity):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$quantityId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$quantity</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeValueSetId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>matchUnit</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isMultiPack</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>



### VariationExportServiceContract<a name="item_contracts_variationexportservicecontract"></a>

Enhances the loading speed.


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>addPreloadTypes</strong>(<a target="_blank" href="http://php.net/array">array</a> $types):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$types</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>preload</strong>(<a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/array">array</a> $parameters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getData</strong>(<a target="_blank" href="http://php.net/string">string</a> $dataType, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$dataType</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAll</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>



### VariationLookupRepositoryContract<a name="item_contracts_variationlookuprepositorycontract"></a>

lookup repository for variations


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>hasBarcode</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, <a target="_blank" href="http://php.net/int">int</a> $barcodeId = null):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasId</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasExternalId</strong>(<a target="_blank" href="http://php.net/string">string</a> $externalId):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$externalId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasNumber</strong>(<a target="_blank" href="http://php.net/string">string</a> $number):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$number</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasSupplierItemNumber</strong>(<a target="_blank" href="http://php.net/string">string</a> $supplierVariationNumber):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$supplierVariationNumber</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAttributeValueMap</strong>(<a target="_blank" href="http://php.net/array">array</a> $attributeValueMap):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeValueMap</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>limit</strong>(<a target="_blank" href="http://php.net/int">int</a> $limit):<a href="item#item_contracts_variationlookuprepositorycontract">VariationLookupRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$limit</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>lookup</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### VariationSearchRepositoryContract<a name="item_contracts_variationsearchrepositorycontract"></a>

A repository for comfortable searches for variations


#### Namespace

`Plenty\Modules\Item\Variation\Contracts`





#### Methods

<pre>public <strong>setSearchFilter</strong>(<a target="_blank" href="http://php.net/int">int</a> $name, <a target="_blank" href="http://php.net/array">array</a> $params):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSearchParam</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSearchParams</strong>(<a target="_blank" href="http://php.net/array">array</a> $params):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>search</strong>():<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    

    
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
    
## Models<a name="item_variation_models"></a>
### Variation<a name="item_models_variation"></a>

Variation


#### Namespace

`Plenty\Modules\Item\Variation\Models`




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
            <td>The ID of the variation. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isMain</td>
            <td>Flag that indicates if the variation is the main variation of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainVariationId</td>
            <td>The variation ID of the item's main variation. Value is NULL if this variation is the item's main variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The item ID of the item that this variation belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the variation. Value is inherited from the item's main variation if inheritance is active.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isActive</td>
            <td>Flag that indicates if the variation is active. Only active variations can be offered in the online store and/or on markets.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>number</td>
            <td>The unique variation number of the variation. The variation number must be specified.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>model</td>
            <td>The model of the variation. Value is inherited from the item's main variation if inheritance is active.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td>The external variation ID of this variation. The external variation number is optional and allows importing items and variations from external systems to plentymarkets.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>availability</td>
            <td>The availability of the variation. Possible values: 1 to 10, null = Variation inherits value of main variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>estimatedAvailableAt</td>
            <td>The estimated delivery date of variations on reorder.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td>The net purchase price. Value e.g. is used for price calculations.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>movingAveragePrice</td>
            <td>The moving average purchase price of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the variation was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the variation was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relatedUpdatedAt</td>
            <td>The time at which related information for this variation was last updated. Related information is defined as information that is linked to the variation, i.e. barcodes, categories, images, markets, clients (stores), prices, suppliers, warehouses and the default category.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>availabilityUpdatedAt</td>
            <td>The time at which the availability of this variation was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceCalculationId</td>
            <td>The ID of the price calculation linked to the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>picking</td>
            <td>The order picking type of the variation. Possible values: single_picking, no_single_picking, exclude_from_picklist, null (no order picking type)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockLimitation</td>
            <td>The stock limitation for the variation. Possible values: <ul><li>0 = No limitation, i.e. stock is not limited. The variations's availability is not checked automatically.</li><li>1 = Stock is limited to net stock. The variation's availability is checked automatically.</li><li>2 = Do not administer stock for this variation.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisibleIfNetStockIsPositive</td>
            <td>Flag that indicates if the variation is visible in the online store if net stock is positive. If true, the variation automatically becomes visible when the net stock changes to positive.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isInvisibleIfNetStockIsNotPositive</td>
            <td>Flag that indicates if the variation is invisible in the online store if net stock is not positive. If true, the variation automatically becomes invisible when the net stock changes to 0 or negative.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isAvailableIfNetStockIsPositive</td>
            <td>Flag that indicates if the variation is available in the online store if net stock is positive. If true, the variation automatically becomes available when the net stock changes to positive.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isUnavailableIfNetStockIsNotPositive</td>
            <td>Flag that indicates if the variation is unavailable in the online store if net stock is not positive. If true, the variation automatically becomes available when the net stock changes to 0 or negative.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisibleInListIfNetStockIsPositive</td>
            <td>Flag that indicates if the variation is visible in the item list of the online store if net stock is positive. If true, the variation automatically becomes visible in categories, search results and item lists (store specials, cross-selling, last seen items) when the net stock changes to positive.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isInvisibleInListIfNetStockIsNotPositive</td>
            <td>Flag that indicates if the variation is invisible in the item list of the online store if net stock is not positive. If true and no net stock is available for the variation, the variation can only be opened using the direct URL. The variation is not shown in the categories, search results or item lists (store specials, cross-selling, last seen items).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainWarehouseId</td>
            <td>The ID of the main warehouse of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>maximumOrderQuantity</td>
            <td>The maximum order quantity permitted per order. Decimal values are possible to allow orders by weight or length. Default value is 0. If value is 0, the maximum order quantity is unlimited.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minimumOrderQuantity</td>
            <td>The minimum order quantity. Decimal values are possible to allow orders by weight or length.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>intervalOrderQuantity</td>
            <td>The quantity intervals the variation can be ordered in. Decimal values are possible to allow orders by weight or length.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>availableUntil</td>
            <td>The last date the item will be available for sale.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>releasedAt</td>
            <td>The release date of the variation. This is the date on which the variation will become available. The variation can be visible in the online store before this date, e.g. for preorders.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitCombinationId</td>
            <td>The unit combination id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightG</td>
            <td>The gross weight of the variation in gramms (g). This weight includes the packaging for variations that are packaged separately. This value is used for calculating shipping packages and weight-based shipping costs.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightNetG</td>
            <td>The net weight of the variation in gramms (g). This is the weight of the variation without packaging.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>widthMM</td>
            <td>The width of the variation in millimetres (mm)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lengthMM</td>
            <td>The length of the variation in millimeters (mm)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>heightMM</td>
            <td>The height of the variation in millimetres (mm)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge1</td>
            <td>The extra shipping charge 1 for the variation. Extra shipping charges are useful for large or bulky items that are particularly expensive to ship. Charge 1 is added to the regular shipping costs for the first item of an order. If different variations are ordered, the extra shipping charge 1 of the variation with the highest charge 1 is selected.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge2</td>
            <td>The extra shipping charge 2 for the variation. Extra shipping charges are useful for large or bulky items that are expensive to ship. Charge 2 is added to the shipping costs for any additional items of an order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitsContained</td>
            <td>The number of sales units contained in one package. Default value is 1.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>palletTypeId</td>
            <td>The ID of the pallet type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnits</td>
            <td>The number of packing units if the item consists of multiple packages. Value is 0 if an item is sent as one package. All items of an order that have the value 0 will be packed into one package.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnitTypeId</td>
            <td>The ID of the packing unit type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>transportationCosts</td>
            <td>The net transportation costs for the variation. This value is used for price calculations and for calculating the acquisition price.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>storageCosts</td>
            <td>The net storage costs for the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customs</td>
            <td>The customs rate in percent</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>operatingCosts</td>
            <td>The operating costs for the variation in percent</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td>The ID of the VAT rate of the variation. VAT rates are created for each client (store) and linked to the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bundleType</td>
            <td>Indicates the bundle type of the variation. Possible values:<ul><li>bundle = The variation is a bundle</li><li>bundle_item = The variation is a bundle component.</li><li>Null = The variation is not associated with a bundle</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>automaticClientVisibility</td>
            <td>Indicates if the variation is set as available for any clients (stores). Possible values:<ul><li>0 / -1 (GET) or 0 (POST) = Variation is not available in any client (store).</li><li>1 / 2 (GET) or 1 (POST) = Variation is available in at least one client (store).</li></ul>The variation's actual visibility depends on the settings for net stock dependency.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>automaticListVisibility</td>
            <td>Indicates if the variation currently is visible in item lists. 3 = Variation is visible in item list because $isHiddenInCategoryList is false. 2, 1 = Variation is visible in item list because $isVisibleInListIfNetStockIsPositive is true and net stock is positive. 0, -1 = Variation is invisible in item list because $isInvisibleInListIfNetStockIsNotPositive is true and net stock is 0 or negative. -2 = Variation is invisible in item list because $isHiddenInCategoryList is true.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isHiddenInCategoryList</td>
            <td>Flag that indicates if the variation is hidden in the category list. If true, the variation will not be shown in any item category and will not be returned as a search result. The variation can only be accessed via its URL.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>defaultShippingCosts</td>
            <td>The default shipping costs for the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>mayShowUnitPrice</td>
            <td>Display unit price in the online store</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>salesRank</td>
            <td>The sales rank of the variation. This ranking is used to position top items automatically if the option <b>Automatically sort by monthly sales</b> (<b>Settings » Client (store) » Standard » Item layouts » Basic settings</b>) is set to <b>Yes</b>. The sales ranking is calculated daily. If the option <b>Automatically sort by monthly sales</b> is set to <b>No</b>, a value of 0 is returned and variations are sorted by position instead.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>parentVariationQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>singleItemCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Categories are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of categories is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Markets are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of markets is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>clientVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Clients (stores) are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of clients (stores) is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>salesPriceVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Sales prices are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of sales prices is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>supplierVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Suppliers are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of suppliers is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Warehouses are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of warehouses is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Properties are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of properties is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>tagVariationId</td>
            <td>Either the ID of the variation or the ID of the item's main variation. No other values are permitted.<ul><li>ID of the variation = Tags are not inherited from the main variation.</li><li>ID of the item's main variation = Inheritance of tags is active.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>hasCalculatedBundleWeight</td>
            <td>Indicates if the gross bundle weight is calculated by its components.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>hasCalculatedBundleNetWeight</td>
            <td>Indicates if the net bundle weight is calculated by its components.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>hasCalculatedBundlePurchasePrice</td>
            <td>Indicates if the net purchase price is calculated by its components.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>hasCalculatedBundleMovingAveragePrice</td>
            <td>Indicates if the moving average net purchase price is calculated by its components.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBarcodes</td>
            <td>An array of the barcodes of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBundleComponents</td>
            <td>An array of the bundle components of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationComponentBundles</td>
            <td>An array of the bundles that this variation is a component of.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationProperties</td>
            <td>An array of the properties of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>properties</td>
            <td>An array of the properties of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSalesPrices</td>
            <td>An array of the sales prices of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketItemNumbers</td>
            <td>An array of the barcodes of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationCategories</td>
            <td>An array of the categories of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationClients</td>
            <td>An array of the clients (stores) of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationMarkets</td>
            <td>An array of the markets of the variation.</td>
        </tr><tr>
            <td><a href="item#item_models_variationdefaultcategory">VariationDefaultCategory</a>
</td>
            <td>variationDefaultCategory</td>
            <td>An array of the default category of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSuppliers</td>
            <td>An array of the suppliers of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemTexts</td>
            <td>An array of the texts of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationTexts</td>
            <td>An array of the texts of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationWarehouses</td>
            <td>An array of the warehouses of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>tags</td>
            <td>An array of the tags of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>comments</td>
            <td>An array of the comments of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>images</td>
            <td>An array of the images of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemImages</td>
            <td>An array of the images of the item linked to the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemCrossSelling</td>
            <td>An array of the cross selling items of the item linked to the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemShippingProfiles</td>
            <td>An array of the shipping profiles of the item linked to the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationAdditionalSkus</td>
            <td>An array of additional SKUs of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSkus</td>
            <td>An array of SKUs of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationAttributeValues</td>
            <td>An array of the attribute values of the variation.</td>
        </tr><tr>
            <td><a href="item#item_models_unitcombination">UnitCombination</a>
</td>
            <td>unit</td>
            <td>The UnitCombination of the Variation. Object contains unitId and content.</td>
        </tr><tr>
            <td><a href="item#item_models_variation">Variation</a>
</td>
            <td>parent</td>
            <td>The details of the main variation of the variation if applicable.</td>
        </tr><tr>
            <td><a href="item#item_models_item">Item</a>
</td>
            <td>item</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>children</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>stockStorageLocations</td>
            <td>An array of the stockStorageLocations of the variation.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Exceptions<a name="item_variation_exceptions"></a>
### VariationException<a name="item_exceptions_variationexception"></a>

Class VariationException


#### Namespace

`Plenty\Modules\Item\Variation\Exceptions`




## Events<a name="item_variation_events"></a>
### BeforeStatisticAccess<a name="item_events_beforestatisticaccess"></a>

The event is triggered before a statics will be loaded


#### Namespace

`Plenty\Modules\Item\Variation\Events`





#### Methods

<pre>public <strong>isAccessAllowed</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setAccessAllowed</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $accessAllowed):<a href="item#item_events_beforestatisticaccess">BeforeStatisticAccess</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$accessAllowed</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getStatistic</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setStatistic</strong>(<a target="_blank" href="http://php.net/string">string</a> $statistic):<a href="item#item_events_beforestatisticaccess">BeforeStatisticAccess</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$statistic</td>
        <td></td>
    </tr>
</table>


# Services<a name="item_services"></a>
    
## ExportPreloadValue<a name="item_services_exportpreloadvalue"></a>
### ExportPreloadValue<a name="item_exportpreloadvalue_exportpreloadvalue"></a>

ExportPreloadValue


#### Namespace

`Plenty\Modules\Item\Variation\Services\ExportPreloadValue`




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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# DefaultShippingCost<a name="item_defaultshippingcost"></a>
    
## Contracts<a name="item_defaultshippingcost_contracts"></a>
### DefaultShippingCostRepositoryContract<a name="item_contracts_defaultshippingcostrepositorycontract"></a>

The contract for the default shipping cost repository


#### Namespace

`Plenty\Modules\Item\DefaultShippingCost\Contracts`





#### Methods

<pre>public <strong>findShippingCost</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/float">float</a> $referrerId, <a target="_blank" href="http://php.net/int">int</a> $shippingDestinationId, <a target="_blank" href="http://php.net/int">int</a> $paymentMethodId):<a target="_blank" href="http://php.net/float">float</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td>The ID of the referrer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingDestinationId</td>
        <td>The ID of the shipping destination</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


## Models<a name="item_defaultshippingcost_models"></a>
### DefaultShippingCost<a name="item_models_defaultshippingcost"></a>

The default shipping cost model


#### Namespace

`Plenty\Modules\Item\DefaultShippingCost\Models`




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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>profileId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationSupplier<a name="item_variationsupplier"></a>
    
## Contracts<a name="item_variationsupplier_contracts"></a>
### VariationSupplierRepositoryContract<a name="item_contracts_variationsupplierrepositorycontract"></a>

The contract for the variation supplier repository


#### Namespace

`Plenty\Modules\Item\VariationSupplier\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationsupplier">VariationSupplier</a>
</pre>

    
Gets the data of a supplier linked to a variation. The variation supplier ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between variation and supplier</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationsupplier">VariationSupplier</a>
</pre>

    
Creates a link between a supplier and a variation and adds supplier data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation supplier data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationsupplier">VariationSupplier</a>
</pre>

    
Updates the data of a supplier linked to a variation. The variation supplier ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation supplier data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between variation and supplier</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a link between a supplier and a variation. The variation supplier ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between variation and supplier</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the data of the suppliers linked to a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the data of the suppliers linked to a variation with inheritance details. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationsupplier_models"></a>
### VariationSupplier<a name="item_models_variationsupplier"></a>

Variation Supplier


#### Namespace

`Plenty\Modules\Item\VariationSupplier\Models`




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
            <td>The unique ID of the link between variation and supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>supplierId</td>
            <td>The unique ID of the supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td>The price at which the variation was purchased from this supplier.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minimumPurchase</td>
            <td>The minimum quantity of the variation that has to be ordered from the supplier. This value is also used as a quantity suggestion when creating reorders.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemNumber</td>
            <td>The external item number assigned to the variation by this supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastPriceQuery</td>
            <td>The date of the last price query to this supplier. This helps to plan price negotiations.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deliveryTimeInDays</td>
            <td>The delivery time in days for the variation saved for this supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>discount</td>
            <td>The discount in percent the supplier grants for the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isDiscountable</td>
            <td>Flag that indicates if the supplier's discount for this variation is active.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>packagingUnit</td>
            <td>The packaging unit of the supplier if it differs from the packaging unit settings in plentymarkets.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td>The time the supplier data was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the supplier data was created</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Property<a name="item_property"></a>
    
## Contracts<a name="item_property_contracts"></a>
### PropertyGroupRepositoryContract<a name="item_contracts_propertygrouprepositorycontract"></a>

The contract for the property group repository


#### Namespace

`Plenty\Modules\Item\Property\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_propertygroup">PropertyGroup</a>
</pre>

    
Creates a property group.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property group data as an associative array</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_propertygroup">PropertyGroup</a>
</pre>

    
Gets a property group. The ID of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property group</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_propertygroup">PropertyGroup</a>
</pre>

    
Updates a property group. The ID of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property group data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property group</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a property group. The ID of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property group</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_propertygroup">PropertyGroup</a>
</pre>

    
Gets a property group. The ID of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property group</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all property groups.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of shown property groups per page. Default value is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByBackendName</strong>(<a target="_blank" href="http://php.net/string">string</a> $backendName):<a href="item#item_models_propertygroup">PropertyGroup</a>
</pre>

    
Gets a property group. The backend name of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$backendName</td>
        <td></td>
    </tr>
</table>



### PropertyGroupNameRepositoryContract<a name="item_contracts_propertygroupnamerepositorycontract"></a>

The contract for the property group name repository


#### Namespace

`Plenty\Modules\Item\Property\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyGroupId):<a href="item#item_models_propertygroupname">PropertyGroupName</a>
</pre>

    
Creates a property group name. The ID of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property group name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyGroupId</td>
        <td>The ID of the property group</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyGroupId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a property group name. The ID of the property group and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyGroupId</td>
        <td>The ID of the property group</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The specific language of the property group name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyGroupId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertygroupname">PropertyGroupName</a>
</pre>

    
Updates a property group name. The ID of the property group and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property group name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyGroupId</td>
        <td>The ID of the property group</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The specific language of the property group name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyGroupId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertygroupname">PropertyGroupName</a>
</pre>

    
Gets a property group name. The ID of the property group and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyGroupId</td>
        <td>The ID of the property group</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The specific language of the property group name</td>
    </tr>
</table>


<pre>public <strong>findByPropertyGroupId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyGroupId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists property group names. The ID of the property group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyGroupId</td>
        <td>The ID of the property group</td>
    </tr>
</table>



### PropertyMarketReferenceRepositoryContract<a name="item_contracts_propertymarketreferencerepositorycontract"></a>

The contract for the property market reference repository


#### Namespace

`Plenty\Modules\Item\Property\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="item#item_models_propertymarketreference">PropertyMarketReference</a>
</pre>

    
Creates a property market reference. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property market component data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/float">float</a> $marketReference):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a property market reference. The ID of the property and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketReference</td>
        <td>The market reference value</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/float">float</a> $marketReference):<a href="item#item_models_propertymarketreference">PropertyMarketReference</a>
</pre>

    
Updates a property market reference. The ID of the property and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property market component data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketReference</td>
        <td>The market reference value</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/float">float</a> $marketReference):<a href="item#item_models_propertymarketreference">PropertyMarketReference</a>
</pre>

    
Gets a property market reference. The ID of the property and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketReference</td>
        <td>The market reference value</td>
    </tr>
</table>


<pre>public <strong>findByPropertyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="item#item_models_propertymarketreference">PropertyMarketReference</a>
</pre>

    
List of property market references. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>getPropertyMarketReferences</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrerId, <a target="_blank" href="http://php.net/int">int</a> $componentId = null, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all property market references.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td>The ID of the referrer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$componentId</td>
        <td>The ID of the component</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>You can pass here multiple filters. Available: `componentId` - pass multiple component IDs that should be searched for.</td>
    </tr>
</table>



### PropertyRepositoryContract<a name="item_contracts_propertyrepositorycontract"></a>

The contract for the property repository


#### Namespace

`Plenty\Modules\Item\Property\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_property">Property</a>
</pre>

    
Creates a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property data as an associative array</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_property">Property</a>
</pre>

    
Gets a property. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_property">Property</a>
</pre>

    
Updates a property. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a property. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_property">Property</a>
</pre>

    
Gets a property. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all properties.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of attribute values shown per page. Default value is 50</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filter = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Search properties.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of attribute values shown per page. Default value is 50</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByBackendName</strong>(<a target="_blank" href="http://php.net/string">string</a> $backendName):<a href="item#item_models_property">Property</a>
</pre>

    
Gets an property. The backend name of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$backendName</td>
        <td></td>
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
    

### PropertyNameRepositoryContract<a name="item_contracts_propertynamerepositorycontract"></a>

The contract for the property name repository


#### Namespace

`Plenty\Modules\Item\Property\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="item#item_models_propertyname">PropertyName</a>
</pre>

    
Creates a property name. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a property name. The ID of the property and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the property name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyname">PropertyName</a>
</pre>

    
Updates a property name. The ID of the property and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the property name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyname">PropertyName</a>
</pre>

    
Gets a property name. The ID of the property and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the property name</td>
    </tr>
</table>


<pre>public <strong>findBypropertyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="item#item_models_propertyname">PropertyName</a>
</pre>

    
Lists property names. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
</table>



### PropertySelectionRepositoryContract<a name="item_contracts_propertyselectionrepositorycontract"></a>

The contract for the property selection repository


#### Namespace

`Plenty\Modules\Item\Property\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>

    
Creates a property selection. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property selection data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>createLang</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>

    
Creates a property selection lang. The ID of the property selection must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property selection data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property selection</td>
    </tr>
</table>


<pre>public <strong>findByProperty</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/string">string</a> $lang = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List of property selections. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language</a> of the property selection</td>
    </tr>
</table>


<pre>public <strong>findByPropertyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="item#item_models_propertyselection">PropertySelection</a>
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
    
List of property selections. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the property</td>
    </tr>
</table>


<pre>public <strong>deleteSelection</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a property selection. The ID of the property selection must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property selection</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a property selection in a specified language. The ID of the property selection and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property selection</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language</a> of the property selection</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>

    
Get a property selection in the specified language. The ID of the property selection and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property selection</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language</a> of the property selection</td>
    </tr>
</table>


<pre>public <strong>findSelection</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a property selection. The ID of the property selection must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property selection</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>

    
Updates a property selection. The ID of the property selection and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The property selection data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the property selection</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language</a> of the property selection</td>
    </tr>
</table>


## Models<a name="item_property_models"></a>
### PropertySelection<a name="item_models_propertyselection"></a>

The property selection including the property


#### Namespace

`Plenty\Modules\Item\Property\Models`




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
            <td>The unique ID of the selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The unique ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The code of the language for which name and description of the selection were saved.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the selection. The name is displayed in the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the selection. This description is displayed in the online store.</td>
        </tr><tr>
            <td><a href="item#item_models_property">Property</a>
</td>
            <td>property</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyGroupName<a name="item_models_propertygroupname"></a>

The PropertyGroupName including PropertyGroup


#### Namespace

`Plenty\Modules\Item\Property\Models`




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
            <td>propertyGroupId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_propertygroup">PropertyGroup</a>
</td>
            <td>propertyGroup</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyMarketReference<a name="item_models_propertymarketreference"></a>

The PropertyMarketReference including Property


#### Namespace

`Plenty\Modules\Item\Property\Models`




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
            <td>propertyId</td>
            <td>The unique ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>componentId</td>
            <td>The unique ID of the reference for the market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td>The unique ID of the market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalComponent</td>
            <td>The external reference of the property</td>
        </tr><tr>
            <td><a href="item#item_models_property">Property</a>
</td>
            <td>property</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Property<a name="item_models_property"></a>

The property including Property name and property market reference


#### Namespace

`Plenty\Modules\Item\Property\Models`




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
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyGroupId</td>
            <td>The ID of the property group the property is assigned to. Value is null if property is not assigned to a property group.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>unit</td>
            <td>The unit of measurement of the property. Value is null if no unit is associated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The backend name of the property. The back end name is not visible to customers.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>comment</td>
            <td>Internal comment/note saved for the property. Internal comments are not visible to customers.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueType</td>
            <td>Permitted property values are: <ul><li>empty = No property type</li><li>int = A whole number can be saved for an item, e.g. a size.</li><li>float = A number with decimal places can be saved for an item, e.g. a measurement.</li><li>selection = One of several options can be saved for the item. The values of the property value Selection can be managed using the route PropertySelection.</li><li>text = Text can be saved for an item.</li><li>file = A file can be saved for an item.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSearchable</td>
            <td>Flag that indicates if items can be found by entering the property name as a search term.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isOderProperty</td>
            <td>Flag that indicates if the property is available in the order process. Depending on the property type, customers e.g. can enter a text or value or select an option from a drop-down list.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShownOnItemPage</td>
            <td>Flag that indicates if the property will be shown on the item's page in the online store-</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShownOnItemList</td>
            <td>Flag that indicates if the property will be shown in the item listing in the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShownAtCheckout</td>
            <td>Flag that indicates if the property will be shown in the order process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShownInPdf</td>
            <td>Flag that indicates if the property will be shown in PDF documents.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShownAsAdditionalCosts</td>
            <td>Display as additional costs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>surcharge</td>
            <td>The surcharge for the property. Surcharges will automatically be added to the item price in the detailed view of an item and in the order process. The default value is 0.00, i.e. no surcharge. In the plentymarkets front end, the template variable PriceDynamic displays the price of a variation including the surcharge.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the property was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketComponents</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>group</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>selections</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyName<a name="item_models_propertyname"></a>

The PropertyName including Property


#### Namespace

`Plenty\Modules\Item\Property\Models`




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
            <td>propertyId</td>
            <td>The unique ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language code of the property name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property. The property name is displayed in the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the property. The property description is displayed in the online store.</td>
        </tr><tr>
            <td><a href="item#item_models_property">Property</a>
</td>
            <td>property</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyGroup<a name="item_models_propertygroup"></a>

The PropertyGroup including PropertyGroupName


#### Namespace

`Plenty\Modules\Item\Property\Models`




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
            <td>The unique ID of the property group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The back end name of the property group. This name is not visible to customers.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderPropertyGroupingType</td>
            <td>Indicates how order properties are grouped for selection in the order process. This parameter is applicable to order properties of the type None only.<ul><li>none = Order properties are not grouped.</li><li>single = One of the grouped order properties can be selected from the drop-down list.</li><li>multi = Multiple order properties can be selected.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSurchargePercental</td>
            <td>Flag that indicates if surcharge values are calculated in percent.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ottoComponentId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the property group was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>properties</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationSku<a name="item_variationsku"></a>
    
## Contracts<a name="item_variationsku_contracts"></a>
### VariationSkuRepositoryContract<a name="item_contracts_variationskurepositorycontract"></a>

The contract of the variation sku repository


#### Namespace

`Plenty\Modules\Item\VariationSku\Contracts`





#### Methods

<pre>public <strong>generateSkuWithParent</strong>(<a target="_blank" href="http://php.net/array">array</a> $variation, <a target="_blank" href="http://php.net/float">float</a> $marketId, <a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/string">string</a> $sku = null, <a target="_blank" href="http://php.net/string">string</a> $parentSku = null, <a target="_blank" href="http://php.net/bool">bool</a> $setLastExportedTimestamp = true, <a target="_blank" href="http://php.net/bool">bool</a> $returnObject = false):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Generates or updates an SKU and parent SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$variation</td>
        <td>The array of values from the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td>The unique ID of the market</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The unique ID of the account</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sku</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$parentSku</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$setLastExportedTimestamp</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$returnObject</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateSku</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/float">float</a> $marketId, <a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/string">string</a> $sku = null, <a target="_blank" href="http://php.net/bool">bool</a> $setLastExportedTimestamp = true, <a target="_blank" href="http://php.net/bool">bool</a> $returnObject = false):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Generates or updates an SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the SKU</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td>The unique ID of the market</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The unique ID of the account</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$sku</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$setLastExportedTimestamp</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$returnObject</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationsku">VariationSku</a>
</pre>

    
Creates an SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $skuId):<a href="item#item_models_variationsku">VariationSku</a>
</pre>

    
Updates an SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$skuId</td>
        <td>The unique ID of the SKU</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $skuId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$skuId</td>
        <td>The unique ID of the SKU</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $skuId):<a href="item#item_models_variationsku">VariationSku</a>
</pre>

    
Gets an SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$skuId</td>
        <td>The unique ID of the SKU</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists SKUs
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists SKUs
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
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
    

### VariationSkuBulkRepositoryContract<a name="item_contracts_variationskubulkrepositorycontract"></a>

The contract of the variation SKU bulk repository.


#### Namespace

`Plenty\Modules\Item\VariationSku\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Creates multiple SKUs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateStatus</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids, <a target="_blank" href="http://php.net/string">string</a> $status):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates status for multiple SKUs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$status</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateExportedAt</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids, <a target="_blank" href="http://php.net/string">string</a> $time = &quot;&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates exportedAt for multiple SKUs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$time</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateStockUpdatedAt</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids, <a target="_blank" href="http://php.net/string">string</a> $time = &quot;&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates stockUpdatedAt for multiple SKUs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$time</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Deletes multiple SKUs.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_variationsku_models"></a>
### VariationSku<a name="item_models_variationsku"></a>

The variation SKU model


#### Namespace

`Plenty\Modules\Item\VariationSku\Models`




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
            <td>The row ID of the table plenty_item_variation_market_status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td>The ID of the market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountId</td>
            <td>The ID of the market account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>initialSku</td>
            <td>The initial SKU of the variation. The initial SKU cannot be modified even if the variation SKU is changed. However, it is possible to reset the variation SKU to the initial SKU.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sku</td>
            <td>The SKU of the variation. The SKU is adjustable but may not exist twice for the combination of market Id and account Id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>parentSku</td>
            <td>The Parent SKU of the variation. The Parent SKU is adjustable. The same Parent SKU value should be used on variations of same article.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isActive</td>
            <td>Flag that indicates if the item is ready for export (currently not in use).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the SKU was created (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the SKU was updated (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>exportedAt</td>
            <td>The time the variation was last exported (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>stockUpdatedAt</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deletedAt</td>
            <td>The time the variation was deleted (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>status</td>
            <td>The status of the variation after the export. Possible entries are INACTIVE, ERROR, SENT and ACTIVE.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>additionalInformation</td>
            <td>The field that contains additional information.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationBundle<a name="item_variationbundle"></a>
    
## Contracts<a name="item_variationbundle_contracts"></a>
### VariationBundleRepositoryContract<a name="item_contracts_variationbundlerepositorycontract"></a>

The contract for the variation bundle repository


#### Namespace

`Plenty\Modules\Item\VariationBundle\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $bundleId):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Gets a variation bundle. The ID of the bundle must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$bundleId</td>
        <td>The ID of the bundle</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Creates a variation bundle.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation bundle data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $bundleId):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Updates a variation bundle. The ID of the bundle must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation bundle data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$bundleId</td>
        <td>The ID of the bundle</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $bundleId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a variation bundle component. The ID of the bundle must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$bundleId</td>
        <td>The ID of the bundle</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Lists variation bundles. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByComponentId</strong>(<a target="_blank" href="http://php.net/int">int</a> $componentId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists variation bundles. The ID of the component variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$componentId</td>
        <td>The ID of the component variation</td>
    </tr>
</table>



### InternalVariationBundleRepositoryContract<a name="item_contracts_internalvariationbundlerepositorycontract"></a>

The contract for the variation bundle repository


#### Namespace

`Plenty\Modules\Item\VariationBundle\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $bundleId):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Gets a variation bundle. The ID of the bundle must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$bundleId</td>
        <td>The ID of the bundle</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Creates a variation bundle.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation bundle data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $bundleId):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Updates a variation bundle. The ID of the bundle must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation bundle data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$bundleId</td>
        <td>The ID of the bundle</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $bundleId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a variation bundle component. The ID of the bundle must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$bundleId</td>
        <td>The ID of the bundle</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationbundle">VariationBundle</a>
</pre>

    
Lists variation bundles. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByComponentId</strong>(<a target="_blank" href="http://php.net/int">int</a> $componentId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists variation bundles. The ID of the component variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$componentId</td>
        <td>The ID of the component variation</td>
    </tr>
</table>


## Models<a name="item_variationbundle_models"></a>
### VariationBundle<a name="item_models_variationbundle"></a>

The variation bundle


#### Namespace

`Plenty\Modules\Item\VariationBundle\Models`




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
            <td>The unique ID of the link that marks a variation as a bundle component</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation to which other variations are added to create a bundle</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>componentVariationId</td>
            <td>The unique ID of the variation added as bundle component</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>componentQuantity</td>
            <td>The quantity of the variation to be added as bundle component</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdatedTimestamp</td>
            <td>The time the bundle was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the bundle was created.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Search<a name="item_search"></a>
    
## Sort<a name="item_search_sort"></a>
### NameSorting<a name="item_sort_namesorting"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Sort`





#### Methods

<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public static <strong>isLanguageSupported</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>isLanguageActivated</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getM10lByLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $fallback = &quot;en&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fallback</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getLanguageByM10l</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $fallback = &quot;english&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fallback</td>
        <td></td>
    </tr>
</table>


## Contracts<a name="item_search_contracts"></a>
### VariationElasticSearchSearchRepositoryContract<a name="item_contracts_variationelasticsearchsearchrepositorycontract"></a>

kommt noch


#### Namespace

`Plenty\Modules\Item\Search\Contracts`





#### Methods

<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
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


<pre>public <strong>addSearch</strong>($search):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>



### VariationElasticSearchMultiSearchRepositoryContract<a name="item_contracts_variationelasticsearchmultisearchrepositorycontract"></a>

kommt noch


#### Namespace

`Plenty\Modules\Item\Search\Contracts`





#### Methods

<pre>public <strong>setIndex</strong>(<a href="cloud#cloud_index_indexinterface">IndexInterface</a>
 $index):<a href="cloud#cloud_contracts_elasticsearchmultisearchrepositorycontract">ElasticSearchMultiSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_index_indexinterface">IndexInterface</a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSearch</strong>($search):<a href="cloud#cloud_contracts_elasticsearchmultisearchrepositorycontract">ElasticSearchMultiSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### VariationElasticSearchScrollRepositoryContract<a name="item_contracts_variationelasticsearchscrollrepositorycontract"></a>

kommt noch


#### Namespace

`Plenty\Modules\Item\Search\Contracts`





#### Methods

<pre>public <strong>hasNext</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setNumberOfDocumentsPerShard</strong>(<a target="_blank" href="http://php.net/int">int</a> $size):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$size</td>
        <td></td>
    </tr>
</table>


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


<pre>public <strong>addSearch</strong>($search):<a href="cloud#cloud_contracts_elasticsearchsearchrepositorycontract">ElasticSearchSearchRepositoryContract</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$search</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>execute</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### VariationElasticSearchAvailibilityRepositoryContract<a name="item_contracts_variationelasticsearchavailibilityrepositorycontract"></a>

VariationElasticSearchAvailibilityRepositoryContract


#### Namespace

`Plenty\Modules\Item\Search\Contracts`





#### Methods

<pre>public <strong>isReady</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### VariationElasticSearchSettingsRepositoryContract<a name="item_contracts_variationelasticsearchsettingsrepositorycontract"></a>

Read and update search settings


#### Namespace

`Plenty\Modules\Item\Search\Contracts`





#### Methods

<pre>public <strong>getLanguages</strong>():<a href="item#item_models_languagesettings">LanguageSettings</a>
</pre>

    
Get language settings
    
<pre>public <strong>saveLanguages</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_languagesettings">LanguageSettings</a>
</pre>

    
Update language settings
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSearchSettings</strong>():<a href="item#item_models_searchsettings">SearchSettings</a>
</pre>

    
Get search settings
    
<pre>public <strong>saveSearchSettings</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_searchsettings">SearchSettings</a>
</pre>

    
Update search settings
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Repositories<a name="item_search_repositories"></a>
### VariationElasticSearchAvailibilityRepository<a name="item_repositories_variationelasticsearchavailibilityrepository"></a>

VariationElasticSearchAvailibilityRepository


#### Namespace

`Plenty\Modules\Item\Search\Repositories`





#### Methods

<pre>public <strong>isReady</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>isAvailable</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
## Models<a name="item_search_models"></a>
### SearchSettings<a name="item_models_searchsettings"></a>

The search settings model


#### Namespace

`Plenty\Modules\Item\Search\Models`




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
            <td>fields</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### LanguageSettings<a name="item_models_languagesettings"></a>

The language settings model


#### Namespace

`Plenty\Modules\Item\Search\Models`




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
            <td>languages</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Mutators<a name="item_search_mutators"></a>
### DefaultCategoryMutator<a name="item_mutators_defaultcategorymutator"></a>




#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>mutateRow</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, $key):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="item#item_mutators_defaultcategorymutator">DefaultCategoryMutator</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### SkuMutator<a name="item_mutators_skumutator"></a>




#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>mutateObject</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setAccount</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### VariationPropertyMutator<a name="item_mutators_variationpropertymutator"></a>

To be written...


#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### ImageMutator<a name="item_mutators_imagemutator"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setSorting</strong>(<a target="_blank" href="http://php.net/string">string</a> $field):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSections</strong>($sections):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$sections</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>mutateObject</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addClient</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addListing</strong>(<a target="_blank" href="http://php.net/int">int</a> $listingId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$listingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### BarcodeMutator<a name="item_mutators_barcodemutator"></a>




#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>mutateObject</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### KeyMutator<a name="item_mutators_keymutator"></a>




#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>getKeyList</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setKeyList</strong>($keyList):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$keyList</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getNestedKeyList</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setNestedKeyList</strong>($nestedKeyList):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$nestedKeyList</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### ImageDomainMutator<a name="item_mutators_imagedomainmutator"></a>

Converts image domains to client specific image domains.


#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>mutateObject</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setClient</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="item#item_search_mutators">Mutators</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### FacetMutator<a name="item_mutators_facetmutator"></a>




#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>facetSort</strong>(<a target="_blank" href="http://php.net/array">array</a> $a, <a target="_blank" href="http://php.net/array">array</a> $b):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$a</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$b</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### VariationPropertyGroupMutator<a name="item_mutators_variationpropertygroupmutator"></a>

To be written...


#### Namespace

`Plenty\Modules\Item\Search\Mutators`





#### Methods

<pre>public <strong>mutate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Suggestions<a name="item_search_suggestions"></a>
### SearchSuggestion<a name="item_suggestions_searchsuggestion"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Suggestions`





#### Methods

<pre>public <strong>setLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $language):<a href="item#item_search_suggestions">Suggestions</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setText</strong>(<a target="_blank" href="http://php.net/string">string</a> $text):<a href="cloud#cloud_search_suggestion">Suggestion</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$text</td>
        <td></td>
    </tr>
</table>



### SearchSuggestionProcessor<a name="item_suggestions_searchsuggestionprocessor"></a>

to be written


#### Namespace

`Plenty\Modules\Item\Search\Suggestions`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>


## Filter<a name="item_search_filter"></a>
### SalesPriceFilter<a name="item_filter_salespricefilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasAtLeastOnePrice</strong>(<a target="_blank" href="http://php.net/array">array</a> $priceIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$priceIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### PropertyFilter<a name="item_filter_propertyfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getPath</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasAtLeastOneProperty</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="item#item_search_filter">Filter</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasEachProperty</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="item#item_search_filter">Filter</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### TextFilter<a name="item_filter_textfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasAnyName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasNameInLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang = self::LANG_DE, <a target="_blank" href="http://php.net/string">string</a> $filter = self::FILTER_ANY_NAME):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>isLanguageSupported</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>isLanguageActivated</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getM10lByLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $fallback = &quot;en&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fallback</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getLanguageByM10l</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $fallback = &quot;english&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fallback</td>
        <td></td>
    </tr>
</table>



### VariationAvailabilityUpdatedAtFilter<a name="item_filter_variationavailabilityupdatedatfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getTimestamp</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### CrossSellingFilter<a name="item_filter_crosssellingfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>hasRelation</strong>(<a target="_blank" href="http://php.net/string">string</a> $relation):<a href="item#item_search_filter">Filter</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAnyRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $relations):<a href="item#item_search_filter">Filter</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$relations</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isDynamic</strong>():<a href="item#item_search_filter">Filter</a>
</pre>

    

    
<pre>public <strong>isManual</strong>():<a href="item#item_search_filter">Filter</a>
</pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### TagFilter<a name="item_filter_tagfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasTag</strong>(<a target="_blank" href="http://php.net/int">int</a> $tagId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAnyTag</strong>(<a target="_blank" href="http://php.net/array">array</a> $tagIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$tagIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAllTags</strong>(<a target="_blank" href="http://php.net/array">array</a> $tagIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$tagIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### VariationPropertyFilter<a name="item_filter_variationpropertyfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasPropertySelection</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAtLeastOnePropertySelection</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasEachPropertySelection</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### FeedbackRangeFilter<a name="item_filter_feedbackrangefilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasFeedbackGreaterThan</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### MarketFilter<a name="item_filter_marketfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>isVisibleForMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isVisibleForAtLeastOneMarket</strong>(<a target="_blank" href="http://php.net/array">array</a> $marketIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$marketIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isVisibleForAllMarkets</strong>(<a target="_blank" href="http://php.net/array">array</a> $marketIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$marketIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### ImageFilter<a name="item_filter_imagefilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getPath</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasMarketId</strong>(<a target="_blank" href="http://php.net/int">int</a> $marketId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSection</strong>(<a target="_blank" href="http://php.net/string">string</a> $section):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$section</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### BarcodeFilter<a name="item_filter_barcodefilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>hasCode</strong>($code, <a target="_blank" href="http://php.net/string">string</a> $precision):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$precision</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasId</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### SearchFilter<a name="item_filter_searchfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>setNamesString</strong>(<a target="_blank" href="http://php.net/string">string</a> $string, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$string</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSearchString</strong>(<a target="_blank" href="http://php.net/string">string</a> $value, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $precision = \Plenty\Modules\Cloud\ElasticSearch\Lib\ElasticSearch::SEARCH_TYPE_EXACT, <a target="_blank" href="http://php.net/string">string</a> $operator = \Plenty\Modules\Cloud\ElasticSearch\Lib\ElasticSearch::OR_OPERATOR):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$precision</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setVariationNumber</strong>(<a target="_blank" href="http://php.net/string">string</a> $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### FacetFilter<a name="item_filter_facetfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasAtLeastOneFacet</strong>(<a target="_blank" href="http://php.net/array">array</a> $facetIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$facetIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasEachFacet</strong>(<a target="_blank" href="http://php.net/array">array</a> $facetIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$facetIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasFacet</strong>(<a target="_blank" href="http://php.net/int">int</a> $facetIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$facetIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAFacet</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasAtLeastOneFacetValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $facetId, <a target="_blank" href="http://php.net/array">array</a> $valueIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$facetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$valueIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasEachFacetValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $facetId, <a target="_blank" href="http://php.net/array">array</a> $valueIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$facetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$valueIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### VariationBaseFilter<a name="item_filter_variationbasefilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasNumber</strong>(<a target="_blank" href="http://php.net/string">string</a> $number, <a target="_blank" href="http://php.net/string">string</a> $precision):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$number</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$precision</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isActive</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>isInactive</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasId</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasIds</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasItemIds</strong>(<a target="_blank" href="http://php.net/array">array</a> $itemIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$itemIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isMain</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>isChild</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>isSalable</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $bool = true):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$bool</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isSalableAndActive</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $bool = true):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$bool</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isHiddenInCategoryList</strong>($bool = true):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$bool</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasADescriptionInLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $language):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAnImageOrItemHasAnImage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasAnImage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasManufacturer</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasSupplier</strong>(<a target="_blank" href="http://php.net/int">int</a> $supplierId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$supplierId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAtLeastOneAvailability</strong>(<a target="_blank" href="http://php.net/array">array</a> $availabilities):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$availabilities</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasActiveChildren</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $bool = true):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$bool</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasChildren</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $bool = true):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$bool</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### CategoryFilter<a name="item_filter_categoryfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>isInAtLeastOneCategory</strong>(<a target="_blank" href="http://php.net/array">array</a> $categoryIds, <a target="_blank" href="http://php.net/string">string</a> $depth = self::DEPTH_ANY):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$categoryIds</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$depth</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getPathByDepth</strong>(<a target="_blank" href="http://php.net/string">string</a> $depth):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$depth</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isInEachCategory</strong>(<a target="_blank" href="http://php.net/array">array</a> $categoryIds, <a target="_blank" href="http://php.net/string">string</a> $depth = self::DEPTH_ANY):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$categoryIds</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$depth</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isInCategory</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/string">string</a> $depth = self::DEPTH_ANY):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$depth</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isInACategory</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### ItemFilter<a name="item_filter_itemfilter"></a>

to bew written


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasId</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasIds</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAnImage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasFlag1</strong>(<a target="_blank" href="http://php.net/int">int</a> $flagId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$flagId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasFlag2</strong>(<a target="_blank" href="http://php.net/int">int</a> $flagId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$flagId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasManufacturer</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasManufacturers</strong>(<a target="_blank" href="http://php.net/array">array</a> $manufacturerIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$manufacturerIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAManufacturer</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>isItemType</strong>(<a target="_blank" href="http://php.net/string">string</a> $itemType):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$itemType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### AttributeFilter<a name="item_filter_attributefilter"></a>

Filters the index by specific attributes or attribute values


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>hasAttribute</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAnyAttribute</strong>(<a target="_blank" href="http://php.net/array">array</a> $attributeIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAllAttributes</strong>(<a target="_blank" href="http://php.net/array">array</a> $attributeIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAttributeValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeValueId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeValueId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAnyAttributeValue</strong>(<a target="_blank" href="http://php.net/array">array</a> $attributeValueIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeValueIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAllAttributeValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $attributeValueIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeValueIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### VariationLastUpdatedFilter<a name="item_filter_variationlastupdatedfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getTimestamp</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### SkuFilter<a name="item_filter_skufilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>getPath</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>hasMarketId</strong>(<a target="_blank" href="http://php.net/float">float</a> $marketId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAccountId</strong>(<a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasStatus</strong>(<a target="_blank" href="http://php.net/string">string</a> $status):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$status</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### ClientFilter<a name="item_filter_clientfilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>isVisibleForClient</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isVisibleForAtLeastOneClient</strong>(<a target="_blank" href="http://php.net/array">array</a> $clientIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$clientIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isVisibleForAllClients</strong>(<a target="_blank" href="http://php.net/array">array</a> $clientIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$clientIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasAutomaticClientVisibility</strong>(<a target="_blank" href="http://php.net/array">array</a> $values):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
-1, 0, 1, 2
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>



### PriceFilter<a name="item_filter_pricefilter"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Filter`





#### Methods

<pre>public <strong>between</strong>(<a target="_blank" href="http://php.net/float">float</a> $min = null, <a target="_blank" href="http://php.net/float">float</a> $max = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$min</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$max</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>betweenByClient</strong>(<a target="_blank" href="http://php.net/float">float</a> $min = null, <a target="_blank" href="http://php.net/float">float</a> $max = null, <a target="_blank" href="http://php.net/int">int</a> $clientId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$min</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$max</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addStatement</strong>(<a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
 $statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_statement_statementinterface">StatementInterface</a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>($statement):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$statement</td>
        <td></td>
    </tr>
</table>


## Query<a name="item_search_query"></a>
### SearchQuery<a name="item_query_searchquery"></a>

foo


#### Namespace

`Plenty\Modules\Item\Search\Query`





#### Methods

<pre>public <strong>addBarcode</strong>(<a target="_blank" href="http://php.net/int">int</a> $boost):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$boost</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addNumericField</strong>(<a target="_blank" href="http://php.net/string">string</a> $field, <a target="_blank" href="http://php.net/int">int</a> $boost):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$boost</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addMultilingualField</strong>(<a target="_blank" href="http://php.net/string">string</a> $field, <a target="_blank" href="http://php.net/string">string</a> $language, <a target="_blank" href="http://php.net/int">int</a> $boost):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$boost</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addField</strong>(<a target="_blank" href="http://php.net/string">string</a> $field, <a target="_blank" href="http://php.net/int">int</a> $boost):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$boost</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setOperator</strong>(<a target="_blank" href="http://php.net/string">string</a> $operator):<a href="cloud#cloud_query_multimatchquery">MultiMatchQuery</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setFuzzy</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $fuzzy):<a href="cloud#cloud_query_multimatchquery">MultiMatchQuery</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$fuzzy</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>isLanguageSupported</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>isLanguageActivated</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getM10lByLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $fallback = &quot;en&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fallback</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getLanguageByM10l</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $fallback = &quot;english&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fallback</td>
        <td></td>
    </tr>
</table>


## Aggregations<a name="item_search_aggregations"></a>
### FacetTermsAggregation<a name="item_aggregations_facettermsaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>setFacetId</strong>(<a target="_blank" href="http://php.net/int">int</a> $facetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$facetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### AttributeValueListAggregation<a name="item_aggregations_attributevaluelistaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getSize</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### AttributeValueListAggregationProcessor<a name="item_aggregations_attributevaluelistaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### ItemAttributeValueCardinalityAggregation<a name="item_aggregations_itemattributevaluecardinalityaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### OptimizedAttributeValueListAggregationProcessor<a name="item_aggregations_optimizedattributevaluelistaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### AvailabilityAggregation<a name="item_aggregations_availabilityaggregation"></a>

aggregation for item availabilities


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### AvailabilityAggregationProcessor<a name="item_aggregations_availabilityaggregationprocessor"></a>

aggregation processor for item availabilities


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### ItemCardinalityAggregationProcessor<a name="item_aggregations_itemcardinalityaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>($data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### VariationAttributeValueListAggregationProcessor<a name="item_aggregations_variationattributevaluelistaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### FeedbackAggregationProcessor<a name="item_aggregations_feedbackaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### FacetFacetTermsAggregation<a name="item_aggregations_facetfacettermsaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### FacetAggregationProcessor<a name="item_aggregations_facetaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### PriceFacetFilterAggregation<a name="item_aggregations_pricefacetfilteraggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>setFacetId</strong>(<a target="_blank" href="http://php.net/int">int</a> $facetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$facetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setIndex</strong>($index):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### VariationCardinalityAggregation<a name="item_aggregations_variationcardinalityaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### CardinalityAggregationBase<a name="item_aggregations_cardinalityaggregationbase"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### ItemAttributeValueCardinalityAggregationProcessor<a name="item_aggregations_itemattributevaluecardinalityaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>($data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### ItemCardinalityAggregation<a name="item_aggregations_itemcardinalityaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### CategoryProcessor<a name="item_aggregations_categoryprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### CategoryBranchTermsAggregation<a name="item_aggregations_categorybranchtermsaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### FacetFilterAggregation<a name="item_aggregations_facetfilteraggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>setFacetId</strong>(<a target="_blank" href="http://php.net/int">int</a> $facetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$facetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setIndex</strong>($index):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### PriceRangeAggregationProcessor<a name="item_aggregations_pricerangeaggregationprocessor"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDependencies</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addMutator</strong>(<a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
 $mutator):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_mutator_mutatorinterface">MutatorInterface</a>
</td>
        <td>$mutator</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addCondition</strong>(<a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
 $conditions):<a href="cloud#cloud_lib_processor">Processor</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_condition_conditioninterface">ConditionInterface</a>
</td>
        <td>$conditions</td>
        <td></td>
    </tr>
</table>



### FacetAggregation<a name="item_aggregations_facetaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getSize</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPath</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### FacetFacetValuesTermsAggregation<a name="item_aggregations_facetfacetvaluestermsaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### CategoryAllTermsAggregation<a name="item_aggregations_categoryalltermsaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setSize</strong>($size = 10):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$size</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### PriceRangeAggregation<a name="item_aggregations_pricerangeaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getField</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregation</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### FeedbackAggregation<a name="item_aggregations_feedbackaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getRanges</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregation</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### VariationAttributeValueListAggregation<a name="item_aggregations_variationattributevaluelistaggregation"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Aggregations`





#### Methods

<pre>public <strong>getName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getField</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getSize</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getAggregation</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Helper<a name="item_search_helper"></a>
### SearchHelper<a name="item_helper_searchhelper"></a>

To be written


#### Namespace

`Plenty\Modules\Item\Search\Helper`





#### Methods

<pre>public <strong>getFacetSearch</strong>():<a href="cloud#cloud_document_documentsearch">DocumentSearch</a>
</pre>

    

    
<pre>public <strong>getFacetFilter</strong>():<a href="item#item_filter_facetfilter">FacetFilter</a>
</pre>

    

    
<pre>public <strong>getSearchQuery</strong>(<a target="_blank" href="http://php.net/string">string</a> $query):<a href="item#item_query_searchquery">SearchQuery</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


# ItemImage<a name="item_itemimage"></a>
    
## Contracts<a name="item_itemimage_contracts"></a>
### ItemImageAvailabilityRepositoryContract<a name="item_contracts_itemimageavailabilityrepositorycontract"></a>

The contract for the item image availability repository


#### Namespace

`Plenty\Modules\Item\ItemImage\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemimageavailability">ItemImageAvailability</a>
</pre>

    
Creates an image availability
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The image availability data as associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an image availability.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The image availability data as associative array</td>
    </tr>
</table>


<pre>public <strong>findByImageId</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId):<a href="item#item_models_itemimageavailability">ItemImageAvailability</a>
</pre>

    
Lists image availabilities. The ID of the image must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
</table>


<pre>public <strong>findByType</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="item#item_models_itemimageavailability">ItemImageAvailability</a>
</pre>

    
Lists image availabilities. The ID of the image and the type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of the image</td>
    </tr>
</table>



### ItemImageSettingsRepositoryContract<a name="item_contracts_itemimagesettingsrepositorycontract"></a>

Get, update or invalidate item image settings


#### Namespace

`Plenty\Modules\Item\ItemImage\Contracts`





#### Methods

<pre>public <strong>get</strong>():<a href="miscellaneous#miscellaneous_item_itemimagesettings">ItemImageSettings</a>
</pre>

    

    
<pre>public <strong>update</strong>($data):<a href="miscellaneous#miscellaneous_item_itemimagesettings">ItemImageSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>invalidate</strong>(<a target="_blank" href="http://php.net/string">string</a> $path):<a href="miscellaneous#miscellaneous_item_itemimagesettings">ItemImageSettings</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>invalidateStatus</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### ItemImageNameRepositoryContract<a name="item_contracts_itemimagenamerepositorycontract"></a>

The contract for the item image name repository


#### Namespace

`Plenty\Modules\Item\ItemImage\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemimagename">ItemImageName</a>
</pre>

    
Creates an image name
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The image name data as associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_itemimagename">ItemImageName</a>
</pre>

    
Updates an image name. The ID of the image and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The image name data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the image name</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an image name. The ID of the image and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the image name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_itemimagename">ItemImageName</a>
</pre>

    
Gets an image name. The ID of the image and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the image name</td>
    </tr>
</table>


<pre>public <strong>findByImageId</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all image names. The ID of the image must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
</table>



### ItemImageRepositoryContract<a name="item_contracts_itemimagerepositorycontract"></a>

The contract for the item image repository


#### Namespace

`Plenty\Modules\Item\ItemImage\Contracts`





#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $imageId):<a href="item#item_models_itemimage">ItemImage</a>
</pre>

    
Updates an image. The ID of the image must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The image data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an image. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId):<a href="item#item_models_itemimage">ItemImage</a>
</pre>

    
Shows an image. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The ID of the image</td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists images. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The ID of the image</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists images. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByItemIdAndOriginalChecksum</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/string">string</a> $checksum):<a href="item#item_models_itemimage">ItemImage</a>
</pre>

    
Shows an image. The ID of the item and hash must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$checksum</td>
        <td>The  MD5 checksum of the image</td>
    </tr>
</table>


<pre>public <strong>upload</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemimage">ItemImage</a>
</pre>

    
Uploads an item image
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The image data as associative array</td>
    </tr>
</table>


<pre>public <strong>warmup</strong>(<a target="_blank" href="http://php.net/array">array</a> $urls, <a target="_blank" href="http://php.net/string">string</a> $queue = &quot;plentymarkets-command&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Calls a stack of image urls to prepare cache
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$urls</td>
        <td>array of urls to call</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$queue</td>
        <td>name of queue</td>
    </tr>
</table>


<pre>public <strong>syncOldImagesToCDN</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
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
    
## Models<a name="item_itemimage_models"></a>
### ItemImage<a name="item_models_itemimage"></a>

The ItemImage Model


#### Namespace

`Plenty\Modules\Item\ItemImage\Models`




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
            <td>The unique ID of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item the image is associated with</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileType</td>
            <td>The file format of the image. Possible file formats: jpg, jpeg, png, gif, svg</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td>The path under which the image is saved.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the image. The position is used for sorting images in the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the image was uploaded.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the image details were last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>md5Checksum</td>
            <td>The MD5 hash value of the image file</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>md5ChecksumOriginal</td>
            <td>The MD5 hash value of the original image file</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>size</td>
            <td>The size of the image in pixels</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>width</td>
            <td>The width of the image in pixels</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>height</td>
            <td>The height of the image in pixels</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>url</td>
            <td>The URL under which the image can be accessed after the upload.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlMiddle</td>
            <td>The URL that points to the  medium-sized version of the item image.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlPreview</td>
            <td>The URL that points to the  first preview version of the item image.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlSecondPreview</td>
            <td>The URL that points to the second preview version of the item image.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>Lists the image's name details as an array.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>availabilities</td>
            <td>Lists the image's availability details as an array.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attributeValueImages</td>
            <td>Lists the attribute value image's details as an array.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemImageUpload<a name="item_models_itemimageupload"></a>

ItemImage


#### Namespace

`Plenty\Modules\Item\ItemImage\Models`




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
            <td>The ID of the image. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item the image is associated with</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileType</td>
            <td>The file format of the image. Possible file formats: JPG, JPEG, PNG, GIF, SVG</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td>The path under which the image is saved. Permitted characters for file names: alphanumeric (a-z, A-Z, 0-9), hypens (-), underscores (_).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the image. The position is used for sorting images in the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>created</td>
            <td>The time the image was uploaded.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updated</td>
            <td>The time the image details were last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uploadImageData</td>
            <td>The base64 encoded image data of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uploadUrl</td>
            <td>The URL under which the image can be accessed for uploading. Permitted characters for file names: alphanumeric (a-z, A-Z, 0-9), hypens (-), underscores (_).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uploadFileName</td>
            <td>The file name assigned to the uploaded image. Permitted characters for file names: alphanumeric (a-z, A-Z, 0-9), hypens (-), underscores (_).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>names</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>availabilities</td>
            <td>availabilities</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemImageAvailability<a name="item_models_itemimageavailability"></a>

ItemImageAvailability


#### Namespace

`Plenty\Modules\Item\ItemImage\Models`




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
            <td>imageId</td>
            <td>The ID of the image. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of referrer for which the image is available. Possible types: <ul><li>mandant = The image can be made available for clients (stores).</li><li>marketplace = The image can be made available for markets.</li><li>listing = The image can be made available for listings.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>For the type <b>mandant</b>, this is the plentyID of the client (store) for which the image is available. For the types <b>marketplace</b> and <b>listing</b>, this is the ID of the referrer for which the image is available. <ul><li><strong>-1.00</strong> = The image is available for all referrers of this type.</li></ul></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemImageName<a name="item_models_itemimagename"></a>

ItemImageName


#### Namespace

`Plenty\Modules\Item\ItemImage\Models`




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
            <td>imageId</td>
            <td>The ID of the image. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the image name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the image in the specified language</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>alternate</td>
            <td>The alternative name of the image in the specified language</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationBarcode<a name="item_variationbarcode"></a>
    
## Contracts<a name="item_variationbarcode_contracts"></a>
### VariationBarcodeRepositoryContract<a name="item_contracts_variationbarcoderepositorycontract"></a>

The contract of the variation barcode repository


#### Namespace

`Plenty\Modules\Item\VariationBarcode\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationbarcode">VariationBarcode</a>
</pre>

    
Gets a variation barcode. The ID of the variation and the ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationbarcode">VariationBarcode</a>
</pre>

    
Creates a variation barcode.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation barcode data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $barcodeId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationbarcode">VariationBarcode</a>
</pre>

    
Updates a variation barcode. The ID of the variation and the ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation barcode data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a variation barcode. The ID of the variation and the ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all barcodes of a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationbarcode_models"></a>
### VariationBarcode<a name="item_models_variationbarcode"></a>

Variation Barcode


#### Namespace

`Plenty\Modules\Item\VariationBarcode\Models`




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
            <td>code</td>
            <td>The code of the variation's barcode. The combination of code and barcode ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>barcodeId</td>
            <td>The unique ID of the barcode linked to the variation. The combination of code and barcode ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the variation's code was created.</td>
        </tr><tr>
            <td><a href="item#item_models_barcode">Barcode</a>
</td>
            <td>barcode</td>
            <td>The barcode of the variation's barcode</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ItemLabel<a name="item_itemlabel"></a>
    
## Contracts<a name="item_itemlabel_contracts"></a>
### ItemLabelRepositoryContract<a name="item_contracts_itemlabelrepositorycontract"></a>

The contract for the item label repository


#### Namespace

`Plenty\Modules\Item\ItemLabel\Contracts`





#### Methods

<pre>public <strong>generateLabel</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get a variation label
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The required data to generate the item label</td>
    </tr>
</table>


<pre>public <strong>listTemplates</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List item label templates
    
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
    
## Models<a name="item_itemlabel_models"></a>
### ItemLabel<a name="item_models_itemlabel"></a>

The item label model


#### Namespace

`Plenty\Modules\Item\ItemLabel\Models`




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
            <td>labelId</td>
            <td>The unique ID of the label template</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ItemSerialNumber<a name="item_itemserialnumber"></a>
    
## Contracts<a name="item_itemserialnumber_contracts"></a>
### ItemSerialNumberRepositoryContract<a name="item_contracts_itemserialnumberrepositorycontract"></a>

The contract of the item serial number repository


#### Namespace

`Plenty\Modules\Item\ItemSerialNumber\Contracts`





#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $perPage = 100, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all serial numbers.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_itemserialnumber">ItemSerialNumber</a>
</pre>

    
Gets a serial number. The ID of the serial number must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemserialnumber">ItemSerialNumber</a>
</pre>

    
Creates a serial number
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemserialnumber">ItemSerialNumber</a>
</pre>

    
Updates a serial number. The ID of the serial number must be specified.
    
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


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_contracts_deleteresponsecontract">DeleteResponseContract</a>
</pre>

    
Deletes a serial number. The ID of the serial number must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="item_itemserialnumber_models"></a>
### ItemSerialNumber<a name="item_models_itemserialnumber"></a>

The item serial number model


#### Namespace

`Plenty\Modules\Item\ItemSerialNumber\Models`




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
            <td>The ID of the serial number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderItemId</td>
            <td>The ID of the order item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>serialNumber</td>
            <td>The serial number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The date the serial number was created</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationDescription<a name="item_variationdescription"></a>
    
## Contracts<a name="item_variationdescription_contracts"></a>
### VariationDescriptionRepositoryContract<a name="item_contracts_variationdescriptionrepositorycontract"></a>

The contract of the variation description repository


#### Namespace

`Plenty\Modules\Item\VariationDescription\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationdescription">VariationDescription</a>
</pre>

    
Creates texts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation description data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_variationdescription">VariationDescription</a>
</pre>

    
Updates texts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation description data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The unique code of the language</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes texts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The unique code of the language</td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_variationdescription">VariationDescription</a>
</pre>

    
Gets texts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The unique code of the language</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationdescription">VariationDescription</a>
</pre>

    
Get texts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the item texts</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List texts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationdescription_models"></a>
### VariationDescription<a name="item_models_variationdescription"></a>

Variation Default Category


#### Namespace

`Plenty\Modules\Item\VariationDescription\Models`




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
            <td>The unique ID of the description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item that this description belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries" target="_blank">language code</a> of the description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The default name of the item. By default, this name is displayed in the online store. For Default items, this name is also used for markets. Character limit: max. 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td>Alternative item name that can be used e.g. for markets. Character limit: max. 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td>Alternative item name that can be used e.g. for markets. Character limit: max. 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>previewDescription</td>
            <td>The preview text. The preview text is a short description that can be displayed in item lists.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td>The meta description of the item. This description is analysed by search engines and displayed in search results. This text should be treated as an advertising text to maximise click-through from search engine result pages. Current recommended limit is 156 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The item description. This is a detailed description displayed in the item layout of the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>technicalData</td>
            <td>The technical data for the item. To display the technical data in the online store, insert the template variable TechnicalData and an optional title into the template ItemViewSingleItem.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlPath</td>
            <td>The URL path of the item in the online store. By default, the URL path consists of the categories and the item name. The path will be assigned automatically by plentymarkets when the item is created and will be displayed as part of the URL when the item is selected in the online store.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaKeywords</td>
            <td>Meta keywords to tag the item for search engines. More than one keyword can be separated by commas.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationSalesPrice<a name="item_variationsalesprice"></a>
    
## Contracts<a name="item_variationsalesprice_contracts"></a>
### VariationSalesPriceRepositoryContract<a name="item_contracts_variationsalespricerepositorycontract"></a>

The contract of the variation sales price repository


#### Namespace

`Plenty\Modules\Item\VariationSalesPrice\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>

    
Gets the price data of a sales price linked to a variation. The ID of the sales price and the ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>

    
Creates a link between a sales price and a variation and adds sales price data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation sales price data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>

    
Updates the data of a sales price linked to a variation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation sales price data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a link between a sales price and a variation and deletes the sales price data. The ID of the sales price and the ID of the variation must be specified. An exception is thrown if at least one relation exists.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>deleteAll</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes all links between a variation and its sales prices and deletes the sales price data. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>

    
Lists the data of the sales prices linked to a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>

    
Lists the data of the sales prices linked to a variation with inheritance details. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>updateBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Updates a list of variation prices. The variation ID, sales price ID and a new price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The array containing the data.</td>
    </tr>
</table>


<pre>public <strong>createBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Creates a list of variation prices. The variation ID, sales price ID and a new price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The array containing the data.</td>
    </tr>
</table>


<pre>public <strong>findAll</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 100, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Gets all sales price relations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="item_variationsalesprice_models"></a>
### VariationSalesPrice<a name="item_models_variationsalesprice"></a>

VariationSalesPrice


#### Namespace

`Plenty\Modules\Item\VariationSalesPrice\Models`




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
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td>The price of the variation saved for this sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Item<a name="item_item"></a>
    
## Contracts<a name="item_item_contracts"></a>
### ItemRepositoryContract<a name="item_contracts_itemrepositorycontract"></a>

The contract for the attribute value repository


#### Namespace

`Plenty\Modules\Item\Item\Contracts`





#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Creates an item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The item data as an associative array</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get an item. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The ID of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded.</td>
    </tr>
</table>


<pre>public <strong>search</strong>($columns = [], $lang = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$columns</td>
        <td>The array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$lang</td>
        <td>The language of the item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The items shown per page. Default value is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="item#item_models_item">Item</a>
</pre>

    
Update a item. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>bulkUpdate</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Update up to 50 items. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete an item. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
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
    
## Models<a name="item_item_models"></a>
### ItemEbayTitle<a name="item_models_itemebaytitle"></a>

The item ebay title model


#### Namespace

`Plenty\Modules\Item\Item\Models`




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
            <td>title</td>
            <td>The title.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The unique ID of the ebay title.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemText<a name="item_models_itemtext"></a>

The item text model


#### Namespace

`Plenty\Modules\Item\Item\Models`




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
            <td>lang</td>
            <td>The language of the item text.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name1</td>
            <td>Default name of the item displayed in the online store and used for markets. The maximum length is 240 characters. The item name is also used for structuring the item URL.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td>Alternative item name that can be used e.g. for markets. The maximum length is 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td>Alternative item name that can be used e.g. for markets. The maximum length is 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td>The preview text of the item. This short description text can be displayed as a teaser in item lists.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td>The meta description of the item. This description is analysed by search engines and displayed in search results. This text should be treated as an advertising text to maximise click-through from search engine result pages. Current recommended limit is 156 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The detailed description of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>technicalData</td>
            <td>Technical data of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keywords</td>
            <td>HTML meta keywords to tag the item for search engines. More than one keyword can be separated by commas.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlPath</td>
            <td>The item's URL path in the online store. By default, the URL path consists of the categories and the item name. The path is assigned automatically when the item is created and is displayed as part of the URL when the item is selected in the online store.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Item<a name="item_models_item"></a>

The item model


#### Namespace

`Plenty\Modules\Item\Item\Models`




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
            <td>The ID of the item. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemType</td>
            <td>The type of the item. Because Set items are managed using a separate route, this value is always Default.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockType</td>
            <td>The stock type of the item. Possible values:<ul><li>0 = Stocked item (default)</li><li>1 = Production item</li><li>2 = Colli</li><li>3 = Special order item</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storeSpecial</td>
            <td>Option to present items more prominently in the online store.<ul><li>1 = Special offer</li><li>2 = New items</li><li>3 = Top items</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ownerId</td>
            <td>The plentymarkets user that is assigned as owner of this item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>manufacturerId</td>
            <td>The ID of the manufacturer of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>producingCountryId</td>
            <td>The ID of the country in which the item was manufactured.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainVariationId</td>
            <td>The ID of the main variation of the item. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customsTariffNumber</td>
            <td>The customs tariff number of the item; usually a 11 digit code number based on the Harmonised System</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>revenueAccount</td>
            <td>The revenue account the item is linked to. An individual revenue account can be saved for each item in plentymarkets. If this is not done, plentymarkets automatically determines a revenue account based on the VAT rate.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>couponRestriction</td>
            <td>Indicates if the item can be purchased using a promotional coupon.<ul><li>0 = Permitted</li><li>1 = Not permitted</li><li>2 = Purchasable with coupon only</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>condition</td>
            <td>The condition of the item. Possible values:<ul><li>0 = New</li><li>1 = Used</li><li>2 = Boxed as new</li><li>3 = New with label</li><li>4 = Factory seconds</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>conditionApi</td>
            <td>The condition of the item that is transferred to markets via API.<ul><li>0 = New</li><li>1 = Used but as new</li><li>2 = Used but very good</li><li>3 = Used but good</li><li>4 = Used but acceptable</li><li>5 = Factory seconds</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>Timestamp of the date and time the item was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>Timestamp of the last date and time the item was updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSubscribable</td>
            <td>Flag that indicates if the item can be ordered as a subscription item. If yes, the item can be ordered for delivery at regular intervals.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSerialNumber</td>
            <td>Flag that indicates if serial numbers are to be assigned to variations of this item to uniquely identify every item sold. Serial numbers ensure traceability of an item in case of errors or problems.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShippingPackage</td>
            <td>Flag that indicates if a shipping package is to be used for this item. If yes and the variation's dimensions are entered in the <b>Settings</b> tab of a variation, the correct shipping package is assigned automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonFbaPlatform</td>
            <td>Indicates the platform used for Fulfilment by Amazon (FBA). <ul><li>0 = Do not use</li><li>1 = AMAZON EU (Europe)</li><li>2 = AMAZON FE (Far East)</li><li>3 = AMAZON NA (North America)</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShippableByAmazon</td>
            <td>Flag that indicates if the item can be shipped with Amazon Multi-Channel. Amazon Multi-Channel Fulfillment is a service for fulfilling orders from sales channels other than Amazon platforms using inventory stored in the Amazon fulfillment center.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonProductType</td>
            <td>The Amazon product type of the item. List of IDs: https://www.plentymarkets.co.uk/manual/data-exchange/data-formats/item/</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazonFedas</td>
            <td>The FEDAS product classification key of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayPresetId</td>
            <td>The eBay preset ID. This plentymarkets ID must be specified to save values for $ebayCategory, $ebayCategory2, $ebayStoreCategory and $ebayStoreCategory2.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory</td>
            <td>The eBay category 1 of the item. This category is used when a new listing is created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory2</td>
            <td>The eBay category 2 of the item. This category is used when a new listing is created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory</td>
            <td>The ID of the eBay store category 1 of the item. This value is used for new listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory2</td>
            <td>The ID of the eBay store category 2 of the item. This value is used for new listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rakutenCategoryId</td>
            <td>The ID of the Rakuten category of this item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flagOne</td>
            <td>Flag 1 of the item. Flags can be used to organise and filter items. Each item can be assigned up to two flags. Possible values: 1 to 31, 0 = no flag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flagTwo</td>
            <td>Flag 2 of the item. Flags can be used to organise and filter items. Each item can be assigned up to two flags. Possible values: 1 to 11, 0 = no flag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ageRestriction</td>
            <td>The age customers must be to purchase the item. Items with an age rating of 18+ must be linked to a shipping profile for which the PostIdent option is activated.<ul><li>0 = None available</li><li>3 = Released for ages 3 and up</li><li>6 = Ages 6 and up</li><li>9 = Ages 9 and up</li><li>12 = Ages 12 and up</li><li>14 = Ages 14 and up</li><li>16 = Ages 16 and up</li><li>18 = Ages 18 and up</li><li>50 = Not marked</li><li>88 = Not required</li><li>99 = Unknown</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedback</td>
            <td>The feedback, i.e. rating, that this item received. Possible values are 1 to 5 or 1 to 10 depending on the maximum rating setting. An initial feedback can be saved for items. The saved value will then be displayed as the initial feedback. Every time new feedback is submitted, the average value will be recalculated automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free1</td>
            <td>The content of the free text field 1. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free2</td>
            <td>The content of the free text field 2. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free3</td>
            <td>The content of the free text field 3. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free4</td>
            <td>The content of the free text field 4. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free5</td>
            <td>The content of the free text field 5. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free6</td>
            <td>The content of the free text field 6. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free7</td>
            <td>The content of the free text field 7. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free8</td>
            <td>The content of the free text field 8. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free9</td>
            <td>The content of the free text field 9. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free10</td>
            <td>The content of the free text field 10. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free11</td>
            <td>The content of the free text field 11. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free12</td>
            <td>The content of the free text field 12. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free13</td>
            <td>The content of the free text field 13. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free14</td>
            <td>The content of the free text field 14. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free15</td>
            <td>The content of the free text field 15. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free16</td>
            <td>The content of the free text field 16. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free17</td>
            <td>The content of the free text field 17. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free18</td>
            <td>The content of the free text field 18. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free19</td>
            <td>The content of the free text field 19. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free20</td>
            <td>The content of the free text field 20. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>maximumOrderQuantity</td>
            <td>The maximum order quantity of an item permitted per order. If a maximum order quantity is specified, no more than this quantity of any combination of the variations of the item can be ordered. Decimal values are possible to allow orders by weight or length. Default value is 0. If value is 0, the maximum order quantity is unlimited.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>texts</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>ebayTitles</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemShippingProfiles</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemProperties</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemCrossSelling</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variations</td>
            <td>An array of the variations of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemImages</td>
            <td>An array of the images of the item.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationMarketIdentNumber<a name="item_variationmarketidentnumber"></a>
    
## Contracts<a name="item_variationmarketidentnumber_contracts"></a>
### VariationMarketIdentNumberRepositoryContract<a name="item_contracts_variationmarketidentnumberrepositorycontract"></a>

The contract of the variation market ident number repository


#### Namespace

`Plenty\Modules\Item\VariationMarketIdentNumber\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationMarketIdentNumberId):<a href="item#item_models_variationmarketidentnumber">VariationMarketIdentNumber</a>
</pre>

    
Gets a market ident number (ASIN/ePID) of a variation. The ID of the market ident number must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationMarketIdentNumberId</td>
        <td>The unique ID of the market ident number</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationmarketidentnumber">VariationMarketIdentNumber</a>
</pre>

    
Creates a new market ident number (ASIN/ePID) for a variation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation market ident number data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $variationMarketIdentNumberId):<a href="item#item_models_variationmarketidentnumber">VariationMarketIdentNumber</a>
</pre>

    
Updates a market ident number (ASIN/ePID) of a variation. The ID of the market ident number must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation market ident number data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationMarketIdentNumberId</td>
        <td>The unique ID of the market ident number</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationMarketIdentNumberId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a market ident number (ASIN/ePID) of a variation. The ID of the market ident number must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationMarketIdentNumberId</td>
        <td>The unique ID of the market ident number</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the market ident numbers (ASIN/ePID) of a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationmarketidentnumber_models"></a>
### VariationMarketIdentNumber<a name="item_models_variationmarketidentnumber"></a>

Variation Market Ident Number


#### Namespace

`Plenty\Modules\Item\VariationMarketIdentNumber\Models`




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
            <td>The unique ID of the market ident number (ASIN/ePID) of a variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The country code of the market ident number (ASIN/ePID)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of market ident number (ASIN/ePID)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the market ident number  (ASIN/ePID)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the market ident number (ASIN/ePID)</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ItemProperty<a name="item_itemproperty"></a>
    
## Contracts<a name="item_itemproperty_contracts"></a>
### ItemPropertyRepositoryContract<a name="item_contracts_itempropertyrepositorycontract"></a>

The contract for the item property repository


#### Namespace

`Plenty\Modules\Item\ItemProperty\Contracts`





#### Methods

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
    
## Models<a name="item_itemproperty_models"></a>
### ItemPropertyValueText<a name="item_models_itempropertyvaluetext"></a>

The ItemPropertyValueText


#### Namespace

`Plenty\Modules\Item\ItemProperty\Models`




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
            <td>valueId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemProperty<a name="item_models_itemproperty"></a>

ItemPropertyValue


#### Namespace

`Plenty\Modules\Item\ItemProperty\Models`




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
            <td>The id of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertySelectionId</td>
            <td>The id of the property selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>valueInt</td>
            <td>The int value of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>valueFloat</td>
            <td>The float value of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueFile</td>
            <td>The file value of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>surcharge</td>
            <td>The surcharge of the variation property value</td>
        </tr><tr>
            <td><a href="item#item_models_property">Property</a>
</td>
            <td>property</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_propertyselection">PropertySelection</a>
</td>
            <td>propertySelection</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>valueTexts</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationCategory<a name="item_variationcategory"></a>
    
## Contracts<a name="item_variationcategory_contracts"></a>
### VariationCategoryRepositoryContract<a name="item_contracts_variationcategoryrepositorycontract"></a>

The contract for the variation category repository


#### Namespace

`Plenty\Modules\Item\VariationCategory\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationcategory">VariationCategory</a>
</pre>

    
Gets the link between a category and a variation. The ID of the variation and the ID of the category must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The ID of the category</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationcategory">VariationCategory</a>
</pre>

    
Creates a link between a category and a variation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation category data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationcategory">VariationCategory</a>
</pre>

    
Updates a link between a category and a variation. The ID of the variation and the ID of the category must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation category data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The ID of the category</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the link between a category and a variation. The ID of the variation and the ID of the category must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The ID of the category</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationcategory">VariationCategory</a>
</pre>

    
Lists the categories linked to a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationcategory">VariationCategory</a>
</pre>

    
Lists the categories linked to a variation including inheritance information. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Updates up to 50 links between variations and categories. The ID of the variations and the ID of the categories must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The array containing the data.</td>
    </tr>
</table>


<pre>public <strong>createBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Creates up to 50 links between variations and categories. The ID of the variations and the ID of the categories must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The array containing the data.</td>
    </tr>
</table>


## Models<a name="item_variationcategory_models"></a>
### VariationCategory<a name="item_models_variationcategory"></a>

Variation Category


#### Namespace

`Plenty\Modules\Item\VariationCategory\Models`




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
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryId</td>
            <td>The unique ID of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isNeckermannPrimary</td>
            <td>Flag that indicates if the category is the primary category for the market Neckermann for this variation.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Availability<a name="item_availability"></a>
    
## Contracts<a name="item_availability_contracts"></a>
### AvailabilityRepositoryContract<a name="item_contracts_availabilityrepositorycontract"></a>

Repository for item availability.


#### Namespace

`Plenty\Modules\Item\Availability\Contracts`





#### Methods

<pre>public <strong>findAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_availability">Availability</a>
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
    
Gets an item availability. The ID of the availability must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the item availability</td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_availability">Availability</a>
</pre>

    
Gets an item availability. The ID of the availability must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the item availability</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_availability">Availability</a>
</pre>

    
Updates an item availability.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all item availabilities.
    
## Models<a name="item_availability_models"></a>
### Availability<a name="item_models_availability"></a>

The item availability model


#### Namespace

`Plenty\Modules\Item\Availability\Models`




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
            <td>The ID of this availability</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>icon</td>
            <td>The icon of this availability</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>averageDays</td>
            <td>The average delivery time in days for this availability</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AvailabilityName<a name="item_models_availabilityname"></a>

The item availability name model


#### Namespace

`Plenty\Modules\Item\Availability\Models`




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
            <td>availabilityId</td>
            <td>The ID of the availability that the name belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language code</a> of the availability name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the item availability in the specified language</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationImage<a name="item_variationimage"></a>
    
## Contracts<a name="item_variationimage_contracts"></a>
### VariationImageRepositoryContract<a name="item_contracts_variationimagerepositorycontract"></a>

The contract of the variation image repository


#### Namespace

`Plenty\Modules\Item\VariationImage\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationimage">VariationImage</a>
</pre>

    
Creates link between image and variation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation image data as an associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $imageId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes Link between image and variation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The unique ID of the image</td>
    </tr>
</table>


<pre>public <strong>findByImageId</strong>(<a target="_blank" href="http://php.net/int">int</a> $imageId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists variations linked to an image
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$imageId</td>
        <td>The unique ID of the image</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists images linked to a variation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all images linked to an item. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the image</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationimage">VariationImage</a>
</pre>

    
Gets an image link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the image link</td>
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
    
## Models<a name="item_variationimage_models"></a>
### VariationImage<a name="item_models_variationimage"></a>




#### Namespace

`Plenty\Modules\Item\VariationImage\Models`




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
            <td>The unique ID of the link between a variation and an image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>imageId</td>
            <td>The unique ID of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the image was linked to the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the link between an image and a variation was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Stock<a name="item_stock"></a>
    
## Hooks<a name="item_stock_hooks"></a>
### CheckItemStock<a name="item_hooks_checkitemstock"></a>

CheckItemStock


#### Namespace

`Plenty\Modules\Item\Stock\Hooks`





#### Methods

<pre>public <strong>handle</strong>(<a href="basket#basket_basketitem_basketitemevent">BasketItemEvent</a>
 $basketItemEvent):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="basket#basket_basketitem_basketitemevent">BasketItemEvent</a>
</td>
        <td>$basketItemEvent</td>
        <td></td>
    </tr>
</table>


## Events<a name="item_stock_events"></a>
### BasketItemWarnOversell<a name="item_events_basketitemwarnoversell"></a>

The event is triggered to warn about an overselling.


#### Namespace

`Plenty\Modules\Item\Stock\Events`





#### Methods

<pre>public <strong>getBasketItem</strong>():<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    

    
<pre>public <strong>getQuantity</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
# VariationMarket<a name="item_variationmarket"></a>
    
## Contracts<a name="item_variationmarket_contracts"></a>
### VariationMarketRepositoryContract<a name="item_contracts_variationmarketrepositorycontract"></a>

The contract of the variation market repository


#### Namespace

`Plenty\Modules\Item\VariationMarket\Contracts`





#### Methods

<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/float">float</a> $marketplaceId):<a href="item#item_models_variationmarket">VariationMarket</a>
</pre>

    
Gets the data of a market linked to a variation. The ID of the market and the ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketplaceId</td>
        <td>The unique ID of the market</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationmarket">VariationMarket</a>
</pre>

    
Creates a link between a market and a variation and adds market data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation market data as an associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $marketplaceId, <a target="_blank" href="http://php.net/float">float</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the link between a market and a variation. The ID of the market and the ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketplaceId</td>
        <td>The unique ID of the market</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationmarket">VariationMarket</a>
</pre>

    
Lists the markets linked to a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationmarket">VariationMarket</a>
</pre>

    
Lists the markets linked to a variation with inheritance details. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>getVariationMarkets</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all links between variations and markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Creates up to 50 links between variations and markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteBulk</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes all market links of the variation specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="item_variationmarket_models"></a>
### VariationMarket<a name="item_models_variationmarket"></a>

Variation Market


#### Namespace

`Plenty\Modules\Item\VariationMarket\Models`




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
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketId</td>
            <td>The unique ID of the market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the link between the variation and the market was created.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Barcode<a name="item_barcode"></a>
    
## Contracts<a name="item_barcode_contracts"></a>
### BarcodeRepositoryContract<a name="item_contracts_barcoderepositorycontract"></a>

The contract for the barcode repository


#### Namespace

`Plenty\Modules\Item\Barcode\Contracts`





#### Methods

<pre>public <strong>showBarcode</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcode">Barcode</a>
</pre>

    
Gets a barcode. The ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The ID of the barcode.</td>
    </tr>
</table>


<pre>public <strong>createBarcode</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_barcode">Barcode</a>
</pre>

    
Creates a barcode.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The barcode data as associative array</td>
    </tr>
</table>


<pre>public <strong>updateBarcode</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcode">Barcode</a>
</pre>

    
Updates a barcode. The ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The barcode data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The ID of the barcode.</td>
    </tr>
</table>


<pre>public <strong>deleteBarcode</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a barcode. The ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
</table>


<pre>public <strong>findBarcodeById</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcode">Barcode</a>
</pre>

    
Gets a barcode. The ID of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
</table>


<pre>public <strong>findBarcodesByType</strong>(<a target="_blank" href="http://php.net/string">string</a> $barcodeType, <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists barcodes. The type of the barcode must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$barcodeType</td>
        <td>The type of the barcode</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The number of barcodes shown per page. Default value is 50.</td>
    </tr>
</table>


<pre>public <strong>allBarcodes</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all barcodes.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The number of barcodes shown per page. Default value is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1.</td>
    </tr>
</table>


<pre>public <strong>createBarcodeReferrerRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcodelinkreferrer">BarcodeLinkReferrer</a>
</pre>

    
Creates new barcode referrer for specified referrer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The barcode data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
</table>


<pre>public <strong>deleteBarcodeReferrerRelation</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrer, <a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes barcode referrer with specified referrer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrer</td>
        <td>The float value of the referrer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td>The unique ID of the barcode</td>
    </tr>
</table>


<pre>public <strong>findBarcodesByReferrerRelation</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrer, <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets barcode referrer by specified referrer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrer</td>
        <td>The float value of the referrer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The number of barcodes shown per page. Default value is 50.</td>
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
    
## Models<a name="item_barcode_models"></a>
### BarcodeLinkReferrer<a name="item_models_barcodelinkreferrer"></a>

The barcode link referrer model including the barcode


#### Namespace

`Plenty\Modules\Item\Barcode\Models`




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
            <td>barcodeId</td>
            <td>The unique ID of the barcode</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The unique ID of the referrer. To activate all referrers, the value <strong>-1</strong> must be specified. This value activates all referrers in the system by default, including any referrers added at a later stage.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the barcode was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the barcode was last updated.</td>
        </tr><tr>
            <td><a href="item#item_models_barcode">Barcode</a>
</td>
            <td>barcode</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Barcode<a name="item_models_barcode"></a>

The barcode model including barcode referrer


#### Namespace

`Plenty\Modules\Item\Barcode\Models`




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
            <td>The unique ID of the barcode</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the barcode</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the barcode. Possible values: GTIN_8, GTIN_13, GTIN_14, GTIN_128, ISBN, QR, CODE_128, UPC</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the code was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>referrers</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationAdditionalSku<a name="item_variationadditionalsku"></a>
    
## Contracts<a name="item_variationadditionalsku_contracts"></a>
### VariationAdditionalSkuRepositoryContract<a name="item_contracts_variationadditionalskurepositorycontract"></a>

The contract of the variation additional sku repository


#### Namespace

`Plenty\Modules\Item\VariationAdditionalSku\Contracts`





#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists additional SKUs
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationadditionalsku">VariationAdditionalSku</a>
</pre>

    
Gets an additional SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the additional SKU</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationadditionalsku">VariationAdditionalSku</a>
</pre>

    
Creates an additional SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationadditionalsku">VariationAdditionalSku</a>
</pre>

    
Updates an additional SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the SKU</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes an additional SKU
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the additional SKU</td>
    </tr>
</table>


## Models<a name="item_variationadditionalsku_models"></a>
### VariationAdditionalSku<a name="item_models_variationadditionalsku"></a>

The variation additional SKU model for order import


#### Namespace

`Plenty\Modules\Item\VariationAdditionalSku\Models`




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
            <td>The ID of the additional sku</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The ID of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td>The ID of the market reference.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketAccountId</td>
            <td>The ID of the market account.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sku</td>
            <td>The additional sku for this variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the SKU was created (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the SKU was updated (YYYY-MM-DD HH:MM:SS).</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationProperty<a name="item_variationproperty"></a>
    
## Contracts<a name="item_variationproperty_contracts"></a>
### VariationPropertyValueTextRepositoryContract<a name="item_contracts_variationpropertyvaluetextrepositorycontract"></a>

The contract of the variation property value text repository


#### Namespace

`Plenty\Modules\Item\VariationProperty\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationpropertyvaluetext">VariationPropertyValueText</a>
</pre>

    
Saves text for a specific property of the type Text in the specified language. The ID of the property value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationpropertyvaluetext">VariationPropertyValueText</a>
</pre>

    
Updates the text saved for a specific property of the type Text in the specified language. The ID of the property value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the text saved for a specific property of the type Text in the specified language. The ID of the property value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_variationpropertyvaluetext">VariationPropertyValueText</a>
</pre>

    
Gets the text saved for a specific property of the type Text in the specified language. The ID of the property value and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>findByPropertyValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Gets the texts saved for a specific property of the type Text in all available languages. The ID of the property value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
</table>



### VariationPropertyValueRepositoryContract<a name="item_contracts_variationpropertyvaluerepositorycontract"></a>

The contract of the variation property value repository


#### Namespace

`Plenty\Modules\Item\VariationProperty\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationpropertyvalue">VariationPropertyValue</a>
</pre>

    
Creates a link between a property value and a variation and adds property value data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation property value data as an associative array</td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationpropertyvalue">VariationPropertyValue</a>
</pre>

    
Gets the data of a property value linked to a variation. The ID of the variation property value and the variation ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between a variation and a property value</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_variationpropertyvalue">VariationPropertyValue</a>
</pre>

    
Updates the data of a variation property linked to a variation. The ID of the variation property value and the variation ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation property value data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the Variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between a property value and a variation</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the link between a property value and a variation. The ID of the variation property value and the variation ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between a variation and a property value</td>
    </tr>
</table>


<pre>public <strong>deleteAll</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes all links between a variation and its property values. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the property values linked to a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>createBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Creates a list of variation properties.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The array containing the data.</td>
    </tr>
</table>


<pre>public <strong>updateBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Updates a list of variation properties.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The array containing the data.</td>
    </tr>
</table>


## Models<a name="item_variationproperty_models"></a>
### VariationPropertyValue<a name="item_models_variationpropertyvalue"></a>

The VariationPropertyValue


#### Namespace

`Plenty\Modules\Item\VariationProperty\Models`




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
            <td>The unique ID of the link between the variation and the property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The unique ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertySelectionId</td>
            <td>The unique ID of the property selection of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>valueInt</td>
            <td>The int value of the property value of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>valueFloat</td>
            <td>The float value of the property value of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueFile</td>
            <td>The file value of the property value of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>surcharge</td>
            <td>The surcharge of the property value of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>Collection of the variationPropertyValueNames names that belong to this variationPropertyValue</td>
        </tr><tr>
            <td><a href="item#item_models_property">Property</a>
</td>
            <td>property</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_propertyselection">PropertySelection</a>
</td>
            <td>propertySelection</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>valueTexts</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationPropertyValueName<a name="item_models_variationpropertyvaluename"></a>

The property name of the variation


#### Namespace

`Plenty\Modules\Item\VariationProperty\Models`




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
            <td>propertyValueId</td>
            <td>The unique ID of the link between the variation and the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries" target="_blank">language</a> of the property value name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property value name in the specified language</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationPropertyValueText<a name="item_models_variationpropertyvaluetext"></a>

The VariationPropertyValueText


#### Namespace

`Plenty\Modules\Item\VariationProperty\Models`




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
            <td>valueId</td>
            <td>The unique ID of the link between the variation and the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language</a> of the property value text</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The text saved for the property of the type Text</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ItemShippingProfiles<a name="item_itemshippingprofiles"></a>
    
## Contracts<a name="item_itemshippingprofiles_contracts"></a>
### ItemShippingProfilesRepositoryContract<a name="item_contracts_itemshippingprofilesrepositorycontract"></a>

Repository for ItemShippingProfiles


#### Namespace

`Plenty\Modules\Item\ItemShippingProfiles\Contracts`





#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_itemshippingprofiles">ItemShippingProfiles</a>
</pre>

    
Finds a shipping profile link by ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between shipping profile and item</td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all shipping profiles activated for an item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td>The unique ID of the item</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_itemshippingprofiles">ItemShippingProfiles</a>
</pre>

    
Activates a shipping profile for an item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deactivates a shipping profile for an item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The unique ID of the link between shipping profile and item</td>
    </tr>
</table>


<pre>public <strong>getItemShippingProfiles</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage, <a target="_blank" href="http://php.net/int">int</a> $page):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all shipping profiles of all items
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Activates up to 50 shipping profiles for items
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteBulk</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deactivates all shipping profiles for an item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingProfileId, <a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete the link between the specified shipping profile and item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingProfileId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="item_itemshippingprofiles_models"></a>
### ItemShippingProfiles<a name="item_models_itemshippingprofiles"></a>

The shipping profile model


#### Namespace

`Plenty\Modules\Item\ItemShippingProfiles\Models`




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
            <td>The unique ID of the link between item and shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The unique ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>profileId</td>
            <td>The unique ID of the shipping profile</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# DataLayer<a name="item_datalayer"></a>
    
## Contracts<a name="item_datalayer_contracts"></a>
### ItemDataLayerRepositoryContract<a name="item_contracts_itemdatalayerrepositorycontract"></a>



<div class="panel panel-warning">
    <div class="panel-heading">
        <h3 class="panel-title">
            <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
            Deprecated! <small>(since 2017-08-22)</small>        </h3>
    </div>
    <div class="panel-body">
        Please use Plenty\Modules\Item\Variation\Contracts\VariationSearchRepositoryContract or Plenty\Modules\Item\Search\Contracts\VariationElasticSearchSearchRepositoryContract instead
    </div>
</div>

#### Namespace

`Plenty\Modules\Item\DataLayer\Contracts`





#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="item#item_models_recordlist">RecordList</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>lookup</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $params = [], <a target="_blank" href="http://php.net/bool">bool</a> $calculateNumberOfRows = false):<a href="item#item_services_itemdatalayerresultlookup">ItemDataLayerResultLookup</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$calculateNumberOfRows</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>searchWithPagination</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_datalayer_models"></a>
### Record<a name="item_models_record"></a>

Record


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td><a href="item#item_models_itembase">ItemBase</a>
</td>
            <td>itemBase</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemPropertyList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemCrossSellingList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_itemdescription">ItemDescription</a>
</td>
            <td>itemDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemShippingProfilesList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationAttributeValueList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationbarcode">VariationBarcode</a>
</td>
            <td>variationBarcode</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBarcodeList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationbase">VariationBase</a>
</td>
            <td>variationBase</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBundleComponentList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationCategoryList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationImageList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationLinkMarketplace</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationLinkWebstore</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationmarketstatus">VariationMarketStatus</a>
</td>
            <td>variationMarketStatus</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationretailprice">VariationRetailPrice</a>
</td>
            <td>variationRecommendedRetailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationRecommendedRetailPriceList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationretailprice">VariationRetailPrice</a>
</td>
            <td>variationRetailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationRetailPriceList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationstandardcategory">VariationStandardCategory</a>
</td>
            <td>variationStandardCategory</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationstock">VariationStock</a>
</td>
            <td>variationStock</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationstockbuffer">VariationStockBuffer</a>
</td>
            <td>variationStockBuffer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationStockList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSupplierList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationwarehouse">VariationWarehouse</a>
</td>
            <td>variationWarehouse</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationWarehouseList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationspecialofferretailprice">VariationSpecialOfferRetailPrice</a>
</td>
            <td>variationSpecialOfferRetailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSpecialOfferRetailPriceList</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationAttributeValue<a name="item_models_variationattributevalue"></a>

VariationAttributeValue


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>attributeId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationLinkWebstore<a name="item_models_variationlinkwebstore"></a>

VariationLinkWebstore


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>created</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationBase<a name="item_models_variationbase"></a>

VariationBase


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>active</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueSetId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockInvisible</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bundleTyp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockNoStockIcon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockPositiveStockIcon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockVisible</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>availability</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>averageOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>content</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitCombinationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>estimatedAvailability</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>heightMm</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lengthMm</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>limitOrderByStockSelect</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainWarehouse</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>model</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>operatingCostsPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnits</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnitType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>parentItemVariationQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>picking</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customsPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceCalculationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>primaryVariation</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>primaryVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>storageCosts</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>transportationCosts</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>unitId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitLoadDevice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitsContained</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightG</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightNetG</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>maximumOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minimumOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>intervalOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>availableUntil</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>releaseDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>widthMm</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationImage<a name="item_models_variationimage"></a>

VariationImage


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>imageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>cleanImageName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemBase<a name="item_models_itembase"></a>

ItemDataLayer - ItemBase


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>abo</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addCmsPage</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonFba</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonProductType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>apiCondition</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storeSpecial</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>bestofferAutoDeclinePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>condition</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>crossSellingCharacter</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customsTariffNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>defaultShippingCost</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directCrossArticle</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayPreset</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>epid</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fedas</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>markingOne</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>markingTwo</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>flashFile</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flashHeight</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flashWidth</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free3</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free4</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free5</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free6</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free7</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free8</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free9</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free10</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free11</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free12</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free13</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free14</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free15</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free16</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free17</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free18</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free19</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free20</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ageRestriction</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>hasAttribute</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>inactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isPacket</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketStockBuffer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>noCoupon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>producingCountryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceOnly4orderby</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>producer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>producerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rating</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>revenueAccount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>scoActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>scoMinPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>scoMinStockNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>serialNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingWithAmazonFba</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sitemapPublished</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storingPosition</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>votes</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>tradoriaCategory</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationRetailPrice<a name="item_models_variationretailprice"></a>

VariationRetailPrice


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>priceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>retailPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>basePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkup</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkupNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>classRebatePercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>classRebate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>classRebateNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryRebatePercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryRebate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryRebateNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRatio</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationSupplier<a name="item_models_variationsupplier"></a>

VariationSupplier


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>deliveryTimeInDays</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>discount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>discountable</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemNumber</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>itemVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastPriceQuery</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minimumOrderValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>packagingUnit</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>supplierId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationSpecialOfferRetailPrice<a name="item_models_variationspecialofferretailprice"></a>

VariationSpecialOfferRetailPrice


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>retailPriceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>retailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>retailPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkup</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkupNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatValue</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>currency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRatio</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationStock<a name="item_models_variationstock"></a>

VariationStock


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>warehouseId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>stockPhysical</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedStock</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedEbay</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reorderDelta</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockNet</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updateAmazon</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatePixmania</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>warehouseType</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reordered</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedBundle</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>averagePurchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>warehousePriority</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastCalculateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedOutOfStock</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedBasket</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### DataLayerModel<a name="item_models_datalayermodel"></a>




#### Namespace

`Plenty\Modules\Item\DataLayer\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemCrossSelling<a name="item_models_itemcrossselling"></a>

ItemCrossSelling


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>crossItemId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>relationship</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dynamic</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationWarehouse<a name="item_models_variationwarehouse"></a>

VariationWarehouse


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>variationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseZoneId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reorderLevel</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maximumStock</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockBuffer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockTurnoverInDays</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storageLocationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationStockBuffer<a name="item_models_variationstockbuffer"></a>

VariationStockBuffer


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>stockBuffer</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationLinkMarketplace<a name="item_models_variationlinkmarketplace"></a>

VariationLinkMarketplace


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>created</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketplaceId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemShippingProfiles<a name="item_models_itemshippingprofiles"></a>

ItemShippingProfiles


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>tags</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationStandardCategory<a name="item_models_variationstandardcategory"></a>

VariationStandardCategory


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>categoryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>manually</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RecordList<a name="item_models_recordlist"></a>

RecordList


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationCategory<a name="item_models_variationcategory"></a>

VariationCategory


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>categoryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>neckermannPrimary</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemProperty<a name="item_models_itemproperty"></a>

ItemProperty


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>itemPropertyId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>propertyValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>propertyValueType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isOrderProperty</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>propertyOrderMarkup</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemDescription<a name="item_models_itemdescription"></a>

ItemDescription


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>characterCache</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>characterCacheXml</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>characterUpdate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keywords</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>technicalData</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlContent</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationBundleComponent<a name="item_models_variationbundlecomponent"></a>

VariationBundleComponent


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>componentVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>componentQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>CreatedTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>LastUpdateTimestamp</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationBarcode<a name="item_models_variationbarcode"></a>

VariationBarcode


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td>code</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>barcodeId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>barcodeType</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### VariationMarketStatus<a name="item_models_variationmarketstatus"></a>

VariationMarketStatus


#### Namespace

`Plenty\Modules\Item\DataLayer\Models`




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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketAccountId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>initialSku</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>sku</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>parentSku</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>active</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastExportTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>deletedTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>marketStatus</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>additionalInformation</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="item_datalayer_services"></a>
### ItemDataLayerResultLookup<a name="item_services_itemdatalayerresultlookup"></a>

ItemDataLayer Lookup


#### Namespace

`Plenty\Modules\Item\DataLayer\Services`





#### Methods

<pre>public <strong>getNumberOfRows</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getResult</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# UnitCombination<a name="item_unitcombination"></a>
    
## Contracts<a name="item_unitcombination_contracts"></a>
### UnitCombinationRepositoryContract<a name="item_contracts_unitcombinationrepositorycontract"></a>

Interface for unit combination


#### Namespace

`Plenty\Modules\Item\UnitCombination\Contracts`





#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Returns all unit combinations
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_unitcombination">UnitCombination</a>
</pre>

    
Returns the unit combination that matches the specified ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
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
    
## Models<a name="item_unitcombination_models"></a>
### UnitCombination<a name="item_models_unitcombination"></a>

The unitCombination model


#### Namespace

`Plenty\Modules\Item\UnitCombination\Models`




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
            <td>The id of the unitCombination</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitId</td>
            <td>The id of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>content</td>
            <td>The content of the unit</td>
        </tr><tr>
            <td><a href="item#item_models_unit">Unit</a>
</td>
            <td>unit</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# SalesPrice<a name="item_salesprice"></a>
    
## Contracts<a name="item_salesprice_contracts"></a>
### SalesPriceSearchRepositoryContract<a name="item_contracts_salespricesearchrepositorycontract"></a>

The contract for the sales price search repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





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



### SalesPriceAccountRepositoryContract<a name="item_contracts_salespriceaccountrepositorycontract"></a>

The contract for the sales price referrer account repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespriceaccount">SalesPriceAccount</a>
</pre>

    
Activates a referrer account for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The account data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $accountType, <a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates a referrer account for a sales price. The ID of the sales price, the type and the ID of the referrer account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountType</td>
        <td>The type of the referrer account linked to the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the referrer account linked to the sales price</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $accountType, <a target="_blank" href="http://php.net/int">int</a> $accountId):<a href="item#item_models_salespriceaccount">SalesPriceAccount</a>
</pre>

    
Gets a referrer account for a sales price. The ID of the sales price, the type and the ID of the referrer account must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountType</td>
        <td>The type of the referrer account linked to the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td>The ID of the referrer account linked to the sales price</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the activated referrer accounts of a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>deleteByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates the referrer accounts for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>



### SalesPriceCountryRepositoryContract<a name="item_contracts_salespricecountryrepositorycontract"></a>

The contract for the sales price country repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespricecountry">SalesPriceCountry</a>
</pre>

    
Activates a country for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price country data as an associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $countryId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates a country for a sales price. The ID of the sales price and the ID of the country must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The unique ID of the <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries"  target="_blank">country</a>; -1 = all countries.</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $countryId):<a href="item#item_models_salespricecountry">SalesPriceCountry</a>
</pre>

    
Gets a country for a sales price. The ID of the sales price and the ID of the country must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The unique ID of the <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries"  target="_blank">country</a>.</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the countries for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>deleteByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes countries from a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
</table>



### SalesPriceOnlineStoreRepositoryContract<a name="item_contracts_salespriceonlinestorerepositorycontract"></a>

The contract for the sales price online store repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespriceonlinestore">SalesPriceOnlineStore</a>
</pre>

    
Activates a client (store) for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The client (store) data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $onlineStoreId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates a client (store) for a sales price. The ID of the sales price and the ID of the client (store) must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$onlineStoreId</td>
        <td>The unique ID of the client (store)</td>
    </tr>
</table>


<pre>public <strong>deleteByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates all clients (stores) for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $onlineStoreId):<a href="item#item_models_salespriceonlinestore">SalesPriceOnlineStore</a>
</pre>

    
Gets client (store) information for a sales price. The ID of the sales price and the ID of the client (store) must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$onlineStoreId</td>
        <td>The ID of the online store</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the active clients (stores) for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>



### SalesPriceRepositoryContract<a name="item_contracts_salespricerepositorycontract"></a>

The contract for the sales price repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>

    
Gets a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>

    
Creates a sales price.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price data as an associative array</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>

    
Updates a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>

    
Gets a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Lists all sales prices.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>An array of the shown columns. All columns are returned by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td>The amount of sales prices shown per page. Default value is 50</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The shown page. Default value is 1</td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### SalesPriceNameRepositoryContract<a name="item_contracts_salespricenamerepositorycontract"></a>

The contract for the sales price name repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespricename">SalesPriceName</a>
</pre>

    
Creates a sales price name. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_salespricename">SalesPriceName</a>
</pre>

    
Updates a sales price name. The ID of the sales price and the language code must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price name data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language code</a> of the sales price name</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a sales price name. The ID of the sales price and the language code must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language code</a> of the sales price name</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_salespricename">SalesPriceName</a>
</pre>

    
Gets a sales price name. The ID of the sales price and the language code must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language code</a> of the sales price name</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all sales price names of a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>



### SalesPriceReferrerRepositoryContract<a name="item_contracts_salespricereferrerrepositorycontract"></a>

The contract for the sales price referrer repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespricereferrer">SalesPriceReferrer</a>
</pre>

    
Activates a referrer for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price referrer data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $referrerId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates a referrer for a sales price. The ID of the sales price and the ID of the referrer must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$referrerId</td>
        <td>The ID of the referrer</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $referrerId):<a href="item#item_models_salespricereferrer">SalesPriceReferrer</a>
</pre>

    
Gets a referrer. The ID of the sales price and the ID of the referrer must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$referrerId</td>
        <td>The ID of the referrer</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all activated referrers of a sales. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>deleteByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates all referrers for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>



### SalesPriceCurrencyRepositoryContract<a name="item_contracts_salespricecurrencyrepositorycontract"></a>

The contract for the sales price currency repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespricecurrency">SalesPriceCurrency</a>
</pre>

    
Activates a currency for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The sales price currency data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/string">string</a> $currency):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates a currency for a sales price. The ID of the sales price and the ISO code of the currency must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#currencies" target="_blank">ISO</a> code of the currency; -1 = all currencies.</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/string">string</a> $currency):<a href="item#item_models_salespricecurrency">SalesPriceCurrency</a>
</pre>

    
Gets a sales price currency. The ID of the sales price and the ISO code of the currency must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#currencies" target="_blank">ISO</a> code of the currency; -1 = all currencies.</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the active currencies of a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>deleteByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates the currencies of a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>



### SalesPriceCustomerClassRepositoryContract<a name="item_contracts_salespricecustomerclassrepositorycontract"></a>

The contract for the sales price customer class repository


#### Namespace

`Plenty\Modules\Item\SalesPrice\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salespricecustomerclass">SalesPriceCustomerClass</a>
</pre>

    
Activates a customer class for a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The customer class data as an associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $customerClassId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates a customer class for a sales price. The ID of the sales price and the ID of the customer class must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$customerClassId</td>
        <td>The unique ID of the customer class</td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $customerClassId):<a href="item#item_models_salespricecustomerclass">SalesPriceCustomerClass</a>
</pre>

    
Gets a customer class for a sales price. The ID of the sales price and the ID of the customer class must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$customerClassId</td>
        <td>The unique ID of the customer class</td>
    </tr>
</table>


<pre>public <strong>findByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists the active customer classes of a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


<pre>public <strong>deleteByPriceId</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivates the customer classes of a sales price. The ID of the sales price must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td>The unique ID of the sales price</td>
    </tr>
</table>


## Models<a name="item_salesprice_models"></a>
### SalesPriceCountry<a name="item_models_salespricecountry"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The unique ID of the <a href="https://developers.plentymarkets.com/rest-doc/introduction#countries"  target="_blank">country</a></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the country was activated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the relationship between country and sales price was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceCurrency<a name="item_models_salespricecurrency"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The ISO code of the <a href="https://developers.plentymarkets.com/rest-doc/introduction#currencies" target="_blank">currency</a>; -1 = all currencies.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the currency was activated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the relationship between currency and sales price was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceAccount<a name="item_models_salespriceaccount"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td>The ID of the referrer linked to the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountId</td>
            <td>The ID of the referrer account linked to the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the referrer account was linked to the sales price.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the link was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceOnlineStore<a name="item_models_salespriceonlinestore"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The unique ID of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the client (store) was activated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the relationship between the client (store) and the sales price was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceSearchResponse<a name="item_models_salespricesearchresponse"></a>

foo


#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>priceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customerClassDiscountPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customerClassDiscount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customerClassDiscountNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryDiscountPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryDiscount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryDiscountNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>interval</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>conversionFactor</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minimumOrderQuantity</td>
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
    

### SalesPriceSearchRequest<a name="item_models_salespricesearchrequest"></a>

foo


#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>variationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerClassId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPrice<a name="item_models_salesprice"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minimumOrderQuantity</td>
            <td>The minimum order quantity of the sales price. Sales prices with different minimum quantities can be used to create a quantity based graduation of prices in plentymarkets.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The price type of the sales price.<ul><li>RRP = Sales price is the recommended retail price (RRP). If the RRP and another sales price are linked with a variation, the RRP will be displayed in the online store as red strike-through text next to the sales price.</li><li>Special offer = Sales price as a special offer. Special offers are used for markets, e.g. Amazon and Hitmeister.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isCustomerPrice</td>
            <td>Flag that indicates if the sales price is a customer price. Currently, this setting is not in use.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isDisplayedByDefault</td>
            <td>Flag that indicates if the sales price is displayed automatically in the Sales Prices area of the plentymarkets backend when a new item is created. When false, the sales price can still be added manually when a new item is created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isLiveConversion</td>
            <td>Flag that indicates if the sales price is converted live in the online store. When true, the default currency price will be converted into the active currencies based on the conversion rates saved in plentymarkets.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>interval</td>
            <td>The interval of the price. Possible values are: daily, weekly, monthly, quarterly, semi-annual and annual.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the sales price was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the sales price was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>names</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>accounts</td>
            <td>accounts</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>countries</td>
            <td>countries</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>currencies</td>
            <td>currencies</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>customerClasses</td>
            <td>customerClasses</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>referrers</td>
            <td>referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>clients</td>
            <td>clients</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceReferrer<a name="item_models_salespricereferrer"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The unique ID of the referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the referrer was activated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the relationship between referrer and sales price was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceCustomerClass<a name="item_models_salespricecustomerclass"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerClassId</td>
            <td>The unique ID of the customer class</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the customer class was activated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the relationship between customer class and sales price was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesPriceName<a name="item_models_salespricename"></a>




#### Namespace

`Plenty\Modules\Item\SalesPrice\Models`




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
            <td>salesPriceId</td>
            <td>The unique ID of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language code</a> of the sales price name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>nameInternal</td>
            <td>The internal name of the sales price. The internal name is used in the plentymarkets back end only.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>nameExternal</td>
            <td>The external name of the sales price. The external name is displayed in the online store and as such is visible for customers.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the name was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the name was last updated.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# VariationClient<a name="item_variationclient"></a>
    
## Contracts<a name="item_variationclient_contracts"></a>
### VariationClientRepositoryContract<a name="item_contracts_variationclientrepositorycontract"></a>

The contract of the variation client repository


#### Namespace

`Plenty\Modules\Item\VariationClient\Contracts`





#### Methods

<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationclient">VariationClient</a>
</pre>

    
Gets a client (store) linked to a variation. The ID of the variation and the client ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The unique ID of the client (store)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationclient">VariationClient</a>
</pre>

    
Creates a link between a variation and a client (store).
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The variation client data as an associative array</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes the link between a variation and a client (store). The ID of the variation and the client ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The unique ID of the client (store)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationclient">VariationClient</a>
</pre>

    
Lists the clients (stores) linked to a variation. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationclient">VariationClient</a>
</pre>

    
Lists the clients (stores) linked to a variation including inheritance information. The ID of the variation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The unique ID of the variation</td>
    </tr>
</table>


## Models<a name="item_variationclient_models"></a>
### VariationClient<a name="item_models_variationclient"></a>

Variation Client


#### Namespace

`Plenty\Modules\Item\VariationClient\Models`




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
            <td>variationId</td>
            <td>The unique ID of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The unique ID of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time at which the client (store) was linked to the variation.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
