

# Warehouse<a name="warehouse_warehouse"></a>
    
## Contracts<a name="warehouse_warehouse_contracts"></a>
### WarehouseLocationRepositoryContract<a name="warehouse_contracts_warehouselocationrepositorycontract"></a>

Get, create, update and delete warehouse locations


#### Namespace

`Plenty\Modules\Warehouse\Contracts`





#### Methods

<pre>public <strong>getWarehouseLocation</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocation):<a href="warehouse#warehouse_models_warehouselocation">WarehouseLocation</a>
</pre>

    
Get a warehouse location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listWarehouseLocations</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $paginate = 1, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $warehouseId = null):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Get all warehouse locations
    
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
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getWarehouseLocationByLabel</strong>(<a target="_blank" href="http://php.net/string">string</a> $label):<a href="warehouse#warehouse_models_warehouselocation">WarehouseLocation</a>
</pre>

    
Get first warehouse location matching the given label
Gets the first warehouse location matching the given label. The label must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$label</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createWarehouseLocation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="warehouse#warehouse_models_warehouselocation">WarehouseLocation</a>
</pre>

    
Create a warehouse location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateWarehouseLocation</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocation, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="warehouse#warehouse_models_warehouselocation">WarehouseLocation</a>
</pre>

    
Update a warehouse location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocation</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteWarehouseLocation</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocation):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a warehouse location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteMultipleWarehouseLocations</strong>(<a target="_blank" href="http://php.net/array">array</a> $warehouseLocationIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete multiple warehouse locations
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$warehouseLocationIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>executeGroupFunction</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Edit the purpose and status for a group of storage locations
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateWarehouseLocationLabel</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId, <a target="_blank" href="http://php.net/array">array</a> $warehouseLocationIds):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Generate warehouse location labels
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$warehouseLocationIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>moveWarehouseLocationPosition</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Move a warehouse location position
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
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
    

### WarehouseLocationLevelRepositoryContract<a name="warehouse_contracts_warehouselocationlevelrepositorycontract"></a>

Get, create, update and delete warehouse location levels


#### Namespace

`Plenty\Modules\Warehouse\Contracts`





#### Methods

<pre>public <strong>getWarehouseLocationLevel</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocationLevel):<a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</pre>

    
Get a warehouse location level
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocationLevel</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getWarehouseLocationLevelByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $warehouseLocationLevelName, <a target="_blank" href="http://php.net/int">int</a> $dimensionId, <a target="_blank" href="http://php.net/int">int</a> $parentId):<a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</pre>

    
Get a warehouse location level
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$warehouseLocationLevelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$dimensionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parentId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getWarehouseLocationLevelOnlyByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $warehouseLocationLevelName):<a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</pre>

    
Get a warehouse location level only by name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$warehouseLocationLevelName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listWarehouseLocationLevels</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $warehouseId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a list of warehouse location levels
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createWarehouseLocationLevel</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/bool">bool</a> $apiMode = false):<a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</pre>

    
Create a warehouse location level
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$apiMode</td>
        <td>If the location is created using a route</td>
    </tr>
</table>


<pre>public <strong>updateWarehouseLocationLevel</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocationLevel, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</pre>

    
Update a warehouse location level
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocationLevel</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteWarehouseLocationLevel</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocationLevel):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a warehouse location level
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocationLevel</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getWarehouseStructure</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a warehouse structure.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>moveWarehouseLocationLevelPosition</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Move a warehouse location level position
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
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
    

### WarehouseLocationDimensionRepositoryContract<a name="warehouse_contracts_warehouselocationdimensionrepositorycontract"></a>

Get, create, update and delete warehouse location dimensions


#### Namespace

`Plenty\Modules\Warehouse\Contracts`





#### Methods

<pre>public <strong>getWarehouseLocationDimension</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocationDimension, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="warehouse#warehouse_models_warehouselocationdimension">WarehouseLocationDimension</a>
</pre>

    
Get a warehouse location dimension
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocationDimension</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listWarehouseLocationDimension</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseId):<a href="warehouse#warehouse_models_warehouselocationdimension">WarehouseLocationDimension</a>
</pre>

    
Get all warehouse location dimensions
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createMultipleWarehouseLocationDimension</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Create multiple warehouse location dimensions
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>createWarehouseLocationDimension</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="warehouse#warehouse_models_warehouselocationdimension">WarehouseLocationDimension</a>
</pre>

    
Create a warehouse location dimension
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateWarehouseLocationDimension</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocationDimension, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="warehouse#warehouse_models_warehouselocationdimension">WarehouseLocationDimension</a>
</pre>

    
Update a warehouse location dimension
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocationDimension</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteWarehouseLocationDimension</strong>(<a target="_blank" href="http://php.net/int">int</a> $warehouseLocationDimension):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a warehouse location dimension
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$warehouseLocationDimension</td>
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
    
## Models<a name="warehouse_warehouse_models"></a>
### WarehouseLocationDimension<a name="warehouse_models_warehouselocationdimension"></a>

The warehouse location dimension model.


#### Namespace

`Plenty\Modules\Warehouse\Models`




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
            <td>The ID of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentId</td>
            <td>The parent ID of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The warehouse ID of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>level</td>
            <td>The level of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortcut</td>
            <td>The shortcut of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>separator</td>
            <td>The separator of the warehouse location dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayInName</td>
            <td>If true, the dimension prefix will be shown in the storage location name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isActiveForPickupPath</td>
            <td>Active flag for pickup path of the warehouse location dimension</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>Date when the warehouse location dimension was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>Date when the warehouse location dimension was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>warehouseLocationLevel</td>
            <td>The linked warehouse location level</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WarehouseLocationLevel<a name="warehouse_models_warehouselocationlevel"></a>

The warehouse location level model.


#### Namespace

`Plenty\Modules\Warehouse\Models`




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
            <td>The ID of the warehouse location level</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentId</td>
            <td>The parent ID of the warehouse location level</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>dimensionId</td>
            <td>The warehouse location dimension id of the warehouse location level</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the warehouse location level</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the warehouse location level</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the warehouse location ['small','medium','large','europallet']</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pathName</td>
            <td>The complete path name from the level</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the warehouse location level was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the warehouse location level was last updated</td>
        </tr><tr>
            <td><a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</td>
            <td>parent</td>
            <td>The parent warehouse location level if existing</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>children</td>
            <td>The children warehouse location level if existing</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>warehouseLocation</td>
            <td>The linked warehouse location</td>
        </tr><tr>
            <td><a href="warehouse#warehouse_models_warehouselocationdimension">WarehouseLocationDimension</a>
</td>
            <td>warehouseLocationDimension</td>
            <td>The linked warehouse location dimension</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WarehouseLocation<a name="warehouse_models_warehouselocation"></a>

The warehouse location model.


#### Namespace

`Plenty\Modules\Warehouse\Models`




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
            <td>The ID of the warehouse location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>levelId</td>
            <td>The level ID of the warehouse location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>label</td>
            <td>The label of the warehouse location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>purposeKey</td>
            <td>The purpose key of the warehouse location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>statusKey</td>
            <td>The status key of the warehouse location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the warehouse location</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fullLabel</td>
            <td>The label with level path name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the warehouse location (array values: 'small','medium','large','europallet')</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>notes</td>
            <td>The notes of the warehouse location</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the warehouse location was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the warehouse location was last updated</td>
        </tr><tr>
            <td><a href="warehouse#warehouse_models_warehouselocationlevel">WarehouseLocationLevel</a>
</td>
            <td>warehouseLocationLevel</td>
            <td>The level from warehouse location.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
