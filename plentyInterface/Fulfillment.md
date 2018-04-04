

# Picklist<a name="fulfillment_picklist"></a>
    
## Contracts<a name="fulfillment_picklist_contracts"></a>
### PickingOrderItemRepositoryContract<a name="fulfillment_contracts_pickingorderitemrepositorycontract"></a>

The PickingOrderItemRepositoryContract


#### Namespace

`Plenty\Modules\Fulfillment\Picklist\Contracts`





#### Methods

<pre>public <strong>getAll</strong>():<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    

    
<pre>public <strong>getPickingOrderItemById</strong>(<a target="_blank" href="http://php.net/int">int</a> $pickingOrderItemId):<a href="fulfillment#fulfillment_models_pickingorderitem">PickingOrderItem</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pickingOrderItemId</td>
        <td></td>
    </tr>
</table>


## Events<a name="fulfillment_picklist_events"></a>
### GetPickingItemConfig<a name="fulfillment_events_getpickingitemconfig"></a>

This event will be triggered, when an item is picked


#### Namespace

`Plenty\Modules\Fulfillment\Picklist\Events`





#### Methods

<pre>public <strong>getPickingOrderItemId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getProcessUserId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>addPluginConfig</strong>(<a target="_blank" href="http://php.net/string">string</a> $identifier, $pluginConfig):<a href="fulfillment#fulfillment_picklist_events">Events</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$identifier</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$pluginConfig</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPluginConfigs</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
## Models<a name="fulfillment_picklist_models"></a>
### PickingOrderItem<a name="fulfillment_models_pickingorderitem"></a>

PickingOrderItem


#### Namespace

`Plenty\Modules\Fulfillment\Picklist\Models`




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
            <td>pickingOrderId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderItemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>processState</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>processDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>processUserId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>comment</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>quantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>holdingArea</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderIdList</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
