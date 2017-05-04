

# DeleteLog<a name="deletelog_deletelog"></a>
    
## Contracts<a name="deletelog_deletelog_contracts"></a>
### DeleteLogRepositoryContract<a name="deletelog_contracts_deletelogrepositorycontract"></a>

List delete log entries.


#### Namespace

`Plenty\Modules\DeleteLog\Contracts`



#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List delete log entries
    
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
    
## Models<a name="deletelog_deletelog_models"></a>
### DeleteLog<a name="deletelog_models_deletelog"></a>

The delete log model


#### Namespace

`Plenty\Modules\DeleteLog\Models`


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
            <td>referenceType</td>
            <td>The type of the deleted record<ul><li>1 = Category</li><li>2 = Payment</li><li>3 = Order</li><li>4 = Customer</li><li>5 = Item</li><li>6 = Facet of the type Attribute</li><li>7 = Facet of the type Property</li><li>8 = Facet of the type Manufacturer</li><li>9 = Facet of the type Availability</li><li>10 = Unit</li><li>11 = Sales price</li><li>12 = Sales price link to variation</li><li>13 = Item variation</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referenceValue</td>
            <td>The ID of the deleted record</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>userRealName</td>
            <td>The real name of the user who deleted the record</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The date and time that the record was deleted</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the user who deleted the record</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
