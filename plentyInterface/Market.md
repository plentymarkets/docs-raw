

# PartsFitment<a name="market_partsfitment"></a>
    
## Contracts<a name="market_partsfitment_contracts"></a>
### FitmentItemPropertyRepositoryContract<a name="market_contracts_fitmentitempropertyrepositorycontract"></a>

The contract for the fitment item property repository.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitemproperty">FitmentItemProperty</a>
</pre>
    
Returns a fitment item property by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item property that should be found.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitemproperty">FitmentItemProperty</a>
</pre>
    
Creates a new fitment item property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item property data as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The fitment item ID that the current property should belong to.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>
    
Updates an existing fitment item property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item property data to update as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item property that should be updated.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Deletes a fitment item property. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item property that should be deleted.</td>
    </tr>
</table>



### FitmentItemRepositoryContract<a name="market_contracts_fitmentitemrepositorycontract"></a>

The contract for the fitment item repository.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>
    
Returns a fitment item by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The id of the fitment item that should be found.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>
    
Creates a new fitment item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item data as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that the current fitment item belongs to.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitmentitem">FitmentItem</a>
</pre>
    
Updates an existing fitment item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment item data to update as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item that should be updated.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Deletes a fitment item. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment item that should be deleted.</td>
    </tr>
</table>



### FitmentRepositoryContract<a name="market_contracts_fitmentrepositorycontract"></a>

The contract for the fitment repository.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitment">Fitment</a>
</pre>
    
Returns a fitment by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be found.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="market#market_models_fitment">Fitment</a>
</pre>
    
Creates a new fitment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment data as associative array.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitment">Fitment</a>
</pre>
    
Updates an existing fitment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The fitment data to update as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be updated.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Deletes a fitment. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be deleted.</td>
    </tr>
</table>


<pre>public <strong>pushSortingOrder</strong>(<a target="_blank" href="http://php.net/string">string</a> $field, <a target="_blank" href="http://php.net/string">string</a> $direction = &quot;asc&quot;):<a href="miscellaneous#miscellaneous_repositories_contracts">Contracts</a>
</pre>
    
Pushes a sorting order to a collection.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$direction</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>applySortingOrder</strong>():<a href="miscellaneous#miscellaneous_repositories_contracts">Contracts</a>
</pre>
    
Applies the sorting order on the underlying builder instance
    
<pre>public <strong>clearSortingOrder</strong>():<a href="miscellaneous#miscellaneous_repositories_contracts">Contracts</a>
</pre>
    
Clears the sorting order on the underlying builder instance
    
## Models<a name="market_partsfitment_models"></a>
### Fitment<a name="market_models_fitment"></a>

The fitment model. This can contain multiple FitmentItems models.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Models`


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
            <td>The id of the fitment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketId</td>
            <td>The id of the market the fitment belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the fitment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryId</td>
            <td>The id of the category the fitment belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>items</td>
            <td>The list of the items that belong to the fitment.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### FitmentItem<a name="market_models_fitmentitem"></a>

The fitment item model. This belongs to one fitment model and can contain multiple FitmentItemProperty models.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Models`


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
            <td>The id of the item that belongs to the fitment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>fitmentId</td>
            <td>The id of the fitment.</td>
        </tr><tr>
            <td><a href="market#market_models_fitment">Fitment</a>
</td>
            <td>fitment</td>
            <td>The fitment this fitment item belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>properties</td>
            <td>A collection of this fitment item properties.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### FitmentItemProperty<a name="market_models_fitmentitemproperty"></a>

The fitment item property model. This bleongs to an FitmentItem model.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Models`


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
            <td>The ID of the fitment item property.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>fitmentItemId</td>
            <td>The ID that the fitment item this property belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property.</td>
        </tr><tr>
            <td><a href="market#market_models_fitmentitem">FitmentItem</a>
</td>
            <td>fitmentItem</td>
            <td>The fitment item this property belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
