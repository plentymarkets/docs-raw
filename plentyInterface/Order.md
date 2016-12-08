

# Order<a name="order_order"></a>
    
## Contracts<a name="order_order_contracts"></a>
### OrderItemRepositoryContract<a name="order_contracts_orderitemrepositorycontract"></a>

The OrderItemRepositoryContract is the interface for the order item repository. This interface allows you to find, create and update order items. An order item can be e.g. items, surcharges and coupons. Each order item is given a unique id, which links it to a specific order.


#### Namespace

`Plenty\Modules\Order\Contracts`



#### Methods

<pre>public <strong>deleteOrderItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $orderItemId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes an order item. The order ID and the order item ID have to be provided.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order the item belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderItemId</td>
        <td>The ID of the order item to be deleted.</td>
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
        <td>The relations to load in the order instance, one of "address", "events", "dates", "relation", "reference", "comments".</td>
    </tr>
</table>


<pre>public <strong>createOrder</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="order#order_models_order">Order</a>
</pre>

    
Create an order
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order data. The properties that are required to create an order can be found in the order model.</td>
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
        <td>The relations to load in the Order instance. Valid are "address", "events", "dates", "relation", "reference", "comments".</td>
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
        <td>The relations to load in the Order instance. The relations available are: "address", "events", "dates", "relation", "reference" and "comments".
                             If you want to load relations, you need to include at least one, but you can also include several or all.</td>
    </tr>
</table>


<pre>public <strong>searchOrders</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List orders by filter options
    
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
        <td>The relations to load in the Order instance. Valid are "address", "events", "dates", "relation", "reference".</td>
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


## Events<a name="order_order_events"></a>
### OrderCreated<a name="order_events_ordercreated"></a>

An event class fired after a new order is created. The order type is not relevant.
 * 	At the same time also type depended events will be fired, like ReturnsCreated or CreditNoteCreated.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderEvent<a name="order_events_orderevent"></a>

A base event class for all order events. Each order event expects an order instance.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderFullyPaid<a name="order_events_orderfullypaid"></a>

An Event class fired after a payment assignment when the order is fully paid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderOverpaid<a name="order_events_orderoverpaid"></a>

An Event class fired after a payment assignment when the order is overpaid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPaidEvent<a name="order_events_orderpaidevent"></a>

A base Event class for all order paid events.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPartlyPaid<a name="order_events_orderpartlypaid"></a>

An Event class fired after a payment assignment when the order is partly paid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPaymentAssigned<a name="order_events_orderpaymentassigned"></a>

An Event class fired after a payment was assigned to an order.
 * After this event one of the following events will be fired, depending the payment status of the order:
 *	 OrderPrepaid, OrderPartlyPaid, OrderFullyPaid, OrderOverpaid.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPrepaid<a name="order_events_orderprepaid"></a>

An Event class fired after a payment assignment when the order is paid in advance.


#### Namespace

`Plenty\Modules\Order\Events`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Models<a name="order_order_models"></a>
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
            <td>The order ID</td>
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
            <td>The ID of the order's payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingProfileId</td>
            <td>The ID of the order's shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paymentStatus</td>
            <td>The payment status of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>statusId</td>
            <td>The ID of the order status</td>
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
            <td>The id of the order  amount.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The id of the order that the amount belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSystemCurrency</td>
            <td>Flag that states if the current currency is the same as system currency or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isNet</td>
            <td>Flag that states if the invoice is net or not.</td>
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
            <td>The surcharge gross price.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>prepaidAmount</td>
            <td>The discount amount. This amount can be a percentage or a fixed value.</td>
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
            <td>The id of the order amount vat.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderAmountId</td>
            <td>The id of the order amount that the vat belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryVatId</td>
            <td>The id of the country vat that the vat belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatField</td>
            <td>The vat id used [0,1,2,3].</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatRate</td>
            <td>The actual vat rate that was used, e.g. 19%.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The vat amount of money given in the order amount currency.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the vat was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the vat was updated last.</td>
        </tr><tr>
            <td><a href="order#order_models_orderamount">OrderAmount</a>
