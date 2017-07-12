

# Stock<a name="stockmanagement_stock"></a>
    
## Contracts<a name="stockmanagement_stock_contracts"></a>
### StockRepositoryContract<a name="stockmanagement_contracts_stockrepositorycontract"></a>

The StockRepositoryContract is the interface for the stock repository. This interface allows you to find, create and update stock. Stock is assigned to one variation and is stored in warehouses.


#### Namespace

`Plenty\Modules\StockManagement\Stock\Contracts`



#### Methods

<pre>public <strong>listStockByWarehouseId</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List stock of a warehouse
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The ID of the warehouse</td>
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


<pre>public <strong>listStock</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>listStockByWarehouseType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List stock by warehouse type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of the warehouse. Currently only 'sales' is supported.</td>
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


<pre>public <strong>correctStock</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Corrects stock. The ID of the warehouse has to be provided.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The ID of the warehouse.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data.</td>
    </tr>
</table>


<pre>public <strong>bookIncomingItems</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Book incoming stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The ID of the warehouse</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request date</td>
    </tr>
</table>


<pre>public <strong>redistributeStock</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Redistribute stock
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>listStockMovements</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List stock movements
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The ID of the warehouse</td>
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
    

### StockStorageLocationRepositoryContract<a name="stockmanagement_contracts_stockstoragelocationrepositorycontract"></a>

The StockStorageLocationRepositoryContract is the interface for the stock storage location repository. This interface allows you to list the stock of all storage locations of a warehouse or to list all storage locations of a variation and the stock stored at these locations.


#### Namespace

`Plenty\Modules\StockManagement\Stock\Contracts`



#### Methods

<pre>public <strong>listStockStorageLocationsByWarehouseId</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List stock of all storage locations of a warehouse
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The ID of the warehouse</td>
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


<pre>public <strong>listStockStorageLocationsByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List stock of a variation per storage location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td>The ID of the variation.</td>
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
    
## Models<a name="stockmanagement_stock_models"></a>
### Stock<a name="stockmanagement_models_stock"></a>

The stock model. There are 4 different stock terms used in plentymarkets. The physical stock, the net stock, the reserved stock and the stock reserved for listings.


#### Namespace

`Plenty\Modules\StockManagement\Stock\Models`


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
            <td>stockPhysical</td>
            <td>The physical stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedStock</td>
            <td>The reserved stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedEbay</td>
            <td>The stock reserved for ebay</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reorderDelta</td>
            <td>The reorder delta</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>stockNet</td>
            <td>The net stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reordered</td>
            <td>The reordered quantity of a variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedBundle</td>
            <td>Reserved bundle</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>averagePurchasePrice</td>
            <td>The average purchase price</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The time the stock was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### StockStorageLocation<a name="stockmanagement_models_stockstoragelocation"></a>

The stock storage location model contains all information about the stock that is stored at one storage location.


#### Namespace

`Plenty\Modules\StockManagement\Stock\Models`


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
            <td>storageLocationId</td>
            <td>The ID of the storage location.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The ID of the warehouse that the storage location is in</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>quantity</td>
            <td>The quantity stored at the storage location</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The day and time the stock was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Warehouse<a name="stockmanagement_warehouse"></a>
    
## Contracts<a name="stockmanagement_warehouse_contracts"></a>
### WarehouseRepositoryContract<a name="stockmanagement_contracts_warehouserepositorycontract"></a>

The WarehouseRepositoryContract is the interface for the warehouse repository. This interface allows you to either get one warehouse by specifying the id or to list all warehouses.


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Contracts`



#### Methods

<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="stockmanagement#stockmanagement_models_warehouse">Warehouse</a>
</pre>

    
Get a warehouse
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The id of the warehouse.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the warehouse instance. repairWarehouse is the only relation currently available.</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List warehouses
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the warehouse instance. repairWarehouse is the only relation currently available.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="stockmanagement#stockmanagement_models_warehouse">Warehouse</a>
</pre>

    
Create a warehouse
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data.</td>
    </tr>
</table>


## Models<a name="stockmanagement_warehouse_models"></a>
### Warehouse<a name="stockmanagement_models_warehouse"></a>

The warehouse model in plentymarkets represents actual warehouses. Every warehouse is identified by an Id. Furthermore a warehouse is described by a name and is always associated with an address. This address may not only contain a physical address information like a street, a house number, a postal code and a town, but also an email address, a telephone number or a fax number.


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Models`


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
            <td>The id of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>note</td>
            <td>A note for this warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The id of the warehouse type. The following types are available:
