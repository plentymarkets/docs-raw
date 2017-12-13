

# RelationReference<a name="order_relationreference"></a>
    
## Contracts<a name="order_relationreference_contracts"></a>
### OrderRelationReferenceRepositoryContract<a name="order_contracts_orderrelationreferencerepositorycontract"></a>

Get, create, update and delete order relation references.


#### Namespace

`Plenty\Modules\Order\RelationReference\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderrelationreference">OrderRelationReference</a>
</pre>

    
Get a relation reference by ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the relation reference</td>
    </tr>
</table>


<pre>public <strong>findByComposite</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $referenceType, <a target="_blank" href="http://php.net/string">string</a> $relation):<a href="order#order_models_orderrelationreference">OrderRelationReference</a>
</pre>

    
Get a relation reference by composite key
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The reference type. Valid types are:
<ul>
	<li>contact</li>
	<li>warehouse</li>
	<li>account</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relation</td>
        <td>The relation. Valid relations are:
<ul>
	<li>sender</li>
	<li>receiver</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>findByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List relation references by order ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>findByAnyValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List relation references by any values
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>The array with the given filter values. E.g. ['referenceType' => 'contact']. Valid filters are:
<ul>
	<li>id</li>
	<li>orderId</li>
	<li>referenceType</li>
	<li>referenceId</li>
	<li>relation</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The items per page</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_orderrelationreference">OrderRelationReference</a>
</pre>

    
Create a relation reference
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_orderrelationreference">OrderRelationReference</a>
</pre>

    
Update a relation reference by ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the relation reference</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateByComposite</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $referenceType, <a target="_blank" href="http://php.net/string">string</a> $relation, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_orderrelationreference">OrderRelationReference</a>
</pre>

    
Update a relation reference by composite key
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The reference type. Valid types are:
<ul>
	<li>contact</li>
	<li>warehouse</li>
	<li>account</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relation</td>
        <td>The relation. Valid relations are:
<ul>
	<li>sender</li>
	<li>receiver</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a relation reference by ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the relation reference</td>
    </tr>
</table>


<pre>public <strong>deleteByComposite</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $referenceType, <a target="_blank" href="http://php.net/string">string</a> $relation):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a relation reference by composite key
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The reference type. Valid types are:
<ul>
	<li>contact</li>
	<li>warehouse</li>
	<li>account</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relation</td>
        <td>The relation. Valid relations are:
<ul>
	<li>sender</li>
	<li>receiver</li>
</ul></td>
    </tr>
</table>


## Models<a name="order_relationreference_models"></a>
### OrderRelationReference<a name="order_models_orderrelationreference"></a>

The order relation reference model specifies how references and orders are related to one another.


#### Namespace

`Plenty\Modules\Order\RelationReference\Models`


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
            <td>The relation reference id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The order id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceType</td>
            <td>The reference type.
                                         The reference types available are the following:
<ul>
<li>contact</li>
<li>account</li>
<li>warehouse</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referenceId</td>
            <td>The reference id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relation</td>
            <td>The relation between a reference and an order.
                                         The relation types available are the following:
<ul>
<li>sender</li>
<li>receiver</li>
</ul></td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order that the reference belongs to.</td>
        </tr><tr>
            <td><a href="account#account_models_contact">Contact</a>
</td>
            <td>contactReceiver</td>
            <td>The Contact referenced with relation "receiver".</td>
        </tr><tr>
            <td><a href="account#account_models_contact">Contact</a>
</td>
            <td>contactSender</td>
            <td>The Contact referenced with relation "sender".</td>
        </tr><tr>
            <td><a href="account#account_models_account">Account</a>
</td>
            <td>accountReceiver</td>
            <td>The Account referenced with relation "receiver".</td>
        </tr><tr>
            <td><a href="account#account_models_account">Account</a>
</td>
            <td>accountSender</td>
            <td>The Account referenced with relation "sender".</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Property<a name="order_property"></a>
    
## Contracts<a name="order_property_contracts"></a>
### OrderItemPropertyRepositoryContract<a name="order_contracts_orderitempropertyrepositorycontract"></a>

The OrderItemPropertyRepositoryContract contains the functionality to find, create, update and delete OrderItemProperty instances.


#### Namespace

`Plenty\Modules\Order\Property\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Find an order item property by its ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order item property.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Create an order item property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item property data. The properties that are required to create an order item can be found in the OrderItemProperty model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Update an order item property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item property data. The properties that are required to create an order item can be found in the OrderItemProperty model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order item property</td>
    </tr>
</table>


<pre>public <strong>save</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Create or update an order item property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item property data. The properties that are required to create an order can be found in the OrderItemProperty model.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order item property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order item property</td>
    </tr>
</table>


<pre>public <strong>findByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Get an order item property by an order item ID and an order property type ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the property type</td>
    </tr>
</table>


<pre>public <strong>createByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Create an order item property by an order item ID and an order property type ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item property data. The properties that are required to create an order can be found in the OrderItemProperty model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the property type</td>
    </tr>
</table>


<pre>public <strong>updateByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderitemproperty">OrderItemProperty</a>
</pre>

    
Update an order item property by an order item ID and an order property type ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item property data. The properties that are required to create an order can be found in the OrderItemProperty model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the property type</td>
    </tr>
</table>


<pre>public <strong>deleteByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order item property by an order item ID and an order property type ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the property type</td>
    </tr>
</table>


<pre>public <strong>findByOrderItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List order item properties of an order item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order</td>
    </tr>
</table>



### OrderPropertyRepositoryContract<a name="order_contracts_orderpropertyrepositorycontract"></a>

The OrderPropertyRepositoryContract contains the functionality to get, list, create, update and delete  OrderPropertyTypes and OrderProperties as well as OrderProperties. Order properties contain information that are additional to an order. Each property has a type and each type can have several names, but only one name per language. An order can only have one property of each property type.


#### Namespace

`Plenty\Modules\Order\Property\Contracts`



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderproperty">OrderProperty</a>
</pre>

    
Create an order property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order property data. The properties that are required to create an order can be found in the OrderProperty model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderPropertyId = null):<a href="order#order_models_orderproperty">OrderProperty</a>
</pre>

    
Update an order property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order property data. The properties that are required to create an order can be found in the OrderProperty model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderPropertyId</td>
        <td>The ID of the order property.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>($data = []):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an order property. The ID of the order property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>Either the ID of the property or an array holding the composite key composed of the order ID and the type ID.</td>
    </tr>
</table>


<pre>public <strong>findByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List order properties of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the type.</td>
    </tr>
</table>


<pre>public <strong>getType</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/array">array</a> $languages = []):<a href="order#order_models_orderpropertytype">OrderPropertyType</a>
</pre>

    
Get a property type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the property type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$languages</td>
        <td>The languages to load</td>
    </tr>
</table>


<pre>public <strong>getTypes</strong>(<a target="_blank" href="http://php.net/array">array</a> $languages = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List order property types
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$languages</td>
        <td>The languages to load</td>
    </tr>
</table>


<pre>public <strong>createType</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderpropertytype">OrderPropertyType</a>
</pre>

    
Create an order property type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order property type data. The properties that are required to create a type can be found in the OrderPropertyType model.</td>
    </tr>
</table>


<pre>public <strong>updateType</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderpropertytype">OrderPropertyType</a>
</pre>

    
Update an order property type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order property type data.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order property type.</td>
    </tr>
</table>


<pre>public <strong>deleteType</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order property type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order property type</td>
    </tr>
</table>


## Models<a name="order_property_models"></a>
### OrderPropertyTypeName<a name="order_models_orderpropertytypename"></a>

The order property type name model. Each order property type can have one name per language.


#### Namespace

`Plenty\Modules\Order\Property\Models`


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
            <td>The ID of type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the type name</td>
        </tr><tr>
            <td><a href="order#order_models_orderpropertytype">OrderPropertyType</a>
</td>
            <td>type</td>
            <td>The property type instance.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPropertyType<a name="order_models_orderpropertytype"></a>

The OrderPropertyType model. Each order property must have a property type. An order can have one property of each property type. The default property types provided by plentymarkets are listed here.


#### Namespace

`Plenty\Modules\Order\Property\Models`


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
            <td>The ID of the property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that states if this type can be deleted or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>cast</td>
            <td>The data type of the values of this property type. Valid types are:
<ul>
	<li>string</li>
	<li>int</li>
	<li>numeric</li>
	<li>bool</li>
	<li>enum(val1,val2,val3,...)</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>The names of the order property types.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemProperty<a name="order_models_orderitemproperty"></a>

The order item property model.


#### Namespace

`Plenty\Modules\Order\Property\Models`


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
            <td>The ID of the order item property.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderItemId</td>
            <td>The ID of the order item that the property belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the property type.
<ul>
<li>WAREHOUSE		              =	1</li>
<li>SHIPPING_PROFILE	              =	2</li>
<li>PAYMENT_METHOD	              =	3</li>
<li>WEIGHT			              =	11</li>
<li>WIDTH			              =	12</li>
<li>LENGTH		                  =	13</li>
<li>HEIGHT	      		          = 14</li>
<li>EXTERNAL_TOKEN_ID              =	16</li>
<li>EXTERNAL_ITEM_ID               =	17</li>
<li>COUPON_CODE	      	          =	18</li>
<li>COUPON_TYPE		              =	19</li>
<li>ORIGINAL_WAREHOUSE	          =	20</li>
<li>ORIGINAL_QUANTITY              =	21</li>
<li>CATEGORY_ID                    = 22</li>
<li>MARKET_FEE		              =	23</li>
<li>STOCK_REVERSING	              =	24</li>
<li>DISPUTE_STATUS      	          =	25</li>
<li>NO_CHANGE_BY_CONTACT           = 26</li>
<li>SIZE 			              =	29</li>
<li>LOCATION_RESERVED	          =	30</li>
<li>EXTERNAL_SHIPMENT_ITEM_ID      =	31</li>
<li>PARTIAL_SHIPPING_COSTS         =	32</li>
<li>MAIN_DOCUMENT_NUMBER           =	33</li>
<li>SALES_TAX_ID_NUMBER            =	34</li>
<li>RETURNS_REASON                 =	35</li>
<li>RETURNS_ITEM_STATUS            =	36</li>
<li>FULFILLMENT_CENTER_ID          = 37</li>
<li>FULFILLMENT_CENTER_COUNTRY_ISO = 38</li>
<li>REORDER_ITEM_ID                = 39</li>
<li>LISTING_TYPE                   = 40</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property. The value depends on type.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the property was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the property was last updated.</td>
        </tr><tr>
            <td><a href="order#order_models_orderitem">OrderItem</a>
</td>
            <td>orderItem</td>
            <td>The order item that the property belongs to.</td>
        </tr><tr>
            <td><a href="order#order_models_orderpropertytype">OrderPropertyType</a>
</td>
            <td>type</td>
            <td>The type of the property.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderProperty<a name="order_models_orderproperty"></a>

The order properties model. Each order property has a type.


#### Namespace

`Plenty\Modules\Order\Property\Models`


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
            <td>The ID of the order property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order that the property belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the property type. The following types are available:
<ul>
  <li>WAREHOUSE		=	1</li>
  <li>SHIPPING_PROFILE	=	2</li>
  <li>PAYMENT_METHOD			=	3</li>
  <li>PAYMENT_STATUS			=	4</li>
  <li>EXTERNAL_SHIPPING_PROFILE			=	5</li>
  <li>DOCUMENT_LANGUAGE			=	6</li>
  <li>EXTERNAL_ORDER_ID			=	7</li>
  <li>CUSTOMER_SIGN			=	8</li>
  <li>DUNNING_LEVEL			=	9</li>
  <li>SELLER_ACCOUNT			=	10</li>
  <li>WEIGHT			=	11</li>
  <li>WIDTH			=	12</li>
  <li>LENGTH          =	13</li>
  <li>HEIGHT		=	14</li>
  <li>FLAG			=	15</li>
  <li>EXTERNAL_TOKEN_ID			=	16</li>
  <li>EXTERNAL_ITEM_ID			=	17</li>
  <li>COUPON_CODE			=	18</li>
  <li>COUPON_TYPE         =   19</li>
  <li>SALES_TAX_ID_NUMBER =   34</li>
  <li>MAIN_DOCUMENT_NUMBER = 33</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property. The value depends on the type.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the property was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the property was updated last.</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order that the property belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Method<a name="order_method"></a>
    
## Contracts<a name="order_method_contracts"></a>
### PaymentMethodRepositoryContract<a name="order_contracts_paymentmethodrepositorycontract"></a>

Repository Contract for PaymentMethod


#### Namespace

`Plenty\Modules\Order\Payment\Method\Contracts`



#### Methods

<pre>public <strong>getPaymentMethods</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId, <a target="_blank" href="http://php.net/int">int</a> $plentyId = null, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


## Models<a name="order_method_models"></a>
### PaymentMethod<a name="order_models_paymentmethod"></a>

The payment method model


#### Namespace

`Plenty\Modules\Order\Payment\Method\Models`


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
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minimumGross</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priority</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>active</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>showBankDetails</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>infoPageType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>infoPageExternalUrl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeDomesticFlatRateWebstore</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeDomesticFlatRateInternal</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeDomesticPercentageWebstore</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeDomesticPercentageInternal</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeForeignFlatRateWebstore</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeForeignFlatRateInternal</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeForeignPercentageWebstore</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>feeForeignPercentageInternal</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>informations</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>webstores</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>coutries</td>
            <td></td>
        </tr><tr>
            <td><a href="order#order_models_paymentmethodinformation">PaymentMethodInformation</a>
</td>
            <td>information</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentMethodInformation<a name="order_models_paymentmethodinformation"></a>

The payment method information model


#### Namespace

`Plenty\Modules\Order\Payment\Method\Models`


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
            <td>lang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>infoPageType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>infoPageInternalContent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>infoPageExternalUrl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>logo</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>showLogo</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Order<a name="order_order"></a>
    
## Contracts<a name="order_order_contracts"></a>
### OrderAmountRepositoryContract<a name="order_contracts_orderamountrepositorycontract"></a>

This interface allows you to get and list order amounts and their vats.


#### Namespace

`Plenty\Modules\Order\Contracts`



#### Methods

<pre>public <strong>getByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $currency = null):<a href="order#order_models_orderamount">OrderAmount</a>
</pre>

    
Get an order amount for an order in a currency. The ID of the order must be specified. The currency is optional. If no currency is specified, the order amount entry will be returned in the default system currency.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td>The currency of the order amount</td>
    </tr>
