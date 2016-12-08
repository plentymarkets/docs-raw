

# ItemSet<a name="itemset_itemset"></a>
    
## Contracts<a name="itemset_itemset_contracts"></a>
### ItemSetComponentRepositoryContract<a name="itemset_contracts_itemsetcomponentrepositorycontract"></a>

The contract for the item set component repository


#### Namespace

`Plenty\Modules\ItemSet\Contracts`



#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with):<a href="itemset#itemset_models_itemsetcomponent">ItemSetComponent</a>
</pre>

    
Return item set component by given id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="itemset#itemset_models_itemsetcomponent">ItemSetComponent</a>
</pre>

    
Return item set component by given set id and id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/int">int</a> $setConfigId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemsetcomponent">ItemSetComponent</a>
</pre>

    
Create a new item set component
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setConfigId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createComponents</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemsetcomponent">ItemSetComponent</a>
</pre>

    
Create new item set components
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateComponents</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemsetcomponent">ItemSetComponent</a>
</pre>

    
Update item set components
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemsetcomponent">ItemSetComponent</a>
</pre>

    
Update one item set component by given setId and id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
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


<pre>public <strong>deleteComponents</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete item set components
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete item set component by given setId and id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Return all item set components
    
<pre>public <strong>findBySetId</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/array">array</a> $with):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>



### ItemSetConfigRepositoryContract<a name="itemset_contracts_itemsetconfigrepositorycontract"></a>

The contract for the item set config repository


#### Namespace

`Plenty\Modules\ItemSet\Contracts`



#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="itemset#itemset_models_itemsetconfig">ItemSetConfig</a>
</pre>

    
Return item set by given id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemsetconfig">ItemSetConfig</a>
</pre>

    
Create new item set config
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemsetconfig">ItemSetConfig</a>
</pre>

    
Update item set config by given id
    
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


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete item set config by given id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $setConfigId):<a href="itemset#itemset_models_itemsetconfig">ItemSetConfig</a>
</pre>

    
Return item set config of item set
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setConfigId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findBySetId</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId):<a href="itemset#itemset_models_itemsetconfig">ItemSetConfig</a>
</pre>

    
Return set config for item set
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
</table>



### ItemSetRepositoryContract<a name="itemset_contracts_itemsetrepositorycontract"></a>

The contract for the item set repository


#### Namespace

`Plenty\Modules\ItemSet\Contracts`



#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="itemset#itemset_models_itemset">ItemSet</a>
</pre>

    
Return item set by given id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemset">ItemSet</a>
</pre>

    
Create new item set
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createSets</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemset">ItemSet</a>
</pre>

    
Create new item sets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateSets</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Update existing item sets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="itemset#itemset_models_itemset">ItemSet</a>
</pre>

    
Update item set by given id
    
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


<pre>public <strong>deleteSets</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete item sets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete item set config by given id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Return all item set configs
    
## Models<a name="itemset_itemset_models"></a>
### ItemSet<a name="itemset_models_itemset"></a>

The ItemSet model.


#### Namespace

`Plenty\Modules\ItemSet\Models`


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
            <td>The item ID of the item set. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the item set. The default language of the system is used.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>categories</td>
            <td>The array with categories of the item set. The category ID key  "categoryId" must be specified. Example for JSON Object:  "categories":[{"categoryId":"34"},{"categoryId":"35"}]}]</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemSetComponent<a name="itemset_models_itemsetcomponent"></a>

The ItemSetComponent model.


#### Namespace

`Plenty\Modules\ItemSet\Models`


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
            <td>The item set component ID. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>setId</td>
            <td>set id The item ID of the item set. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The item ID of the set component</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The number of copies of the component that are part of the set. Default quantity is 1.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPurchasable</td>
            <td>Flag that indicates if enough stock is available for at least one variation of the component to cover the specified quantity.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ItemSetConfig<a name="itemset_models_itemsetconfig"></a>

The ItemSetConfig model.


#### Namespace

`Plenty\Modules\ItemSet\Models`


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
            <td>setId</td>
            <td>set id The item ID of the item set. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>rebate</td>
            <td>The discount in percent to be subtracted from the sum of the prices of the selected set components.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minPrice</td>
            <td>The minimum price of the sum of all components; read only</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>maxPrice</td>
            <td>the maximum price of the sum of all components; read only</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isPurchasable</td>
            <td>Flag that indicates if all components of the set have sufficient stock. Purchasability of a set depends on the component with the lowest stock.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