</td>
            <td>orderAmount</td>
            <td>The OrderAmount model this OrderAmountVat belongs to.</td>
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
            <td>The item order name (description)</td>
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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>amounts</td>
            <td>The order item amounts that are associated with the order item.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td>The order item property that are associated with the order item.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>orderProperties</td>
            <td>The order item order properties that are associated with the order item.</td>
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
            <td>Flag that states if the current currency is the same as the system currency or not.</td>
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
            <td>Flag that states if a discount is given as a percentage or as a fixed value.</td>
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
    

### OrderItemOrderProperty<a name="order_models_orderitemorderproperty"></a>

This model holds the order properties that are assigned to order items.


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
            <td>The URL of the oder property</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderItemProperty<a name="order_models_orderitemproperty"></a>

The order item property model.


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
<li>WAREHOUSE		=	1</li>
<li>SHIPPING_PROFILE	=	2</li>
<li>CATEGORY			=	3</li>
<li>WEIGHT			=	4</li>
<li>WIDTH			=	5</li>
<li>LENGTH			=	6</li>
<li>HEIGHT			=	7</li>
<li>QUANTITY			=	8</li>
<li>MARKET			=	9</li>
<li>VARIANT			=	10</li>
<li>POSITION			=	11</li>
<li>TOKEN			=	12</li>
<li>METHOD_OF_PAYMENT=	13</li>
<li>IDENTIFIER		=	14</li>
<li>DUNNING			=	15</li>
<li>ORDER			=	16</li>
<li>DOCUMENT			=	17</li>
<li>PROPERTY			=	18</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>subTypeId</td>
            <td>The ID of the property subtype
<ul>
<li>MAIN_VALUE		=	1</li>
<li>ORIGINAL_VALUE	=	2</li>
<li>STATUS			=	3</li>
<li>SURCHARGE		=	4</li>
<li>TYPE				=	5</li>
<li>EXTERNAL			=	6</li>
<li>NAME				=	7</li>
<li>CONTENT			=	8</li>
<li>ACCOUNT			=	9</li>
<li>FLAG				=	10</li>
<li>LANGUAGE			=	11</li>
<li>CONSUMER			=	12</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property. The value depends on type/subtype.</td>
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
        </tr><tr>
            <td><a href="order#order_models_orderpropertysubtype">OrderPropertySubType</a>
</td>
            <td>subType</td>
            <td>The subtype of the property.</td>
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
            <td>The ID of the order item type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
            <td>isErasable</td>
            <td>Flag that states if this type can be deleted or not</td>
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
            <td>The type name id.</td>
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
            <td>The type name's language.</td>
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
    

### OrderProperty<a name="order_models_orderproperty"></a>

The order properties model. Each order property has a type and can have an additional sub-type.


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
            <td>The order property id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The id of the order that the property belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The property type id.
<ul>
<li>WAREHOUSE		=	1</li>
<li>SHIPPING_PROFILE	=	2</li>
<li>CATEGORY			=	3</li>
<li>WEIGHT			=	4</li>
<li>WIDTH			=	5</li>
<li>LENGTH			=	6</li>
<li>HEIGHT			=	7</li>
<li>QUANTITY			=	8</li>
<li>MARKET			=	9</li>
<li>VARIANT			=	10</li>
<li>POSITION			=	11</li>
<li>TOKEN			=	12</li>
<li>METHOD_OF_PAYMENT=	13</li>
<li>IDENTIFIER		=	14</li>
<li>DUNNING			=	15</li>
<li>ORDER			=	16</li>
<li>DOCUMENT			=	17</li>
<li>PROPERTY			=	18</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>subTypeId</td>
            <td>The property sub-type id.