</table>


<pre>public <strong>getById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderamount">OrderAmount</a>
</pre>

    
Get an order amount. The ID of the order amount must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order amount</td>
    </tr>
</table>


<pre>public <strong>listByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all order amounts of an order. The ID of the order must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>



### OrderRepositoryContract<a name="order_contracts_orderrepositorycontract"></a>

The OrderRepositoryContract is the interface for the order repository. This interface allows you to find, create and update orders. There are many different order types and the data returned depends on the order type.


#### Namespace

`Plenty\Modules\Order\Contracts`



#### Methods

<pre>public <strong>findOrderById</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="order#order_models_order">Order</a>
</pre>

    
Get an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the order instance, one of "addresses", "events", "dates", "relation", "reference", "location", "payments", "documents" and "comments".</td>
    </tr>
</table>


<pre>public <strong>createOrder</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/string">string</a> $coupon = null):<a href="order#order_models_order">Order</a>
</pre>

    
Create an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order data. The properties that are required to create an order can be found in the order model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$coupon</td>
        <td>A coupon code to be redeemed in the order.</td>
    </tr>
</table>


<pre>public <strong>updateOrder</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="order#order_models_order">Order</a>
</pre>

    
Update an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order data. The properties that are required to update an order can be found in the order model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>deleteOrder</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>undeleteOrder</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/float">float</a> $status):<a href="order#order_models_order">Order</a>
</pre>

    
Restore an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$status</td>
        <td>The status of the order</td>
    </tr>
</table>


<pre>public <strong>isDeleted</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether an order has been deleted or not.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>findSchedulerById</strong>(<a target="_blank" href="http://php.net/int">int</a> $schedulerId):<a href="order#order_models_orderscheduler">OrderScheduler</a>
</pre>

    
Get a scheduler order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$schedulerId</td>
        <td>The ID of the scheduler order</td>
    </tr>
</table>


<pre>public <strong>allOrdersByContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List orders of a contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of orders to be displayed per page. The default number of orders per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Order instance. Valid are "addresses", "events", "dates", "relation", "reference", "location", "payments", "documents" and "comments".</td>
    </tr>
</table>


<pre>public <strong>allOrdersBySupplier</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List orders that include one or more variations from a supplier
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact (supplier id)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of orders to be displayed per page. The default number of orders per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Order instance. Valid are "addresses", "events", "dates", "relation", "reference", "location", "payments", "documents" and "comments".</td>
    </tr>
</table>


<pre>public <strong>allOrdersByContactSender</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List orders sent by a contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of orders to be displayed per page. The default number of orders per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Order instance. Valid are "addresses", "events", "dates", "relation", "reference", "location", "payments", "documents" and "comments".</td>
    </tr>
</table>


<pre>public <strong>getLatestOrderByContactId</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="order#order_models_order">Order</a>
</pre>

    
Get latest order of a contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Order instance. The relations available are: "addresses", "events", "dates", "relation", "reference", "location", "payments", "documents" and "comments".
If you want to load relations, you need to include at least one, but you can also include several or all.</td>
    </tr>
</table>


<pre>public <strong>searchOrders</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List orders
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of orders to be displayed per page. The default number of orders per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Order instance. Valid are "addresses", "events", "dates", "relation", "reference", "location", "payments", "documents" and "comments".</td>
    </tr>
</table>


<pre>public <strong>getPackageNumbers</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List package numbers of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>cancelOrder</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Cancel an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>findOrderByAccessKey</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $accessKey):<a href="order#order_models_order">Order</a>
</pre>

    
Find the order for the given order ID and access key.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order to be checked.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$accessKey</td>
        <td>The access key, that belongs to the order.</td>
    </tr>
</table>


<pre>public <strong>generateAccessKey</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Generate an access key for the given order ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createMultiOrderByContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId):<a href="order#order_models_order">Order</a>
</pre>

    
Creates a multi order for a specific contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
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
    

### OrderItemRepositoryContract<a name="order_contracts_orderitemrepositorycontract"></a>

The OrderItemRepositoryContract is the interface for the order item repository. This interface allows you to find, create and update order items. An order item can be e.g. items, surcharges and coupons. Each order item is given a unique id, which links it to a specific order.


#### Namespace

`Plenty\Modules\Order\Contracts`



#### Methods

<pre>public <strong>getOrderItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId):<a href="order#order_models_orderitem">OrderItem</a>
</pre>

    
Get an order item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
</table>


<pre>public <strong>deleteOrderItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $orderItemId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order that the item belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item to be deleted.</td>
    </tr>
</table>


## Models<a name="order_order_models"></a>
### PriceCalculationResultItem<a name="order_models_pricecalculationresultitem"></a>

price calculation result item


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>total</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>totalNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>totalGross</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>totalVat</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>highestVatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>netAmountsMap</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>vatAmountsMap</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderReference<a name="order_models_orderreference"></a>