<ul>
    <li>0 = Sales warehouse</li>
    <li>1 = Repair warehouse</li>
    <li>4 = Storage warehouse</li>
    <li>5 = Transit warehouse</li>
    <li>6 = Distribution warehouse</li>
    <li>7 = Other</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>onStockAvailability</td>
            <td>Displayed availability of a variation if stock is available</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>outOfStockAvailability</td>
            <td>Displayed availability of a variation if no stock is available</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>splitByShippingProfile</td>
            <td>Flag that indicates if for this warehouse orders are split by shipping profiles or not. <ul><li>True = Orders are split by shipping profiles</li> <li>False = Orders will not be split by shipping profiles</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationType</td>
            <td>The storage location type. The following types are available: <ul><li>none</li> <li>small</li><li>medium</li> <li>large</li> <li>europallet</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storageLocationZone</td>
            <td>The zone that the storage location is in</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>repairWarehouseId</td>
            <td>The id of the associated repair warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isInventoryModeActive</td>
            <td>Flag that indicates if the inventory mode for this warehouse is active or not. <ul><li>True = active</li> <li>False = inactive</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>logisticsType</td>
            <td>The id of the logistics type of the warehouse. The logistics type states which service provider fulfills the storage and shipping. The following logistics types are available:
<ul>
<li>own</li>
<li>amazon</li>
<li>dhlFulfillment</li>
</ul></td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>address</td>
            <td>The address that the warehouse is located at</td>
        </tr><tr>
            <td><a href="stockmanagement#stockmanagement_models_warehouse">Warehouse</a>
</td>
            <td>repairWarehouse</td>
            <td>All information about the repair warehouse if a repair warehouse is linked to the sales warehouse</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Management<a name="stockmanagement_management"></a>
    
## Contracts<a name="stockmanagement_management_contracts"></a>
### RackManagementRepositoryContract<a name="stockmanagement_contracts_rackmanagementrepositorycontract"></a>

The RackManagementRepositoryContract is the interface for the rack management repository. This interface provides the functionality to manage the warehouse configuration for racks. Racks can be retrieved, created or updated here.


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Management\Contracts`



#### Methods

<pre>public <strong>getRackById</strong>(<a target="_blank" href="http://php.net/int">int</a> $rackId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="stockmanagement#stockmanagement_models_rack">Rack</a>
</pre>

    
Find a rack by id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rackId</td>
        <td>The id of the rack.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded. Possible values are 'warehouse', 'shelves' and 'storageLocations'.</td>
    </tr>
</table>


<pre>public <strong>findRacks</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Find racks. The results can be filtered by warehouse id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The requested page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>Number of items per page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded. Possible values are 'warehouse', 'shelves' and 'storageLocations'.</td>
    </tr>
</table>


<pre>public <strong>createRack</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $warehouseId):<a href="stockmanagement#stockmanagement_models_rack">Rack</a>
</pre>

    
Create a new rack.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data to create a new rack.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The id of the warehouse the rack shall belong to.</td>
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
    

### ShelfManagementRepositoryContract<a name="stockmanagement_contracts_shelfmanagementrepositorycontract"></a>

The ShelfManagementRepositoryContract is the interface for the shelf management repository. This interface provides the functionality to manage the warehouse configuration for shelves. Shelves can be retrieved, created or updated here.


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Management\Contracts`



#### Methods