<ul>
<li>MAIN_VALUE		=	1</li>
<li>ORIGINAL_VALUE	=	2</li>
<li>STATUS			=	3</li>
<li>SURCHARGE		=	4</li>
<li>TYPE				=	5</li>
<li>EXTERNAL			=	6</li>
<li>NAME				=	7</li>
<li>CONTENT			=	8</li>
<li>ACCOUNT			=	9</li>
<li>FLAG				=	10</li>
<li>LANGUAGE			=	11</li>
<li>CONSUMER			=	12</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property. The value depends on type/sub-type.</td>
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
        </tr><tr>
            <td><a href="order#order_models_orderpropertytype">OrderPropertyType</a>
</td>
            <td>type</td>
            <td>The property type.</td>
        </tr><tr>
            <td><a href="order#order_models_orderpropertysubtype">OrderPropertySubType</a>
</td>
            <td>subType</td>
            <td>The property sub-type.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPropertySubType<a name="order_models_orderpropertysubtype"></a>

The order property sub-type model


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
            <td>The ID of the property sub-type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
            <td>isErasable</td>
            <td>Flag that states if this type can be deleted or not</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The names of the order property sub-types</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPropertySubTypeName<a name="order_models_orderpropertysubtypename"></a>

The order property sub type name model


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
            <td>The ID of the sub type name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>subTypeId</td>
            <td>The ID of the sub type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the sub type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the  sub type name</td>
        </tr><tr>
            <td><a href="order#order_models_orderpropertysubtype">OrderPropertySubType</a>
</td>
            <td>subType</td>
            <td>The sub type instance.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPropertyType<a name="order_models_orderpropertytype"></a>

The order property type model. Each order has a type and can have an additional sub-type.


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
            <td>The ID of the property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
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
            <td>The names of the order property types</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderPropertyTypeName<a name="order_models_orderpropertytypename"></a>

The order property type name model.


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
            <td>The type name id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the type name.</td>
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
    

### OrderRelationReference<a name="order_models_orderrelationreference"></a>

The order relation reference model specifies how references and orders are related to one another.


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
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
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
            <td>The type name id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the type name.</td>
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
    
## Services<a name="order_order_services"></a>
### OrderCreatedTypeService<a name="order_services_ordercreatedtypeservice"></a>

(Un)Register event classes extending OrderCreated for custom order types.


#### Namespace

`Plenty\Modules\Order\Services`



#### Methods

<pre>public <strong>handle</strong>(<a href="order#order_events_ordercreated">OrderCreated</a>
 $created):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Handle the OrderCreated event by detecting the subevent to fire according the order type id of the order.
    
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

    
Add an event class extending OrderCreated for the given custom order type id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The custom order type id.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$className</td>
        <td>The class name of the event class.</td>
    </tr>
</table>


<pre>public static <strong>removeEventForType</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/string">string</a> $className):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Removes an event class for the given custom order type id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The custom order type id.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$className</td>
        <td>The class name of the event class.</td>
    </tr>
</table>


# Code<a name="order_code"></a>
    
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
            <td><a href="order#order_models_couponcampaign">CouponCampaign</a>
</td>
            <td>campaign</td>
            <td>The coupon campaign and all information about the campaign that this code belongs to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
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
            <td>The external ID of a coupon campaign</td>
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


<pre>public <strong>findByContact</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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