The order reference model. Each OrderReference has an origin order (the most top order) and a referenced order (currently only &#039;parent&#039;).


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The id of the order reference entry.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The order id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>originOrderId</td>
            <td>The id of the origin order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referenceOrderId</td>
            <td>The id of the referenced order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceType</td>
            <td>The reference type (currently only "parent") of the referenced order.</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td></td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>originOrder</td>
            <td>The origin order of the order.</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>referenceOrder</td>
            <td>The referenced order of the order.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderAmountVat<a name="order_models_orderamountvat"></a>

The order amount vat model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the VAT information of an order amount</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderAmountId</td>
            <td>The ID of the order amount that the VAT information belong to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryVatId</td>
            <td>The ID of the VAT configuration</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatField</td>
            <td>The ID of the VAT rate's field [0,1,2,3].</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatRate</td>
            <td>The actual VAT rate that was used, e.g. 19%.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The VAT amount of money given in the same currency as the order amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>netTotal</td>
            <td>The net amount for the current vat rate.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>grossTotal</td>
            <td>The gross amount for the current vat rate.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the VAT was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the VAT was updated last.</td>
        </tr><tr>
            <td><a href="order#order_models_orderamount">OrderAmount</a>
</td>
            <td>orderAmount</td>
            <td>The OrderAmount model that the OrderAmountVat belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Order<a name="order_models_order"></a>

The order model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the order type
                                								It is possible to define individual order types. However,
                                								the following types are available by default:
<ul>
    <li>Sales order = 1</li>
    <li>Delivery = 2</li>
    <li>Returns = 3</li>
    <li>Credit note = 4</li>
    <li>Warranty = 5</li>
    <li>Repair = 6</li>
    <li>Offer = 7</li>
    <li>Advance order = 8</li>
    <li>Multi-order = 9</li>
    <li>Multi credit note = 10</li>
    <li>Multi delivery = 11</li>
    <li>Reorder = 12</li>
    <li>Partial delivery = 13</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>methodOfPaymentId</td>
            <td>The ID of the order's payment method (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingProfileId</td>
            <td>The ID of the order's shipping profile (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paymentStatus</td>
            <td>The payment status of the order (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>statusId</td>
            <td>The ID of the order status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>statusName</td>
            <td>The name for the status ID (read only)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ownerId</td>
            <td>The user ID of the order's owner</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the order was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the order was updated last</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The plenty ID of the client that the order belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>locationId</td>
            <td>The ID of the location that the order belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lockStatus</td>
            <td>The lock status of the order. The following statuses are available:
<ul>
 <li>unlocked</li>
 <li>permanentlyLocked</li>
 <li>reversibleLocked</li>
</ul></td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>billingAddress</td>
            <td>The invoice address of the order</td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>deliveryAddress</td>
            <td>The delivery address of the order</td>
        </tr><tr>
            <td><a href="authentication#authentication_models_user">User</a>
</td>
            <td>owner</td>
            <td>The owner of the order</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>addresses</td>
            <td>The address objects that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>addressRelations</td>
            <td>The address relations for this order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>orderItems</td>
            <td>The order items that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td>The order properties that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>relations</td>
            <td>The order relation reference instances that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>amounts</td>
            <td>The order amounts that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>comments</td>
            <td>The order comments.</td>
        </tr><tr>
            <td><a href="accounting#accounting_models_accountinglocation">AccountingLocation</a>
</td>
            <td>location</td>
            <td>The accounting location of the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>payments</td>
            <td>The payments that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>orderReferences</td>
            <td>The order references.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>documents</td>
            <td>The documents that are associated with the order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dates</td>
            <td>The dates of the order. Can contain many different dates with their types like:
<ul>
<li>Delete date = 1</li>
<li>Entry date = 2</li>
<li>Payment date = 3</li>
<li>Delivery date = 4</li>
</ul></td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>originOrder</td>
            <td>The origin order of this order. If this order is the origin, this attribute is null. (deprecated)</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>parentOrder</td>
            <td>The parent order of this order. If this order has no parent, this attribute is null. (deprecated)</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>originOrders</td>
            <td>The origin orders of this order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>parentOrders</td>
            <td>The parent orders of this order.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemOrderProperty<a name="order_models_orderitemorderproperty"></a>

This model contains the order properties that are assigned to order items.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value for the order property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileUrl</td>
            <td>The URL of the order property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the order property</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderAmount<a name="order_models_orderamount"></a>

The order amount model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order that the amount belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSystemCurrency</td>
            <td>Flag that states if the current currency is the same as system currency or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isNet</td>
            <td>Flag that states if the invoice is net or not. If the invoice is not net, it is gross.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency of the amounts.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRate</td>
            <td>The exchange rate for converting the current currency into the system currency.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>netTotal</td>
            <td>The total net amount of the order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>grossTotal</td>
            <td>The total gross amount of the order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatTotal</td>
            <td>The total vat amount of the order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>invoiceTotal</td>
            <td>The total invoice amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>paidAmount</td>
            <td>The order amount that is already paid.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>prepaidAmount</td>
            <td>This is deprecated and will be removed in the next version. Please use <code>$giftCardAmount</code> instead.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>giftCardAmount</td>
            <td>The amount that comes from gift cards that were redeemed when placing the order
The gift cards amount does not reduce the invoice total, but reduces the amount that still needs to be paid.
The amount that still needs to paid is not an own parameter because the amount can be calculated by subtracting the gift cards amount from the invoice total.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the amount was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the amount was updated last.</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order that this amount belongs to.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>vats</td>
            <td>The vat amounts</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItem<a name="order_models_orderitem"></a>

The order item model. Items, shipping costs, coupons, surcharges etc. are all displayed as order items.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order that the order item belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the order item type
<ul>
<li>VARIATION			=	1</li>
<li>ITEM_BUNDLE			=	2</li>
<li>BUNDLE_COMPONENT		=	3</li>
<li>PROMOTIONAL_COUPON	=	4</li>
<li>GIFT_CARD			=	5</li>
<li>SHIPPING_COSTS		=	6</li>
<li>PAYMENT_SURCHARGE	=	7</li>
<li>GIFT_WRAP			=	8</li>
<li>UNASSIGEND_VARIATION	=	9</li>
<li>DEPOSIT				=	10</li>
<li>ORDER				=	11</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The ID of order item referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemVariationId</td>
            <td>The ID of the item variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>quantity</td>
            <td>The quantity.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderItemName</td>
            <td>The name of the order item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>attributeValues</td>
            <td>The attribute value names</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingProfileId</td>
            <td>The ID of the order item's shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryVatId</td>
            <td>The ID of the country vat</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatField</td>
            <td>The vat id (0-3).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatRate</td>
            <td>The vat amount, e.g. 19.0 for 19% VAT.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The order items position in the order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The ID of the warehouse.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date at which the order item was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the order item was last updated.</td>
        </tr><tr>
            <td><a href="order#order_models_orderitemamount">OrderItemAmount</a>
</td>
            <td>systemAmount</td>
            <td>The order item's amount in the system currency.</td>
        </tr><tr>
            <td><a href="order#order_models_orderitemamount">OrderItemAmount</a>
</td>
            <td>amount</td>
            <td>The order item's amount in the order currency. If the order currency is the same as the system currency this amount is the same.</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order that the property belongs to.</td>
        </tr><tr>
            <td><a href="order#order_models_orderitemtype">OrderItemType</a>
</td>
            <td>type</td>
            <td>The order item type</td>
        </tr><tr>
            <td><a href="accounting#accounting_models_vat">Vat</a>
</td>
            <td>countryVat</td>
            <td>The country vat instance.</td>
        </tr><tr>
            <td><a href="item#item_models_variation">Variation</a>
</td>
            <td>variation</td>
            <td>The item variation in the position.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>amounts</td>
            <td>The order item amounts that belong to the order item.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td>The order item properties that belong to the order item.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>orderProperties</td>
            <td>The order item order properties that belong to the order item.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>orderDates</td>
            <td>The dates of the associated order.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dates</td>
            <td>The dates of the order item. Can contain many different dates with their types. The following types are currently available:
<ul>
<li>Deleted on = 1</li>
<li>Created on = 2</li>
<li>Paid date = 3</li>
<li>Last update = 4</li>
<li>Completed on = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
<li>Start date = 9</li>
<li>End date = 10</li>
<li>Possible delivery date = 11</li>
<li>Market transfer date = 12</li>
</ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>references</td>
            <td>The order item references.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>giftCardCodes</td>
            <td>The gift card codes that belong to the order item.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemAmount<a name="order_models_orderitemamount"></a>

The order item amount model. Order item amount refers to amounts of money.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order item amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderItemId</td>
            <td>The ID of the order item that the amount belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSystemCurrency</td>
            <td>Flag that indicates if the current currency is the same as the system currency or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency of the amounts.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRate</td>
            <td>The exchange rate for converting the current currency into the system currency.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td>The purchase price of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>priceOriginalGross</td>
            <td>The original gross price without any surcharges or discounts.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>priceOriginalNet</td>
            <td>The original net price without any surcharges or discounts.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>priceGross</td>
            <td>The total gross price including surcharges and discounts [READONLY].</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>priceNet</td>
            <td>The total net price including surcharges and discounts [READONLY].</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>surcharge</td>
            <td>The surcharge as gross amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>discount</td>
            <td>The discount can be a percentage or a fixed value.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPercentage</td>
            <td>Flag that indicates if a discount is given as a percentage or as a fixed value.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the amount was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the amount was last updated.</td>
        </tr><tr>
            <td><a href="order#order_models_orderitem">OrderItem</a>
</td>
            <td>orderItem</td>
            <td>The order item that the amount belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemType<a name="order_models_orderitemtype"></a>

The order item type model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order item type. The following types are currently available: <br />
<ul>
<li>VARIATION			=	1</li>
<li>ITEM_BUNDLE			=	2</li>
<li>BUNDLE_COMPONENT		=	3</li>
<li>PROMOTIONAL_COUPON	=	4</li>
<li>GIFT_CARD			=	5</li>
<li>SHIPPING_COSTS		=	6</li>
<li>PAYMENT_SURCHARGE	=	7</li>
<li>GIFT_WRAP			=	8</li>
<li>UNASSIGEND_VARIATION	=	9</li>
<li>DEPOSIT				=	10</li>
<li>ORDER				=	11</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if this type can be deleted or not</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The names of the order item types</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemTypeName<a name="order_models_orderitemtypename"></a>

The order item type name model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The related type id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The ISO 639-1 language code for the name, e.g. "en" for English</td>
        </tr><tr>
            <td><a href="order#order_models_orderitemtype">OrderItemType</a>
</td>
            <td>type</td>
            <td>The order item type instance.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderTypeName<a name="order_models_ordertypename"></a>

The order type name model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The ISO 639-1 language code for the name, e.g. "en" for English</td>
        </tr><tr>
            <td><a href="order#order_models_ordertype">OrderType</a>
</td>
            <td>type</td>
            <td>The order type instance.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderType<a name="order_models_ordertype"></a>

The order type model.


#### Namespace

`Plenty\Modules\Order\Models`


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
            <td>The ID of the order type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that states if this type can be deleted or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The names of the order item types.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CouponCodeOrder<a name="order_models_couponcodeorder"></a>

The CouponCodeOrder model.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Order\Models`


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
            <td>corderItemId</td>
            <td>The ID of the order item that the coupon was redeemed for</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>campaignId</td>
            <td>The ID of the campaign that the coupon belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>code</td>
            <td>The coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The display type of the redeemed coupon
The following display types are available:<ul>
<li>disposable</li>
<li>fixed_vat</li>
<li>fixed</li>
<li>percental</li>
<li>undefined</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>amount</td>
            <td>The redeemed amount of the coupon</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>vatRate</td>
            <td>The redeemed vat rate of the coupon</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### GiftCardCode<a name="order_models_giftcardcode"></a>

Model that holds gift card codes.


#### Namespace

`Plenty\Modules\Order\Coupon\Campaign\Code\Order\Models`


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
            <td>The ID of the gift card code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderItemId</td>
            <td>The order item ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>campaignId</td>
            <td>The campaign ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>code</td>
            <td>The coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sender</td>
            <td>The name of the sender</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>receiver</td>
            <td>The name of the receiver</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>message</td>
            <td>The message</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="order_order_events"></a>
### OrderPartlyPaid<a name="order_events_orderpartlypaid"></a>

An Event class fired after a payment is assigned and if the order is only partly paid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderOverpaid<a name="order_events_orderoverpaid"></a>

An event class will be fired after a payment is assigned and if the order is overpaid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderCreated<a name="order_events_ordercreated"></a>

An event class fired after a new order is created. The order type is not relevant.
 * 	At the same time also type depended events will be fired, like ReturnsCreated or CreditNoteCreated.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderPaidEvent<a name="order_events_orderpaidevent"></a>

A base Event class for all order paid events.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderFullyPaid<a name="order_events_orderfullypaid"></a>

An Event class fired after a payment assignment when the order is fully paid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderPaymentAssigned<a name="order_events_orderpaymentassigned"></a>

An Event class fired after a payment was assigned to an order.
 * After this event one of the following events will be fired, depending the payment status of the order:
 *	 OrderPrepaid, OrderPartlyPaid, OrderFullyPaid, OrderOverpaid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order, <a href="payment#payment_models_payment">Payment</a>
 $payment):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderPaymentAssigned constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="payment#payment_models_payment">Payment</a>
</td>
        <td>$payment</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPayment</strong>():<a href="payment#payment_models_payment">Payment</a>
</pre>

    
Get the payment.
    
<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderPrepaid<a name="order_events_orderprepaid"></a>

An Event class fired after a payment is assigned and if the order is paid in advance.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### OrderEvent<a name="order_events_orderevent"></a>

A base event class for all order events. Each order event expects an order instance.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    
## Services<a name="order_order_services"></a>
### OrderCreatedTypeService<a name="order_services_ordercreatedtypeservice"></a>

This class is used as an event listener as well as a service for registering events. The class allows to register event classes to extend the OrderCreated event for custom order types.


#### Namespace

`Plenty\Modules\Order\Services`



#### Methods

<pre>public <strong>handle</strong>(<a href="order#order_events_ordercreated">OrderCreated</a>
 $created):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Reacts upon the OrderCreated event
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_events_ordercreated">OrderCreated</a>
</td>
        <td>$created</td>
        <td>The event instance.</td>
    </tr>
</table>


<pre>public static <strong>addEventForType</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/string">string</a> $className):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create event class for a custom order type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the custom order type.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$className</td>
        <td>The name of the event class.</td>
    </tr>
</table>


<pre>public static <strong>removeEventForType</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/string">string</a> $className):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete event class from a custom order type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the custom order type.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$className</td>
        <td>The name of the event class.</td>
    </tr>
</table>


# Date<a name="order_date"></a>
    
## Contracts<a name="order_date_contracts"></a>
### OrderDateRepositoryContract<a name="order_contracts_orderdaterepositorycontract"></a>

The OrderDateRepositoryContract contains the functionality to find available OrderDateTypes with their names in a specific language. Furthermore it is possible to create new OrderDateTypes, to update or delete existing date types and to create date type names for a language.


#### Namespace

`Plenty\Modules\Order\Date\Contracts`



#### Methods

<pre>public <strong>findNamesByTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List names of a date type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>findNameByTypeIdAndLang</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="order#order_models_orderdatetypename">OrderDateTypeName</a>
</pre>

    
Get a name of a date type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language ISO 639-1 code, e.g. "en" for English</td>
    </tr>
</table>


<pre>public <strong>findTypes</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List date types
    
<pre>public <strong>findTypeById</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderdatetype">OrderDateType</a>
</pre>

    
Get a date type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderdate">OrderDate</a>
</pre>

    
Create an order date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order date data. The properties that are required to create an order can be found in the OrderDate model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderDateId):<a href="order#order_models_orderdate">OrderDate</a>
</pre>

    
Update a date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order date data. The properties that are required to create an order can be found in the OrderDate model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderDateId</td>
        <td>The ID of the order date</td>
    </tr>
</table>


<pre>public <strong>save</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderdate">OrderDate</a>
</pre>

    
Create or update an order date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order date data. The properties that are required to create an order can be found in the OrderDate model.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderDateId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderDateId</td>
        <td>The ID of the order date</td>
    </tr>
</table>


<pre>public <strong>deleteByOrderIdAndType</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete an order date from an order by the type of the order date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type.</td>
    </tr>
</table>


<pre>public <strong>findByOrderIdAndTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderdate">OrderDate</a>
</pre>

    
Get an order date from an order by the type of the order date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>findByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List order dates of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>



### OrderItemDateRepositoryContract<a name="order_contracts_orderitemdaterepositorycontract"></a>

The OrderItemDateRepositoryContract contains the functionality to get, create, update and delete OrderItemDate instances.


#### Namespace

`Plenty\Modules\Order\Date\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Get an order item date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order item date.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Create an order item date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item date data. The properties that are required to create an order item can be found in the OrderItemDate model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Update an order date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item date data. The properties that are required to create an order item can be found in the OrderItemDate model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order item date</td>
    </tr>
</table>


<pre>public <strong>save</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Create or update an order item date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item date data. The properties that are required to create or update an order can be found in the OrderItemDate model.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the order item date</td>
    </tr>
</table>


<pre>public <strong>findByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Get an order item date by an order item and an order date type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>createByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Create an order item date by an order item and an order date type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item date data. The properties that are required to create an order can be found in the OrderItemDate model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>updateByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderitemdate">OrderItemDate</a>
</pre>

    
Update an order item date by an order item and an order date type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order item date data. The properties that are required to update an order can be found in the OrderItemDate model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>deleteByOrderItemIdAndTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order item date by an order item and an order date type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the date type</td>
    </tr>
</table>


<pre>public <strong>findByOrderItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List order item dates of an order item.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order</td>
    </tr>
</table>


## Models<a name="order_date_models"></a>
### OrderDateType<a name="order_models_orderdatetype"></a>

The OrderDateType model.


#### Namespace

`Plenty\Modules\Order\Date\Models`


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
            <td>The ID of the order date type. The following date types are available:
<ul>
<li>Deleted on = 1</li>
<li>Created on = 2</li>
<li>Paid date = 3</li>
<li>Last update = 4</li>
<li>Completed on = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
<li>Start date = 9</li>
<li>End date = 10</li>
<li>Possible delivery date = 11</li>
<li>Market transfer date = 12</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if this type can be deleted or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The names for this OrderDateType</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>orderDates</td>
            <td>The actual dates that belong to the order date type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderDate<a name="order_models_orderdate"></a>

The OrderDate model.


#### Namespace

`Plenty\Modules\Order\Date\Models`


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
            <td>The ID of the order date</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order that the date belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the date type. The following types are available:
<ul>
<li>Deleted on = 1</li>
<li>Created on = 2</li>
<li>Paid date = 3</li>
<li>Last update = 4</li>
<li>Completed date = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
<li>Start date = 9</li>
<li>End date = 10</li>
<li>Estimated delivery date = 11</li>
</ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>date</td>
            <td>The date plus hours, minutes and seconds. The date format must comply with the W3C standard.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the date was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the date was last updated</td>
        </tr><tr>
            <td><a href="order#order_models_orderdatetype">OrderDateType</a>
</td>
            <td>type</td>
            <td>The type of date</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemDate<a name="order_models_orderitemdate"></a>

The OrderItemDate model.


#### Namespace

`Plenty\Modules\Order\Date\Models`


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
            <td>The ID of the order date</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderItemId</td>
            <td>The ID of the order item that the date belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the date type. The following types are available:
<ul>
<li>Start date = 9</li>
<li>End date = 10</li>
<li>Estimated delivery date = 11</li>
</ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>date</td>
            <td>The date plus hours, minutes and seconds. The date format must comply with the W3C standard.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the date was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the date was last updated</td>
        </tr><tr>
            <td><a href="order#order_models_orderdatetype">OrderDateType</a>
</td>
            <td>type</td>
            <td>The type of the date.  The following date types are available:
<ul>
<li>Deleted on = 1</li>
<li>Created on = 2</li>
<li>Paid date = 3</li>
<li>Last update = 4</li>
<li>Completed on = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
<li>Start date = 9</li>
<li>End date = 10</li>
<li>Possible delivery date = 11</li>
<li>Market transfer date = 12</li>
</ul></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderDateTypeName<a name="order_models_orderdatetypename"></a>

The OrderDateTypeName model. Order date types can have several names. One name per language. Each name has a unique ID.


#### Namespace

`Plenty\Modules\Order\Date\Models`


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
            <td>The ID of the order date type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the date type that this name belongs to. The following date types are available:
<ul>
<li>Deleted on = 1</li>
<li>Created on = 2</li>
<li>Paid date = 3</li>
<li>Last update = 4</li>
<li>Completed on = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
<li>Start date = 9</li>
<li>End date = 10</li>
<li>Possible delivery date = 11</li>
<li>Market transfer date = 12</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The ISO 639-1 language code for the name, e.g. "en" for English</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the order date type</td>
        </tr><tr>
            <td><a href="order#order_models_orderdatetype">OrderDateType</a>
</td>
            <td>type</td>
            <td>The date type that this name belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Pdf<a name="order_pdf"></a>
    
## Models<a name="order_pdf_models"></a>
### OrderPdfGeneration<a name="order_models_orderpdfgeneration"></a>

OrderPdfGeneration Model


#### Namespace

`Plenty\Modules\Order\Pdf\Models`


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
            <td>language</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>advice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>sums</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="order_pdf_events"></a>
### OrderPdfGenerationEvent<a name="order_events_orderpdfgenerationevent"></a>

OrderPdfGenerationEvent


#### Namespace

`Plenty\Modules\Order\Pdf\Events`



#### Methods

<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the
    
<pre>public <strong>getDocType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the
    
<pre>public <strong>addOrderPdfGeneration</strong>(<a href="order#order_models_orderpdfgeneration">OrderPdfGeneration</a>
 $orderPdfGeneration):<a href="order#order_pdf_events">Events</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_orderpdfgeneration">OrderPdfGeneration</a>
</td>
        <td>$orderPdfGeneration</td>
        <td></td>
    </tr>
</table>


# Scheduler<a name="order_scheduler"></a>
    
## Models<a name="order_scheduler_models"></a>
### OrderScheduler<a name="order_models_orderscheduler"></a>

The legacy order model


#### Namespace

`Plenty\Modules\Order\Scheduler\Models`


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
            <td>The order id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The contact id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>methodOfPayment</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>start</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>last</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>end</td>
            <td></td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>deliveryAddress</td>
            <td></td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>billingAddress</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>addresses</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>addressRelations</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ContactWish<a name="order_contactwish"></a>
    
## Contracts<a name="order_contactwish_contracts"></a>
### ContactWishRepositoryContract<a name="order_contracts_contactwishrepositorycontract"></a>

This interface allows you to get and create contact wishes.


#### Namespace

`Plenty\Modules\Order\ContactWish\Contracts`



#### Methods

<pre>public <strong>getContactWish</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="order#order_models_contactwish">ContactWish</a>
</pre>

    
Get the contact wish
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>createContactWish</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $text):<a href="order#order_models_contactwish">ContactWish</a>
</pre>

    
Create a contact wish
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$text</td>
        <td>The text for the contact wish</td>
    </tr>
</table>


## Models<a name="order_contactwish_models"></a>
### ContactWish<a name="order_models_contactwish"></a>

The contact wish model.


#### Namespace

`Plenty\Modules\Order\ContactWish\Models`


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
            <td>text</td>
            <td>The text of the contact wish</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Models<a name="order_models"></a>
    
## Legacy<a name="order_models_legacy"></a>
### Order<a name="order_legacy_order"></a>

The legacy order model


#### Namespace

`Plenty\Modules\Order\Models\Legacy`


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
            <td>The Id of an order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderType</td>
            <td>The type of an order type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>status</td>
            <td>The status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The owner of an order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>entryDate</td>
            <td>The date that the order was entered</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>webstoreId</td>
            <td>The ID of the webstore</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The ID of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sellerAccount</td>
            <td>The seller account</td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>deliveryAddress</td>
            <td></td>
        </tr><tr>
            <td><a href="account#account_models_address">Address</a>
</td>
            <td>billingAddress</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>addresses</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>addressRelations</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Information<a name="order_information"></a>
    
## Contracts<a name="order_information_contracts"></a>
### ShippingInformationRepositoryContract<a name="order_contracts_shippinginformationrepositorycontract"></a>

The ShippingInformationRepositoryContract is the interface for the shipping information repository. This interface allows to get shipping information by order ID, create new shipping information or update shipping information.


#### Namespace

`Plenty\Modules\Order\Shipping\Information\Contracts`



#### Methods

<pre>public <strong>getShippingInformationByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="order#order_models_shippinginformation">ShippingInformation</a>
</pre>

    
Get Shipping Information by an order ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the Order</td>
    </tr>
</table>


<pre>public <strong>resetShippingInformation</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete Shipping Information by an order ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the Order</td>
    </tr>
</table>


<pre>public <strong>saveShippingInformation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_shippinginformation">ShippingInformation</a>
</pre>

    
Create Shipping Information
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The shipping information data as associative array.</td>
    </tr>
</table>


<pre>public <strong>updateAdditionalData</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="order#order_models_shippinginformation">ShippingInformation</a>
</pre>

    
Update Additional Data of Shipping Information by Order ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The additional data as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order.</td>
    </tr>
</table>


<pre>public <strong>updateShippingStatus</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="order#order_models_shippinginformation">ShippingInformation</a>
</pre>

    
Update Shipping Status of Shipping Information by Order ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The status data as associative array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order.</td>
    </tr>
</table>


## Models<a name="order_information_models"></a>
### ShippingInformation<a name="order_models_shippinginformation"></a>

ShippingInformationModel


#### Namespace

`Plenty\Modules\Order\Shipping\Information\Models`


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
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingServiceProvider</td>
            <td>The name of the shipping service provider</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>transactionId</td>
            <td>The ID of the transaction</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingStatus</td>
            <td>The shipping status. Possible values are 'open', 'prepared' and 'registered'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>shippingCosts</td>
            <td>The shipping costs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>additionalData</td>
            <td>The additional data. Depending on the shipping service provider selected, this data may contain different information, e.g. shipping service, email address and order ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>registrationAt</td>
            <td>The date and time the shipment was registered</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shipmentAt</td>
            <td>The date the items will be shipped</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Shipping<a name="order_shipping"></a>
    
## Contracts<a name="order_shipping_contracts"></a>
### EUCountryCodesServiceContract<a name="order_contracts_eucountrycodesservicecontract"></a>

The EUCountryCodesServiceContract


#### Namespace

`Plenty\Modules\Order\Shipping\Contracts`



#### Methods

<pre>public <strong>isEUCountry</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasCommunityTax</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getTaxTerritory</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasCommunityToll</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getTollTerritory</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isExportDelivery</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId, <a target="_blank" href="http://php.net/int">int</a> $merchandCountryId = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$merchandCountryId</td>
        <td></td>
    </tr>
</table>



### ParcelServicePresetRepositoryContract<a name="order_contracts_parcelservicepresetrepositorycontract"></a>

The ParcelServicePresetRepositoryContract is the interface for the shipping profile repository. This interface allows to get a shipping profile by the ID or list all shipping profiles.


#### Namespace

`Plenty\Modules\Order\Shipping\Contracts`



#### Methods

<pre>public <strong>getPresetList</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/string">string</a> $with = null, <a target="_blank" href="http://php.net/string">string</a> $parcelServiceName = null, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Lists shipping profiles.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns (attributes) to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$with</td>
        <td>The parameter contains the name of an relation</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$parcelServiceName</td>
        <td>Filter that restricts the search result to parcel service presets with a specified service name (e.g. 'DHL' for DHL)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Possible attributes are updatedAtBefore and updatedAtAfter (yyyy-mm-dd or yyyy-mm-dd hh:mm:ss)</td>
    </tr>
</table>


<pre>public <strong>getPresetById</strong>(<a target="_blank" href="http://php.net/int">int</a> $presetId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="order#order_models_parcelservicepreset">ParcelServicePreset</a>
</pre>

    
Gets a shipping profile. The ID of the shipping profile must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$presetId</td>
        <td>The ID of the shipping profile</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns (attributes) to retrieve</td>
    </tr>
</table>


<pre>public <strong>getLastWeightedPresetCombinations</strong>(<a href="basket#basket_models_basket">Basket</a>
 $basket, <a target="_blank" href="http://php.net/int">int</a> $contactClass, <a target="_blank" href="http://php.net/array">array</a> $customParams = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Calculate shipping costs and list last weighted preset combinations.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="basket#basket_models_basket">Basket</a>
</td>
        <td>$basket</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactClass</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$customParams</td>
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
    
## Models<a name="order_shipping_models"></a>
### DefaultShipping<a name="order_models_defaultshipping"></a>

The Default Shipping model


#### Namespace

`Plenty\Modules\Order\Shipping\Models`


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
            <td>referrerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingDestinationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentMethod1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentMethod2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentMethod3</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="order_shipping_events"></a>
### AfterShippingCostCalculated<a name="order_events_aftershippingcostcalculated"></a>

An event class fired after the shipping calculation is done. Listeners can add fees to the shipping costs.
 * The shipping provider type name is mandatory, orderId is optional.


#### Namespace

`Plenty\Modules\Order\Shipping\Events`



#### Methods

<pre>public <strong>getShippingServiceProvider</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the
    
<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $shippingServiceProvider, <a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $shippingProfileId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
AfterShippingCostCalculated constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$shippingServiceProvider</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingProfileId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrderId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the
    
<pre>public <strong>getAdditonalFee</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>

    
Get the
    
<pre>public <strong>addAdditionalFee</strong>(<a target="_blank" href="http://php.net/float">float</a> $additonalFee):<a href="order#order_events_aftershippingcostcalculated">AfterShippingCostCalculated</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$additonalFee</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getShippingProfileId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setShippingProfileId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingProfileId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingProfileId</td>
        <td></td>
    </tr>
</table>


# ServiceProvider<a name="order_serviceprovider"></a>
    
## Contracts<a name="order_serviceprovider_contracts"></a>
### ShippingServiceProviderRepositoryContract<a name="order_contracts_shippingserviceproviderrepositorycontract"></a>

The ShippingServiceProviderRepositoryContract is the interface for the shipping service provider repository. This interface allows to list shipping service providers.


#### Namespace

`Plenty\Modules\Order\Shipping\ServiceProvider\Contracts`



#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Lists shipping service providers.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to retrieve</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingServiceProviderId):<a href="order#order_models_shippingserviceprovider">ShippingServiceProvider</a>
</pre>

    
Gets a shipping service provider. The ID of the shipping service provider must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingServiceProviderId</td>
        <td>The ID of the shipping service provider</td>
    </tr>
</table>


<pre>public <strong>findByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $shippingServiceProviderName):<a href="order#order_models_shippingserviceprovider">ShippingServiceProvider</a>
</pre>

    
Gets a shipping service provider. The name of the shipping service provider must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$shippingServiceProviderName</td>
        <td>The name of the shipping service provider</td>
    </tr>
</table>


<pre>public <strong>saveShippingServiceProvider</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $shippingServiceProviderName):<a href="order#order_models_shippingserviceprovider">ShippingServiceProvider</a>
</pre>

    
Creates a shipping service provider or updates it if already existing
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>The plugin name the plugin is registered with</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$shippingServiceProviderName</td>
        <td>The name of the shipping service provider</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### ShippingServiceProviderPluginRepositoryContract<a name="order_contracts_shippingserviceproviderpluginrepositorycontract"></a>

The ShippingServiceProviderPluginRepositoryContract is the interface for the shipping service provider plugin repository. This interface allows to list shipping service provider plugins.


#### Namespace

`Plenty\Modules\Order\Shipping\ServiceProvider\Contracts`



#### Methods

<pre>public <strong>plugins</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>filteredPluginList</strong>(<a target="_blank" href="http://php.net/string">string</a> $filter):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


## Models<a name="order_serviceprovider_models"></a>
### ShippingServiceProvider<a name="order_models_shippingserviceprovider"></a>

The service provider model


#### Namespace

`Plenty\Modules\Order\Shipping\ServiceProvider\Models`


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
            <td>The ID of the shipping service provider</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the shipping service provider</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pluginId</td>
            <td>The optional ID of the plugin when the shipping service provider is registered as a plugin</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The time the shipping service provider was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The time the shipping service provider was updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="order_serviceprovider_services"></a>
### ShippingServiceProviderService<a name="order_services_shippingserviceproviderservice"></a>

The ShippingServiceProviderService class offers the possibility to register a shipping provider class and method that can be called by plentymarkets shipping controllers.


#### Namespace

`Plenty\Modules\Order\Shipping\ServiceProvider\Services`



#### Methods

<pre>public <strong>registerShippingProvider</strong>(<a target="_blank" href="http://php.net/string">string</a> $shippingServiceProviderCode, <a target="_blank" href="http://php.net/array">array</a> $shippingServiceProviderNames, <a target="_blank" href="http://php.net/array">array</a> $shippingServiceProviderClasses):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$shippingServiceProviderCode</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$shippingServiceProviderNames</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$shippingServiceProviderClasses</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasShippingServiceProviderMethod</strong>(<a target="_blank" href="http://php.net/string">string</a> $shippingServiceProviderCode, <a target="_blank" href="http://php.net/string">string</a> $methodName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$shippingServiceProviderCode</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$methodName</td>
        <td></td>
    </tr>
</table>


# Services<a name="order_services"></a>
    
## Entries<a name="order_services_entries"></a>
### ShippingServiceProviderEntry<a name="order_entries_shippingserviceproviderentry"></a>

The shipping provider entry contains all information needed to use module shipping in plentymarkets shipping .


#### Namespace

`Plenty\Modules\Order\Shipping\ServiceProvider\Services\Entries`



#### Methods

<pre>public <strong>getShippingServiceProviderClasses</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the
    
<pre>public <strong>getShippingServiceProviderNames</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the
    
<pre>public <strong>setShippingServiceProviderNames</strong>(<a target="_blank" href="http://php.net/array">array</a> $shippingServiceProviderNames):<a href="order#order_entries_shippingserviceproviderentry">ShippingServiceProviderEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$shippingServiceProviderNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getShippingServiceProviderCode</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the
    
<pre>public <strong>setShippingServiceProviderCode</strong>(<a target="_blank" href="http://php.net/string">string</a> $shippingServiceProviderCode):<a href="order#order_entries_shippingserviceproviderentry">ShippingServiceProviderEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$shippingServiceProviderCode</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getShippingServiceProviderClass</strong>(<a target="_blank" href="http://php.net/string">string</a> $methodName):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$methodName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>methodExists</strong>(<a target="_blank" href="http://php.net/string">string</a> $methodName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$methodName</td>
        <td></td>
    </tr>
</table>


# ParcelService<a name="order_parcelservice"></a>
    
## Models<a name="order_parcelservice_models"></a>
### ParcelServiceName<a name="order_models_parcelservicename"></a>

The Parcel Service Name Model


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelService\Models`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ParcelServicePreset<a name="order_models_parcelservicepreset"></a>

The Parcel Service Preset Model


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelService\Models`


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
            <td>The ID of the shipping profile (autoincrement value)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parcelServiceId</td>
            <td>The ID of the shipping service provider</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The back end name of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flag</td>
            <td>The icon of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priority</td>
            <td>The priority of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category</td>
            <td>The category of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>useArticlePorto</td>
            <td>Flag that indicates if the extra shipping charge saved in the item data record is used</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isInsured</td>
            <td>Flag that indicates if the shipping profile is insured</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isExpress</td>
            <td>Flag that indicates if the shipping profile is used for express delivery</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isPostident</td>
            <td>Flag that indicates if the shipping profile includes an authority verification</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isDefaultEnabled</td>
            <td>Flag that indicates if the shipping profile is automatically assigned to new items</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>islandFee</td>
            <td>The extra charge for islands saved in the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isCod</td>
            <td>Flag that indicates Cash on Delivery</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>supportedMultishop</td>
            <td>The clients (stores) that are activated for the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>supportedReferrer</td>
            <td>The order referrers that are activated for the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>subreferrerSupport</td>
            <td>This field is currently without any function.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>excludedPaymentMethods</td>
            <td>The blocked payment methods that are not offered for the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>excludedCustomerGroups</td>
            <td>The blocked customer groups for the shipping profile. Blocked customer groups cannot select the shipping profile during checkout.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingGroup</td>
            <td>The group of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>dispatchIdentifier</td>
            <td>This field is currently without any function.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>auctionType</td>
            <td>The eBay listing type for the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>supportedLoyaltyPrograms</td>
            <td>The loyalty programs that are supported by the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The date the shipping profile was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>parcelServicePresetNames</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>parcelServiceNames</td>
            <td></td>
        </tr><tr>
            <td><a href="order#order_models_parcelservice">ParcelService</a>
</td>
            <td>parcelService</td>
            <td>The parcel service.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ParcelService<a name="order_models_parcelservice"></a>

The Parcel Service Model


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelService\Models`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ParcelServicePresetName<a name="order_models_parcelservicepresetname"></a>

The Parcel Service Preset Name Model


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelService\Models`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ParcelServiceRegion<a name="order_parcelserviceregion"></a>
    
## Contracts<a name="order_parcelserviceregion_contracts"></a>
### ParcelServiceRegionRepositoryContract<a name="order_contracts_parcelserviceregionrepositorycontract"></a>

Get parcel service region


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelServiceRegion\Contracts`



#### Methods

<pre>public <strong>getParcelServiceRegion</strong>(<a target="_blank" href="http://php.net/int">int</a> $parcelServiceRegionId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="order#order_models_parcelserviceregion">ParcelServiceRegion</a>
</pre>

    
Get a parcel service region
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parcelServiceRegionId</td>
        <td>The ID of the parcel service region.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listParcelServiceRegions</strong>(<a target="_blank" href="http://php.net/int">int</a> $parcelServicePresetId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists parcel service regions by parcel service preset id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parcelServicePresetId</td>
        <td>The ID of the parcel service preset.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


## Models<a name="order_parcelserviceregion_models"></a>
### ParcelServiceRegion<a name="order_models_parcelserviceregion"></a>

The parcel service region model.


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelServiceRegion\Models`


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
            <td>The ID of the parcel service region</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingRegionId</td>
            <td>The ID of the shipping region</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parcelServicePresetId</td>
            <td>The ID of the parcel service preset</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingRegionName</td>
            <td>The name of the shipping region</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>serviceType</td>
            <td>Type of the parcel service</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ParcelServiceRegionName<a name="order_models_parcelserviceregionname"></a>

The parcel service region name model.


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelServiceRegion\Models`


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
            <td>The ID of the parcel service region name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>name</td>
            <td>The name of the shipping region</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Countries<a name="order_countries"></a>
    
## Contracts<a name="order_countries_contracts"></a>
### CountryRepositoryContract<a name="order_contracts_countryrepositorycontract"></a>

Repository for Country


#### Namespace

`Plenty\Modules\Order\Shipping\Countries\Contracts`



#### Methods

<pre>public <strong>findIsoCode</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId, <a target="_blank" href="http://php.net/string">string</a> $isoCodeType):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$isoCodeType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCountryById</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId):<a href="order#order_models_country">Country</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCountriesList</strong>(<a target="_blank" href="http://php.net/int">int</a> $active, <a target="_blank" href="http://php.net/array">array</a> $with):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$active</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getActiveCountriesList</strong>():<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    

    
<pre>public <strong>getActiveCountryNameMap</strong>(<a target="_blank" href="http://php.net/string">string</a> $language):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCountryByIso</strong>(<a target="_blank" href="http://php.net/string">string</a> $isoCode, <a target="_blank" href="http://php.net/string">string</a> $isoType):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$isoCode</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$isoType</td>
        <td>('isoCode2', 'isoCode3')</td>
    </tr>
</table>


## Models<a name="order_countries_models"></a>
### Country<a name="order_models_country"></a>

The country model


#### Namespace

`Plenty\Modules\Order\Shipping\Countries\Models`


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
            <td>The country id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The system country name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingDestinationId</td>
            <td>The shipping destination (region) id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>active</td>
            <td>The active flag (1: active, 2: backend active, 3: supplier active</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storehouseId</td>
            <td>The id of the main warehouse in this country.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isoCode2</td>
            <td>The ISO 3166 ALPHA-2 code of the country.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isoCode3</td>
            <td>The ISO 3166 ALPHA-3 code of the country.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The main language spoken in the country.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isCountryStateMandatory</td>
            <td>Flag that states if a country state is mandatory for the country.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>states</td>
            <td>An array with country states.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>An array with country names in different languages.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CountryState<a name="order_models_countrystate"></a>

country state


#### Namespace

`Plenty\Modules\Order\Shipping\Countries\Models`


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
            <td>countryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isoCode</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isoCode3166</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CountryName<a name="order_models_countryname"></a>

country name


#### Namespace

`Plenty\Modules\Order\Shipping\Countries\Models`


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
            <td>language</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Package<a name="order_package"></a>
    
## Contracts<a name="order_package_contracts"></a>
### OrderShippingPackageRepositoryContract<a name="order_contracts_ordershippingpackagerepositorycontract"></a>

Create, get, update and delete order shipping packages.


#### Namespace

`Plenty\Modules\Order\Shipping\Package\Contracts`



#### Methods

<pre>public <strong>getOrderShippingPackage</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderShippingPackageId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="order#order_models_ordershippingpackage">OrderShippingPackage</a>
</pre>

    
Get an order shipping package
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderShippingPackageId</td>
        <td>The ID of the order shipping package</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The properties to be loaded</td>
    </tr>
</table>


<pre>public <strong>listOrderShippingPackages</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List order shipping packages
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The properties to be loaded</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>(optional) Possible value is 'labelBase64' to get the label with the response</td>
    </tr>
</table>


<pre>public <strong>createOrderShippingPackage</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_ordershippingpackage">OrderShippingPackage</a>
</pre>

    
Create an order shipping package
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateOrderShippingPackage</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderShippingPackageId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_ordershippingpackage">OrderShippingPackage</a>
</pre>

    
Update an order shipping package
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderShippingPackageId</td>
        <td>The ID of the order shipping package</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteOrderShippingPackage</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderShippingPackageId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete an order shipping package
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderShippingPackageId</td>
        <td>The ID of the order shipping package</td>
    </tr>
</table>


## Models<a name="order_package_models"></a>
### OrderShippingPackage<a name="order_models_ordershippingpackage"></a>

The order shipping package model


#### Namespace

`Plenty\Modules\Order\Shipping\Package\Models`


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
            <td>The ID of the order shipping package</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packageId</td>
            <td>The ID of the package</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weight</td>
            <td>The weight of the package in grams</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>packageNumber</td>
            <td>The package number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>labelPath</td>
            <td>The path to the label</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>labelBase64</td>
            <td>The base64 encoded label</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packageType</td>
            <td>The type of the package. The following types are valid:
<ul>
<li>0: unpacked</li>
<li>1: Bale</li>
<li>2: Dispenser</li>
<li>3: Coil</li>
<li>4: Roll pallet</li>
<li>5: Colli</li>
<li>6: Container</li>
<li>7: Bucket</li>
<li>8: Cask</li>
<li>9: Bottles</li>
<li>10: European flat pallet</li>
<li>11: Structural frame</li>
<li>12: Gas cylinder</li>
<li>13: Pallet cage</li>
<li>14: Hobbock</li>
<li>15: Half pallet</li>
<li>16: Pallet of food items</li>
<li>17: Wooden coaster</li>
<li>18: IBC container</li>
<li>19: Pitcher</li>
<li>20: Wicker bottle</li>
<li>21: Case</li>
<li>22: Canister</li>
<li>23: Customer pallet</li>
<li>24: Cardboard box</li>
<li>25: Composite packaging</li>
<li>26: Package</li>
<li>27: Ring</li>
<li>28: Role</li>
<li>29: Sack</li>
<li>30: units</li>
<li>31: Tank</li>
<li>32: Drum</li>
<li>34: Crate</li>
<li>35: Quarter pallet</li>
<li>36: Other pallets</li>
<li>37: Bin</li>
<li>38: One-way pallet</li>
<li>39: Foil bag</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>volume</td>
            <td>The volume of the package</td>
        </tr><tr>
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order the package belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# PackageType<a name="order_packagetype"></a>
    
## Contracts<a name="order_packagetype_contracts"></a>
### ShippingPackageTypeRepositoryContract<a name="order_contracts_shippingpackagetyperepositorycontract"></a>

The ShippingPackageTypeRepositoryContract is the interface for the shipping package type repository. This interface allows to list all shipping package types or to get a shipping package type by the ID.


#### Namespace

`Plenty\Modules\Order\Shipping\PackageType\Contracts`



#### Methods

<pre>public <strong>findShippingPackageTypeById</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingPackageTypeId):<a href="order#order_models_shippingpackagetype">ShippingPackageType</a>
</pre>

    
Gets a shipping package type. The ID of the shipping package type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingPackageTypeId</td>
        <td>The ID of the shipping package type</td>
    </tr>
</table>


<pre>public <strong>listShippingPackageTypes</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists shipping packages types.
    
## Models<a name="order_packagetype_models"></a>
### ShippingPackageType<a name="order_models_shippingpackagetype"></a>

The shipping package type model.


#### Namespace

`Plenty\Modules\Order\Shipping\PackageType\Models`


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
            <td>The ID of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>width</td>
            <td>The width of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>height</td>
            <td>The height of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>length</td>
            <td>The length of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>unit</td>
            <td>The unit of the shipping package type dimension</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxWeight</td>
            <td>The maximum weight of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxVolume</td>
            <td>The maximum volume of the shipping package type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>volumeType</td>
            <td>The volume type of the shipping package type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Contact<a name="order_contact"></a>
    
## Contracts<a name="order_contact_contracts"></a>
### CouponCodeContactRepositoryContract<a name="order_contracts_couponcodecontactrepositorycontract"></a>

This is the contract for the coupon codes by contacts repository. It allows you to list coupon codes redeemed by a contact as well as to create, update and delete redeemed coupon codes.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Contact\Contracts`



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_couponcodecontact">CouponCodeContact</a>
</pre>

    
Create redeemed coupons for a contact.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The redeemed coupon data. The properties that are required to create an entry can be found in the CouponCodeContact model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $campaignId, <a target="_blank" href="http://php.net/string">string</a> $coupon, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_couponcodecontact">CouponCodeContact</a>
</pre>

    
Update a redeemed coupon of a contact.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact that redeemed the coupon code</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$campaignId</td>
        <td>The ID of the coupon campaign</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$coupon</td>
        <td>The coupon code</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The redeemed coupon data. The properties that are required to update an entry can be found in the CouponCodeContact model</td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $campaignId, <a target="_blank" href="http://php.net/string">string</a> $coupon):<a href="order#order_models_couponcodecontact">CouponCodeContact</a>
</pre>

    
Get a redeemed coupon for a contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact which redeemed the coupon code</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$campaignId</td>
        <td>The ID of the coupon campaign</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$coupon</td>
        <td>The coupon code</td>
    </tr>
</table>


<pre>public <strong>findByContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List redeemed coupons for a contact
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The contact ID as filter for redeemed coupons.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of coupons to be displayed per page. The default number of coupons per page is 50.</td>
    </tr>
</table>


<pre>public <strong>findByCampaign</strong>(<a target="_blank" href="http://php.net/int">int</a> $campaignId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List redeemed coupons of a campaign.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$campaignId</td>
        <td>The campaign ID as filter for redeemed coupons.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of coupons to be displayed per page. The default number of coupons per page is 50.</td>
    </tr>
</table>


<pre>public <strong>findByCoupon</strong>(<a target="_blank" href="http://php.net/string">string</a> $coupon, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List redeemed coupons of a coupon code
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$coupon</td>
        <td>The coupon code</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of coupons to be displayed per page. The default number of coupons per page is 50.</td>
    </tr>
</table>


## Models<a name="order_contact_models"></a>
### CouponCodeContact<a name="order_models_couponcodecontact"></a>

The CouponCodeContact model.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Contact\Models`


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
            <td>The coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact that redeemed the coupon</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>openAmount</td>
            <td>The coupon amount that can still be redeemed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>redeemCount</td>
            <td>How many times a coupon code has already been redeemed</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the coupon code was updated last.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>campaignId</td>
            <td>The ID of the campaign that the coupon belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>externalTransactionId</td>
            <td>The ID that is assigned to a coupon by the external coupon service provider, when the coupon is redeemed.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Code<a name="order_code"></a>
    
## Contracts<a name="order_code_contracts"></a>
### CouponCodeRepositoryContract<a name="order_contracts_couponcoderepositorycontract"></a>

The CouponCodeRepositoryContract is the interface for the coupon code repository. This interface allows you to redeem coupons.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Contracts`



#### Methods

<pre>public <strong>redeem</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $coupon):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Redeem coupon codes
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$coupon</td>
        <td>The coupon code to be redeemed</td>
    </tr>
</table>



### CouponCampaignCodeRepositoryContract<a name="order_contracts_couponcampaigncoderepositorycontract"></a>

This interface allows you to get and create coupon codes.


#### Namespace

`Plenty\Modules\Order\Coupon\Campaign\Code\Contracts`



#### Methods

<pre>public <strong>getByCode</strong>(<a target="_blank" href="http://php.net/string">string</a> $code):<a href="order#order_models_couponcampaigncode">CouponCampaignCode</a>
</pre>

    
Gets a coupon code. The code string must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_couponcampaigncode">CouponCampaignCode</a>
</pre>

    
Creates a coupon code. The ID of the campaign must be specified. A code can optionally be specified. A random code will be generated if the code is not specified. A coupon value can also be optionally specified. The value of the campaign will be used if no individual value is specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Models<a name="order_code_models"></a>
### CouponCampaignCode<a name="order_models_couponcampaigncode"></a>

The CouponCampaignCode model contains information about coupon codes. Each code belongs to one campaign only.


#### Namespace

`Plenty\Modules\Order\Coupon\Campaign\Code\Models`


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
            <td>The coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>campaignId</td>
            <td>The ID of the campaign that the code belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>disable</td>
            <td>Flag that indicates if a code is active or deactivated.
<ul><li>True = the code is deactivated</li>
	<li>False = the code is active</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>consumed</td>
            <td>Flag that indicates if a code was redeemed or not.
<ul><li>True = the code was redeemed</li>
	<li>False = the code is not redeemed</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>usedCount</td>
            <td>How many times a code has been redeemed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>usedAmount</td>
            <td>The amount that is already redeemed. The total amount that can be redeemed is defined in the campaign as coupon value, because the value applies to all codes of a campaign.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>generatedAt</td>
            <td>The date and time that the code was generated</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>lastUsedAt</td>
            <td>The date and time that the code was redeemed last. This date will be set if the coupon amount has not been fully used.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>consumedAt</td>
            <td>The date and time that the coupon amount of this code was fully consumed</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>expiresAt</td>
            <td>The date and time that the code will expire or has expired</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The value of the coupon if it differs from the campaign value. The value is null if the campaign value is used.</td>
        </tr><tr>
            <td><a href="order#order_models_couponcampaign">CouponCampaign</a>
</td>
            <td>campaign</td>
            <td>The coupon campaign and all information about the campaign that this code belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Validation<a name="order_validation"></a>
    
## Contracts<a name="order_validation_contracts"></a>
### CouponCodeValidatorContract<a name="order_contracts_couponcodevalidatorcontract"></a>

CouponCodeValidatorContract is the interface for the coupon code validation repository. This interface provides the functionality to validate coupon data.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Validation\Contracts`



#### Methods

<pre>public <strong>validate</strong>(<a href="order#order_models_couponcodevalidation">CouponCodeValidation</a>
 $validationData):<a href="order#order_models_couponcodevalidation">CouponCodeValidation</a>
</pre>

    
Validate a coupon code
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_couponcodevalidation">CouponCodeValidation</a>
</td>
        <td>$validationData</td>
        <td>The data to validate a coupon</td>
    </tr>
</table>


## Models<a name="order_validation_models"></a>
### CouponCodeValidation<a name="order_models_couponcodevalidation"></a>

The CouponCodeValidation data model contains all data necessary for validating a coupon.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Validation\Models`


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
            <td>campaignId</td>
            <td>The ID of the campaign</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>validationType</td>
            <td>The type of the campaign. Currently the only type available is plentymarkets.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>items</td>
            <td>The list of items or variations to be validated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact that wants to redeem the coupon</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>couponCode</td>
            <td>The coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency of the purchase</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrer</td>
            <td>The order referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>salesDiscount</td>
            <td>The total discount from a coupon applied to an order. The discount is given as gross amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>salesDiscountNet</td>
            <td>The net discount from a coupon applied to an order. The net discount is the total discount minus the vat amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>itemDiscount</td>
            <td>The discount amount applied to items.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>itemDiscountNet</td>
            <td>The net discount applied to items.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>shippingDiscount</td>
            <td>The discount applied to shipping costs.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>shippingDiscountNet</td>
            <td>The net discount applied to shipping costs.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>usedVatFields</td>
            <td>The vat fields used for the validation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>restCouponAmount</td>
            <td>The remaining coupon amount</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>checkedItems</td>
            <td>The list of variations that passed the validation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>validateParams</td>
            <td>Validation parameters</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CouponCodeValidationItem<a name="order_models_couponcodevalidationitem"></a>

The CouponCodeValidationItem model contains all item data needed for validating whether the coupon can be redeemed for these items or not.


#### Namespace

`Plenty\Modules\Order\Coupon\Code\Validation\Models`


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
            <td>amount</td>
            <td>The price of a variation multiplied by the quantity</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>noCoupon</td>
            <td>Flag that indicates whether a variation can be bought with a coupon, can exclusively be bought with a coupon or can not be bought with a coupon.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The quantity of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>singlePrice</td>
            <td>The price of a single variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatField</td>
            <td>The field of the VAT rate</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Campaign<a name="order_campaign"></a>
    
## Models<a name="order_campaign_models"></a>
### CouponCampaign<a name="order_models_couponcampaign"></a>

The CouponCampaign model contains all information of a campaign.


#### Namespace

`Plenty\Modules\Order\Coupon\Campaign\Models`


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
            <td>The ID of a coupon campaign</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td>DEPRECATED! The external ID of a coupon campaign</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the coupon campaign</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variable</td>
            <td>The variable to display coupon codes in emails. There are only 10 variables available. A variable may only be used for one campaign. The variable names follow this pattern: CouponCode + Number e.g. CouponCode1.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPermittedForExternalReferrers</td>
            <td>Flag that indicates whether or not coupons can be redeemed if a customer enters the online store from an external referrer.
<ul><li>TRUE = The coupon can be redeemed if the customer enters the online store from an external referrer </li>
<li>FALSE = The coupon can not be redeemed</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>includeShipping</td>
            <td>The discount also applies to shipping costs. The property will be only be set if the discount type fixed is set.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unusedCodesCount</td>
            <td>The number of codes that have been redeemed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>usedCodesCount</td>
            <td>The number of codes that have not been redeemed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>endsAt</td>
            <td>The date that the campaign ends</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>startsAt</td>
            <td>The date that the campaign starts</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minOrderValue</td>
            <td>The minimum order value that needs to be reached for the coupon to be redeemed. If the value is not reached the coupon will not be redeemed.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>codeDurationWeeks</td>
            <td>The number of weeks that codes of this campaign can be redeemed after they have been generated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>codeAssignment</td>
            <td>The code assignment is only relevant for vouchers. Codes can either be generated every time a voucher is bought or a code from a previously created list of codes can be used. The two options available are generate and use_existing.
<ul><li>generate = a new code is generated on demand</li>
<li>use_existing = the code already exists and is taken from a previously entered list of codes</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>codeLength</td>
            <td>There are 3 different length available. The code can be 6, 16 or 24 characters long.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>usage</td>
            <td>The usage defines what the coupon codes from this campaign can be used for. There are three options available:
<ul><li>single_and_subscription = The codes can be used for single orders and subscription orders</li>
<li>single_order = The codes can be used for single orders only</li>
<li>subscription = The codes can be used for subscriptions only</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>concept</td>
            <td>The campaign concept defines how many codes belong to a campaign. The concept interacts with the redeem type that is explained next. There are two concept options available:
<ul><li>single_code = The campaign has only one code</li>
<li>multi_code = The campaign has several codes</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>redeemType</td>
            <td>The redeem type defines how many times a code of a campaign can be redeemed. There are 4 redeem types available:
<ul><li>multi_redeem_per_user = Each customer is allowed to redeem the same code several times</li>
<li>single_redeem_per_user =  Each customer can only redeem the same code once</li>
<li>redeem_until_value_reached = A code can be entered several times by the same customer or by different customers, but only until the coupon value is depleted</li>
<li>unique_redeem = The code can be redeemed once. If several customers get the same code, only the first customer to enter the code can use it.</li></ul>
The redeem type interacts with the concept. Pay attention to the combination these two options form.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>discountType</td>
            <td>There are 4 discount types available:
<ul><li>fixed = The coupon value is a fixed amount of money. This discount type is the only one that makes sense for coupons that are sold in the online store. The actual amount of money needs to be set with the value property.</li>
<li>percent = The discount is given as percentage and the actual value depends on the purchase. The actual number of percent need to be set with the value property.</li>
<li>item = The discount applies to entire items. A typical example would be - Buy 1 get 1 free - or in other words - Get 2 for the price of 1. The number of items the customer gets and the number of items the customer has to pay for need to be set with itemDiscountToPay and itemDiscountToBuy.</li>
<li>shipping = The shipping does not cost anything. The cost will be set to zero no matter what the actual shipping costs are.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemDiscountToPay</td>
            <td>The number of items that the customer has to pay for. This number needs to be compared to the number of items the customer receives, itemDiscountToBuy</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemDiscountToBuy</td>
            <td>The number of items that the customer receives, but he or she only has to pay for the number of items set with itemDiscountToPay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>campaignType</td>
            <td>The two campaign types available are coupon or voucher.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>couponType</td>
            <td>The coupon type is only for campaigns that have the campaign type coupon. The two coupon types available are promotion and sales.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the campaign</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The actual discount value of a coupon. The value needs to be set for the two discount types fixed and percent.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>codes</td>
            <td>The codes and information about the codes that belong to this CouponCampaign</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Address<a name="order_address"></a>
    
## Contracts<a name="order_address_contracts"></a>
### OrderAddressRepositoryContract<a name="order_contracts_orderaddressrepositorycontract"></a>

The OrderAddressRepositoryContract is the interface for the order address repository. This interface allows you to get, create, update and delete addresses of an order.


#### Namespace

`Plenty\Modules\Order\Address\Contracts`



#### Methods

<pre>public <strong>findAddressByType</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Get an address of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>findSchedulerAddressByType</strong>(<a target="_blank" href="http://php.net/int">int</a> $schedulerId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Get an address of a scheduler order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$schedulerId</td>
        <td>The ID of the scheduler</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type</td>
    </tr>
</table>


<pre>public <strong>createOrderAddress</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId = \Plenty\Modules\Account\Address\Models\AddressRelationType::BILLING_ADDRESS):<a href="account#account_models_address">Address</a>
</pre>

    
Create an address for an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>[optional] The ID of the address type. The default ID is 1 for billing address. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>updateOrderAddress</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Update an address of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The address data</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>getAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="account#account_models_address">Address</a>
</pre>

    
Get an address
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the address instance. The relations available are "options", "contacts", "orders", "country".</td>
    </tr>
</table>


<pre>public <strong>findAddresses</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
List addresses of an an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>getAddressOfOrder</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Get an address of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>getAddressOfScheduler</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $schedulerId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="account#account_models_address">Address</a>
</pre>

    
Get an address of a scheduler
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$schedulerId</td>
        <td>The ID of the scheduler</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>addOrderAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create an address relation from an order to an address
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>addSchedulerAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $schedulerId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create an address relation from a scheduler to an address
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$schedulerId</td>
        <td>The ID of the scheduler</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>deleteOrderAddress</strong>(<a target="_blank" href="http://php.net/int">int</a> $addressId, <a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an address relation from an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$addressId</td>
        <td>The ID of the address</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the address type. The types available are:

<ul>
<li>Billing address = 1</li>
<li>Delivery address = 2</li>
<li>Sender address = 3</li>
<li>Return address = 4</li>
<li>Client address = 5</li>
<li>Contractor address = 6</li>
<li>Warehouse address = 7</li>
</ul></td>
    </tr>
</table>


# StatusHistory<a name="order_statushistory"></a>
    
## Contracts<a name="order_statushistory_contracts"></a>
### StatusHistoryRepositoryContract<a name="order_contracts_statushistoryrepositorycontract"></a>

This interface allows you to get the status history of an order and to list the status histories of all orders.


#### Namespace

`Plenty\Modules\Order\StatusHistory\Contracts`



#### Methods

<pre>public <strong>getStatusHistoryByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Get the status history of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to get</td>
    </tr>
</table>


<pre>public <strong>getStatusHistory</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List status histories
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to get</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries from status histories listed per page</td>
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
    
## Models<a name="order_statushistory_models"></a>
### StatusHistoryEntry<a name="order_models_statushistoryentry"></a>

The status history entry model


#### Namespace

`Plenty\Modules\Order\StatusHistory\Models`


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
            <td>The ID of the status history entry</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>statusId</td>
            <td>The ID of the status</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the entry was created</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>procedureText</td>
            <td>The information text of the procedure that created the entry</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Documents<a name="order_documents"></a>
    
## Contracts<a name="order_documents_contracts"></a>
### OrderDocumentStorageContract<a name="order_contracts_orderdocumentstoragecontract"></a>

Provides methods to store, get and delete order document files. The files are stored on an AWS S3 storage by default. The implementation for this contract can be replaced by your own implementation.


#### Namespace

`Plenty\Modules\Order\Documents\Contracts`



#### Methods

<pre>public <strong>fileExists</strong>(<a target="_blank" href="http://php.net/string">string</a> $path):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Check if the file path exists on the storage.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td>The file path</td>
    </tr>
</table>


<pre>public <strong>put</strong>(<a target="_blank" href="http://php.net/string">string</a> $path, <a target="_blank" href="http://php.net/string">string</a> $file):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Store a file on the storage.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td>The file path</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$file</td>
        <td>The file to store. Can be either a file path on the file system or an object.</td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $path):<a href="cloud#cloud_models_storageobject">StorageObject</a>
</pre>

    
Get a file from the storage
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td>The file path</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $path):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a file from the storage.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$path</td>
        <td>The file path</td>
    </tr>
</table>


# SerialNumber<a name="order_serialnumber"></a>
    
## Contracts<a name="order_serialnumber_contracts"></a>
### OrderSerialNumberRepositoryContract<a name="order_contracts_orderserialnumberrepositorycontract"></a>

List serial numbers for orders


#### Namespace

`Plenty\Modules\Order\SerialNumber\Contracts`



#### Methods

<pre>public <strong>listSerialNumbersByOrder</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List serial numbers of an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>listSerialNumbersByOrderItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderItemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List serial numbers if an order item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item</td>
    </tr>
</table>


## Models<a name="order_serialnumber_models"></a>
### OrderSerialNumber<a name="order_models_orderserialnumber"></a>

The order serial number model


#### Namespace

`Plenty\Modules\Order\SerialNumber\Models`


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
            <td>serialNumberId</td>
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
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>serialNumber</td>
            <td>The serial number</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Idea<a name="order_idea"></a>
    
## Models<a name="order_idea_models"></a>
### Export<a name="order_models_export"></a>

The export model for IDEA exports.


#### Namespace

`Plenty\Modules\Order\Export\Pos\Idea\Models`


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
            <td>The id of the export entry.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>token</td>
            <td>The token generated for the export entry.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>progress</td>
            <td>The progress of the export process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currentModule</td>
            <td>The currently exporting module of the export process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>state</td>
            <td>The current state of the export process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>filename</td>
            <td>The filename of the export content.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>createdAt</td>
            <td>Specifies the creation date of the export entry.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>updatedAt</td>
            <td>Specifies the last update date of the export entry.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>modules</td>
            <td>The modules to be used by the export process.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>options</td>
            <td>The options for the export process. Currently only "year" is supported as option key.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Events<a name="order_events"></a>
    
## Created<a name="order_events_created"></a>
### CreditNoteCreated<a name="order_created_creditnotecreated"></a>

An event class fired after a new credit note is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### WarrantyCreated<a name="order_created_warrantycreated"></a>

An event class fired after a new warranty is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### ReturnCreated<a name="order_created_returncreated"></a>

An event class fired after a new returns is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### MultiCreditNoteCreated<a name="order_created_multicreditnotecreated"></a>

An event class fired after a new multi credit note is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### SalesOrderCreated<a name="order_created_salesordercreated"></a>

An event class fired after a new sales order is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### DeliveryOrderCreated<a name="order_created_deliveryordercreated"></a>

An event class fired after a new delivery order is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### RepairCreated<a name="order_created_repaircreated"></a>

An event class fired after a new repair is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### MultiOrderCreated<a name="order_created_multiordercreated"></a>

An event class fired after a new multi order is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    
## Canceled<a name="order_events_canceled"></a>
### BeforeOrderCanceled<a name="order_canceled_beforeordercanceled"></a>

An event class fired before an order will be canceled.


#### Namespace

`Plenty\Modules\Order\Events\Canceled`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    

### AfterOrderCanceled<a name="order_canceled_afterordercanceled"></a>

An event class fired after an order is canceled.


#### Namespace

`Plenty\Modules\Order\Events\Canceled`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderEvent constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    
## Changed<a name="order_events_changed"></a>
### OrderStatusChanged<a name="order_changed_orderstatuschanged"></a>

An event class fired after the status of an order has changed.


#### Namespace

`Plenty\Modules\Order\Events\Changed`



#### Methods

<pre>public <strong>__construct</strong>(<a href="order#order_models_order">Order</a>
 $order, <a target="_blank" href="http://php.net/float">float</a> $oldStatus):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
OrderStatusChanged constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$oldStatus</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOldStatus</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>

    
Get the old order status.
    
<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order instance.
    
# Currency<a name="order_currency"></a>
    
## Contracts<a name="order_currency_contracts"></a>
### CurrencyRepositoryContract<a name="order_contracts_currencyrepositorycontract"></a>

Provides methods for currency data.


#### Namespace

`Plenty\Modules\Order\Currency\Contracts`



#### Methods

<pre>public <strong>getCurrency</strong>(<a target="_blank" href="http://php.net/string">string</a> $currencyIso, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="order#order_models_currency">Currency</a>
</pre>

    
Get a currency
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currencyIso</td>
        <td>The currency ISO 4217 code, e.g. "EUR".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded in the currency instance.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded in the currency instance. Valid relations are "names" or "countries").</td>
    </tr>
</table>


<pre>public <strong>getCurrencyList</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get all currencies supported in the system.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded in the currency instances.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded in the currency instance. Valid relations are "names" or "countries".</td>
    </tr>
</table>


<pre>public <strong>getCurrencyCountries</strong>(<a target="_blank" href="http://php.net/string">string</a> $currencyIso, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List countries for a currency
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currencyIso</td>
        <td>The currency ISO 4217 code, e.g. "EUR".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded in the country instances.</td>
    </tr>
</table>


<pre>public <strong>getCountryCurrency</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="order#order_models_currency">Currency</a>
</pre>

    
Get a currency for a country
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td>The country id.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes to be loaded in the currency instance.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded in the currency instance ("names" or "countries").</td>
    </tr>
</table>


## Models<a name="order_currency_models"></a>
### CurrencyName<a name="order_models_currencyname"></a>

The currency name model.


#### Namespace

`Plenty\Modules\Order\Currency\Models`


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
            <td>The ID of the currency name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the currency name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name in the language</td>
        </tr><tr>
            <td><a href="order#order_models_currency">Currency</a>
</td>
            <td>currencyInstance</td>
            <td>The currency instance.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Currency<a name="order_models_currency"></a>

The currency model. The model includes information like the ISO 4217 code and the related currency symbols as well as the countries that a currency is used in.


#### Namespace

`Plenty\Modules\Order\Currency\Models`


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
            <td>currency</td>
            <td>The ISO 4217 code and id of the currency.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>htmlCode</td>
            <td>The html code (entity) for the currency.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>unicodeSign</td>
            <td>The unicode symbol for the currency. If no unicode symbol exists, the html code will be used.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isActive</td>
            <td>Flag that indicates if the currency is active in the system or not. Currencies are activated per sales price.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if this currency can be deleted or not. <ul><li>False = Currency cannot be deleted</li><li>True = Currency can be deleted</li></ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>countries</td>
            <td>A list of countries that use the currency.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>A list of names in different languages for the currency.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CurrencyCountryRelation<a name="order_models_currencycountryrelation"></a>

The CurrencyCountryRelation model indicates which currency is related to which country.


#### Namespace

`Plenty\Modules\Order\Currency\Models`


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
            <td>The ID of the relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The ID of the country</td>
        </tr><tr>
            <td><a href="order#order_models_country">Country</a>
</td>
            <td>country</td>
            <td>The related country information</td>
        </tr><tr>
            <td><a href="order#order_models_currency">Currency</a>
</td>
            <td>currencyInstance</td>
            <td>The related currency information</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Referrer<a name="order_referrer"></a>
    
## Contracts<a name="order_referrer_contracts"></a>
### OrderReferrerRepositoryContract<a name="order_contracts_orderreferrerrepositorycontract"></a>

Provides methods for processing order referrers. An order referrer indicates where a purchase was made originally. 


#### Namespace

`Plenty\Modules\Order\Referrer\Contracts`



#### Methods

<pre>public <strong>getList</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List order referrers
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns (attributes) to load in the instances.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/float">float</a> $parentReferrerId = null):<a href="order#order_models_orderreferrer">OrderReferrer</a>
</pre>

    
Create an order referrer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order referrer data. The properties that are required to create an order referrer can be found in the order referrer model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$parentReferrerId</td>
        <td>If a parent referrer ID is specified, the new referrer will be created as a sub referrer to this one and will be assigned a sub referrer ID. Sub referrer IDs are build of an integer part and a fractional part. The integer part is the parent ID followed by a 2 character long fractional part. This way the relation between a sub referrer and the parent referrer can be seen easily.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/float">float</a> $referrerId):<a href="order#order_models_orderreferrer">OrderReferrer</a>
</pre>

    
Update an order referrer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order referrer data. The properties that are required to update an order referrer can be found in the order referrer model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td>The ID of the order referrer</td>
    </tr>
</table>


<pre>public <strong>getReferrerById</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrerId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="order#order_models_orderreferrer">OrderReferrer</a>
</pre>

    
Get an order referrer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td>The ID of the order referrer</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns (attributes) to load in the instances.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrerId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an order referrer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td>The ID of the order referrer</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="order_referrer_models"></a>
### OrderReferrer<a name="order_models_orderreferrer"></a>

The order referrer model. An order referrer shows where a purchase was originally made.


#### Namespace

`Plenty\Modules\Order\Referrer\Models`


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
            <td>id</td>
            <td>The ID of the order referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isEditable</td>
            <td>Flag that indicates if this referrer can be updated as well as deleted or not
<ul><li>True = the referrer can be edited and deleted</li>
<li>False = the referrer can neither be edited nor deleted</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The backend name of the referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The public name of the referrer as it is displayed e.g. on documents</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderOwnerId</td>
            <td>The user ID of whoever owns new orders from this referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isFilterable</td>
            <td>Flag that indicates if this referrer can be used as a filter or not
<ul><li>True = Can be used as a filter</li>
<li>False = Cannot be used as a filter</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>origin</td>
            <td>The origin of this referrer</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