<pre>public <strong>getShelfById</strong>(<a target="_blank" href="http://php.net/int">int</a> $shelfId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="stockmanagement#stockmanagement_models_shelf">Shelf</a>
</pre>

    
Find a shelf by id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shelfId</td>
        <td>The id of the shelf.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded. Possible values are 'warehouse', 'rack' and 'storageLocations'.</td>
    </tr>
</table>


<pre>public <strong>findShelves</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Find shelves. The results can be filtered by warehouse id and rack id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The requested page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>Number of items per page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded. Possible values are 'warehouse', 'rack' and 'storageLocations'.</td>
    </tr>
</table>


<pre>public <strong>createShelf</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/int">int</a> $rackId):<a href="stockmanagement#stockmanagement_models_shelf">Shelf</a>
</pre>

    
Create a new shelf.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data to create a new shelf.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The id of the warehouse the shelf shall belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rackId</td>
        <td>The id of the rack the shelf shall belong to.</td>
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
    

### StorageLocationManagementRepositoryContract<a name="stockmanagement_contracts_storagelocationmanagementrepositorycontract"></a>

The StorageLocationManagementRepositoryContract is the interface for the storage location management repository. This interface provides the functionality to manage the warehouse configuration for storage locations. Storage locations can be retrieved, created or updated here.


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Management\Contracts`



#### Methods

<pre>public <strong>getStorageLocationById</strong>(<a target="_blank" href="http://php.net/int">int</a> $storageLocationId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="stockmanagement#stockmanagement_models_storagelocation">StorageLocation</a>
</pre>

    
Find a storage location by id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$storageLocationId</td>
        <td>The id of the storage location.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded. Possible values are 'warehouse', 'rack' and 'shelf'.</td>
    </tr>
</table>


<pre>public <strong>findStorageLocations</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Find storage locations. The results can be filtered by warehouse id, rack id and shelf id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The requested page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>Number of items per page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded. Possible values are 'warehouse', 'rack' and 'shelf'.</td>
    </tr>
</table>


<pre>public <strong>createStorageLocation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/int">int</a> $rackId, <a target="_blank" href="http://php.net/int">int</a> $shelfId):<a href="stockmanagement#stockmanagement_models_storagelocation">StorageLocation</a>
</pre>

    
Create a new storage location.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data to create a new storage location.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td>The id of the warehouse the storage location shall belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rackId</td>
        <td>The id of the rack the storage location shall belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shelfId</td>
        <td>The id of the shelf the storage location shall belong to.</td>
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
    
## Models<a name="stockmanagement_management_models"></a>
### Rack<a name="stockmanagement_models_rack"></a>

The storage rack model


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Management\Models`


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
            <td>The id of the rack.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>name</td>
            <td>The name of the rack.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the rack.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The id of the warehouse the rack belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>zone</td>
            <td>The zone of the rack. Numbers between 1 and 20 are valid.</td>
        </tr><tr>
            <td><a href="stockmanagement#stockmanagement_models_warehouse">Warehouse</a>
</td>
            <td>warehouse</td>
            <td>The warehouse this rack belongs to.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>shelves</td>
            <td>The shelves that belong to this rack.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>storageLocations</td>
            <td>The storage locations that belong to this rack.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Shelf<a name="stockmanagement_models_shelf"></a>

The storage shelf model


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Management\Models`


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
            <td>The id of the shelf.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rackId</td>
            <td>The id of the rack the shelf belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the shelf.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>level</td>
            <td>The level of the shelf. Numbers between 1 and 25 are valid.</td>
        </tr><tr>
            <td><a href="stockmanagement#stockmanagement_models_rack">Rack</a>
</td>
            <td>rack</td>
            <td>The rack this shelf belongs to.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>storageLocations</td>
            <td>The storage locations of this shelf.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### StorageLocation<a name="stockmanagement_models_storagelocation"></a>

The storage location model


#### Namespace

`Plenty\Modules\StockManagement\Warehouse\Management\Models`


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
            <td>The id of the storage location.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The id of the warehouse the storage location belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rackId</td>
            <td>The id of the rack the storage location belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shelfId</td>
            <td>The id of the shelf the storage location belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the storage location.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>type</td>
            <td>The type of the storage location. Valid strings are: 'small', 'medium', 'large', 'europallet'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the storage location.</td>
        </tr><tr>
            <td><a href="stockmanagement#stockmanagement_models_warehouse">Warehouse</a>
</td>
            <td>warehouse</td>
            <td>The warehouse this storage location belongs to.</td>
        </tr><tr>
            <td><a href="stockmanagement#stockmanagement_models_rack">Rack</a>
</td>
            <td>rack</td>
            <td>The rack this storage location belongs to.</td>
        </tr><tr>
            <td><a href="stockmanagement#stockmanagement_models_shelf">Shelf</a>
</td>
            <td>shelf</td>
            <td>The shelf this storage location belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