<pre>public <strong>findByCampaign</strong>(<a target="_blank" href="http://php.net/int">int</a> $campaignId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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


<pre>public <strong>findByCoupon</strong>(<a target="_blank" href="http://php.net/string">string</a> $coupon, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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
            <td><a target="_blank" href="http://php.net/double">double</a></td>
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
        <td>The CouponCodeValidation data to validate</td>
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
            <td>The remaining coupon amount
int                                    $orderUid				The order ID from affiliprint
string                                 $campaignUid				The id of the affiliprint coupon campaign</td>
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
            <td>The quantity of the item</td>
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
            <td>The field of the vat rate</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
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


<pre>public <strong>getCurrencyList</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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


<pre>public <strong>getCurrencyCountries</strong>(<a target="_blank" href="http://php.net/string">string</a> $currencyIso, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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
### Currency<a name="order_models_currency"></a>

The currency model. The model includes information like ISO 4217 code and the related symbols as well as the countries that a currency is used in.


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
            <td>The id of the currency name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the name</td>
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
    
# Date<a name="order_date"></a>
    
## Contracts<a name="order_date_contracts"></a>
### OrderDateRepositoryContract<a name="order_contracts_orderdaterepositorycontract"></a>

The OrderDateRepositoryContract contains the functionality to find available OrderDateTypes with their names in a specific language. Furthermore it is possible to create new OrderDateTypes, to update or delete existing date types and to create date type names for a language.


#### Namespace

`Plenty\Modules\Order\Date\Contracts`



#### Methods

<pre>public <strong>findNamesByTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get date type names
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The id of the date type</td>
    </tr>
</table>


<pre>public <strong>findNameByTypeIdAndLang</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="order#order_models_orderdatetypename">OrderDateTypeName</a>
</pre>

    
Get a date type name
    
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

    
Get the date types
    
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

    
Create or update order date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The order date data. The properties that are required to create an order can be found in the OrderDate model.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderDateId):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>

    
Delete a date
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderDateId</td>
        <td>The ID of the order date</td>
    </tr>
</table>


<pre>public <strong>findByOrderIdAndTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a href="order#order_models_orderdate">OrderDate</a>
</pre>

    
Get an order date
    
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


<pre>public <strong>findByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List order dates
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


## Models<a name="order_date_models"></a>
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
</ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>date</td>
            <td>The actual complete date plus hours, minutes and seconds for the date. The date format must comply with the W3C standard.</td>
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
            <td><a href="order#order_models_order">Order</a>
</td>
            <td>order</td>
            <td>The order that the date belongs to</td>
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
<li>Completed date = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
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
            <td>A collection of names for this OrderDateType</td>
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
<li>Completed date = 5</li>
<li>Return date = 6</li>
<li>Payment due date = 7</li>
<li>Estimated shipping date = 8</li>
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
    
# Events<a name="order_events"></a>
    
## Created<a name="order_events_created"></a>
### CreditNoteCreated<a name="order_created_creditnotecreated"></a>

An event class fired after a new credit note is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### DeliveryOrderCreated<a name="order_created_deliveryordercreated"></a>

An event class fired after a new delivery order is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### MultiCreditNoteCreated<a name="order_created_multicreditnotecreated"></a>

An event class fired after a new multi credit note is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### MultiOrderCreated<a name="order_created_multiordercreated"></a>

An event class fired after a new multi order is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RepairCreated<a name="order_created_repaircreated"></a>

An event class fired after a new repair is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ReturnCreated<a name="order_created_returncreated"></a>

An event class fired after a new returns is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SalesOrderCreated<a name="order_created_salesordercreated"></a>

An event class fired after a new sales order is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WarrantyCreated<a name="order_created_warrantycreated"></a>

An event class fired after a new warranty is created.


#### Namespace

`Plenty\Modules\Order\Events\Created`



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
            <td>The order id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderType</td>
            <td>The order type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The contact id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The referrer.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>status</td>
            <td>The status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The order owner.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>entryDate</td>
            <td>The entry date.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>webstoreId</td>
            <td>The webstore id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The warehouse id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sellerAccount</td>
            <td>The seller account.</td>
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
    
# Referrer<a name="order_referrer"></a>
    
## Contracts<a name="order_referrer_contracts"></a>
### OrderReferrerRepositoryContract<a name="order_contracts_orderreferrerrepositorycontract"></a>

Provides methods for processing order referrers. An order referrer indicates where a purchase was made originally. 


#### Namespace

`Plenty\Modules\Order\Referrer\Contracts`



#### Methods

<pre>public <strong>getList</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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
    
# Shipping<a name="order_shipping"></a>
    
## Contracts<a name="order_shipping_contracts"></a>
### ParcelServicePresetRepositoryContract<a name="order_contracts_parcelservicepresetrepositorycontract"></a>

The ParcelServicePresetRepositoryContract is the interface for the shipping profile repository. This interface allows to get a shipping profile by the id or list all shipping profiles.


#### Namespace

`Plenty\Modules\Order\Shipping\Contracts`



#### Methods

<pre>public <strong>getPresetList</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all available parcel service presets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns (attributes) to load in the instances.</td>
    </tr>
</table>


<pre>public <strong>getPresetById</strong>(<a target="_blank" href="http://php.net/int">int</a> $presetId, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="order#order_models_parcelservicepreset">ParcelServicePreset</a>
</pre>

    
Get specific parcel service preset determined by preset id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$presetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns (attributes) to load in the instances.</td>
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


<pre>public <strong>getCountriesList</strong>(<a target="_blank" href="http://php.net/int">int</a> $active, <a target="_blank" href="http://php.net/array">array</a> $with):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
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


<pre>public <strong>getActiveCountryNameMap</strong>(<a target="_blank" href="http://php.net/string">string</a> $language):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
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
    
# ParcelService<a name="order_parcelservice"></a>
    
## Models<a name="order_parcelservice_models"></a>
### ParcelService<a name="order_models_parcelservice"></a>

The Parcel Service Model


#### Namespace

`Plenty\Modules\Order\Shipping\ParcelService\Models`



#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

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
        </tr></tbody>
</table>


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
    
# Status<a name="order_status"></a>
    
## Contracts<a name="order_status_contracts"></a>
### StatusRepositoryContract<a name="order_contracts_statusrepositorycontract"></a>

The StatusRepositoryContract is the interface for the status repository. This interface allows you to find, create and update status.


#### Namespace

`Plenty\Modules\Order\Status\Contracts`



#### Methods

<pre>public <strong>findStatusById</strong>(<a target="_blank" href="http://php.net/float">float</a> $statusId, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="order#order_models_orderstatus">OrderStatus</a>
</pre>

    
Get a status
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$statusId</td>
        <td>The ID of the status</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the status instance. Currently the only relation available is "names".</td>
    </tr>
</table>


<pre>public <strong>findStatusNameById</strong>(<a target="_blank" href="http://php.net/float">float</a> $statusId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="order#order_models_orderstatusname">OrderStatusName</a>
</pre>

    
Get a name of a status in one language
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$statusId</td>
        <td>The id of the status to be found.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The lang of the status to be found.</td>
    </tr>
</table>


<pre>public <strong>searchStatus</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List statuses
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of statuses to be displayed per page. The default number of statuses per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Status instance. Currently the only relation available is "names".</td>
    </tr>
</table>


## Models<a name="order_status_models"></a>
### OrderStatus<a name="order_models_orderstatus"></a>

The order status model contains the ID of an order status. The ID is always an integer with two decimal places. The highest number available is 99. Every status has names in different languages, which are accessible through the names attribute.


#### Namespace

`Plenty\Modules\Order\Status\Models`


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
            <td>The status ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if the status can be deleted or not.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The names of the order statuses</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### OrderStatusName<a name="order_models_orderstatusname"></a>

The order status name model represents a status name for a given status ID. However, a status can not only have one name, but two names per language: a frontend name and a backend name.


#### Namespace

`Plenty\Modules\Order\Status\Models`


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
            <td>The ID of the status name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>statusId</td>
            <td>The ID of the status that the name belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The backend name of the status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>frontendName</td>
            <td>The frontend name of the status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the status name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisibleInFrontend</td>
            <td>Flag that indicates if this status should be visible in the frontend or not. True = the status is visible in the frontend. False = the status is not visible in the frontend.</td>
        </tr><tr>
            <td><a href="order#order_models_orderstatus">OrderStatus</a>
</td>
            <td>status</td>
            <td>The order status that this name belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
