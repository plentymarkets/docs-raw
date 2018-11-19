

# Basket<a name="basket_basket"></a>
    
## Contracts<a name="basket_basket_contracts"></a>
### BasketItemRepositoryContract<a name="basket_contracts_basketitemrepositorycontract"></a>

The BasketItemRepositoryContract is the interface for the basket item repository. This interface allows to list, add, update and delete items from the shopping cart of the current customer session.


#### Namespace

`Plenty\Modules\Basket\Contracts`





#### Methods

<pre>public <strong>findOneById</strong>(<a target="_blank" href="http://php.net/int">int</a> $basketRowId):<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    
Gets an existing item by ID in the shopping cart of the current customer session.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$basketRowId</td>
        <td>The ID of the basket row</td>
    </tr>
</table>


<pre>public <strong>findExistingOneByData</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    
Gets an existing item by item data in the shopping cart of the current customer session.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The item's data</td>
    </tr>
</table>


<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all items in the shopping cart of the current customer session.
    
<pre>public <strong>addBasketItem</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    
Creates an item with the specified item data in the shopping cart.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The item's data</td>
    </tr>
</table>


<pre>public <strong>updateBasketItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $basketItemId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates an existing item in the shopping cart. The ID of the item and the data to be updated must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$basketItemId</td>
        <td>The ID of the item in the shopping cart</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The item's data</td>
    </tr>
</table>


<pre>public <strong>removeBasketItem</strong>(<a target="_blank" href="http://php.net/int">int</a> $basketItemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes an item from the shopping cart. The ID of the item must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$basketItemId</td>
        <td>The ID of the item in the shopping cart</td>
    </tr>
</table>



### BasketRepositoryContract<a name="basket_contracts_basketrepositorycontract"></a>

The BasketRepositoryContract is the interface for the basket repository. This interface allows to get the shopping cart of the current customer session.


#### Namespace

`Plenty\Modules\Basket\Contracts`





#### Methods

<pre>public <strong>load</strong>():<a href="basket#basket_models_basket">Basket</a>
</pre>

    
Gets the shopping cart from current customer session.
    
<pre>public <strong>save</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setCouponCode</strong>(<a target="_blank" href="http://php.net/string">string</a> $couponCode):<a href="basket#basket_models_basket">Basket</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$couponCode</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>removeCouponCode</strong>():<a href="basket#basket_models_basket">Basket</a>
</pre>

    

    
## Models<a name="basket_basket_models"></a>
### BasketItem<a name="basket_models_basketitem"></a>

The basket item model


#### Namespace

`Plenty\Modules\Basket\Models`




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
            <td>The ID of the item in the shopping cart</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>basketId</td>
            <td>The ID of the shopping cart. The ID increases by 1 when a new customer enters the online store and adds an item to the shopping cart.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sessionId</td>
            <td>The ID of the current customer session</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderRowId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>quantity</td>
            <td>The current quantity of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>quantityOriginally</td>
            <td>The initial quantity of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceId</td>
            <td>The ID of the item price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueSetId</td>
            <td>The ID of the attribute value set</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rebate</td>
            <td>The discount on the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vat</td>
            <td>The VAT</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td>The item price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>givenPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>useGivenPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>inputWidth</td>
            <td>The width of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>inputLength</td>
            <td>The length of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>inputHeight</td>
            <td>The height of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemType</td>
            <td>The item type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalItemId</td>
            <td>The external variation ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>noEditByCustomer</td>
            <td>Shows whether the item was edited by the customer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>costCenterId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>giftPackageForRowId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The item position</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>size</td>
            <td>The item size</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingProfileId</td>
            <td>The ID of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The ID of the order referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deliveryDate</td>
            <td>The delivery date</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryId</td>
            <td>The ID of the item category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reservationDatetime</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The ID of the item variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>bundleVariationId</td>
            <td>The ID of the item bundle type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The date that the shopping cart was created</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The date that the shopping cart was updated last</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>attributeTotalMarkup</td>
            <td>attribute total markup</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>basketItemOrderParams</td>
            <td>Array of BasketItemParams</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### BasketItemParams<a name="basket_models_basketitemparams"></a>

The basket item params model


#### Namespace

`Plenty\Modules\Basket\Models`




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
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>basketItemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Basket<a name="basket_models_basket"></a>

The basket model


#### Namespace

`Plenty\Modules\Basket\Models`




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
            <td>The ID of the shopping cart. The ID increases by 1 when a new customer enters the online store and adds an item to the shopping cart.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sessionId</td>
            <td>The ID of the current customer session</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerId</td>
            <td>The ID of the customer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerInvoiceAddressId</td>
            <td>The ID of the customer's invoice address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerShippingAddressId</td>
            <td>The ID of the customer's shipping address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The ID of the order referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingCountryId</td>
            <td>The ID of the shipping country</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>methodOfPaymentId</td>
            <td>The ID of the payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingProviderId</td>
            <td>The ID of the shipping provider</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingProfileId</td>
            <td>The ID of the shipping profile</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>itemSum</td>
            <td>The gross value of items in the shopping cart</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>itemSumNet</td>
            <td>The net value of items in the shopping cart</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basketAmount</td>
            <td>The total gross value of the shopping cart</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basketAmountNet</td>
            <td>The total net value of the shopping cart</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>shippingAmount</td>
            <td>The gross shipping costs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>shippingAmountNet</td>
            <td>The net shipping costs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>paymentAmount</td>
            <td>The amount of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>couponCode</td>
            <td>The entered coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>couponDiscount</td>
            <td>The received discount due to the coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>shippingDeleteByCoupon</td>
            <td>Shows whether the shipping costs are subtracted due to a coupon code. Shopping carts that are free of shipping costs have the value true.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basketRebate</td>
            <td>The discount to the shopping cart value. The discount can either be set as a discount scale for items, as a customer class discount or as a discount based on the payment method.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>basketRebateType</td>
            <td>The discount type. The following types are available:
<ul>
    <li>Discount scale based on net value of items = 4</li>
    <li>    Discount based on method of payment = 5</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxFsk</td>
            <td>The age rating</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderTimestamp</td>
            <td>The timestamp of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The date that the shopping cart was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The date that the shopping cart was updated last.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>basketItems</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Exceptions<a name="basket_basket_exceptions"></a>
### BasketCheckException<a name="basket_exceptions_basketcheckexception"></a>

Class BasketCheckException


#### Namespace

`Plenty\Modules\Basket\Exceptions`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $code, <a target="_blank" href="http://php.net/string">string</a> $message = &quot;&quot;, <a href="miscellaneous#miscellaneous__exception">Exception</a>
 $previous = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
BasketItemCheckException constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__exception">Exception</a>
</td>
        <td>$previous</td>
        <td></td>
    </tr>
</table>



### BasketItemQuantityCheckException<a name="basket_exceptions_basketitemquantitycheckexception"></a>

Created by ptopczewski, 17.05.16 09:37
Class BasketItemQuantityCheckException


#### Namespace

`Plenty\Modules\Basket\Exceptions`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/int">int</a> $code, <a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/float">float</a> $requestedQuantity, <a target="_blank" href="http://php.net/string">string</a> $message = &quot;&quot;, <a href="miscellaneous#miscellaneous__exception">Exception</a>
 $previous = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
BasketItemQuantityCheckException constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$requestedQuantity</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__exception">Exception</a>
</td>
        <td>$previous</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getVariationId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getRequestedQuantity</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>

    

    

### BasketItemCheckException<a name="basket_exceptions_basketitemcheckexception"></a>

Created by ptopczewski, 12.05.16 09:03
Class BasketItemCheckException


#### Namespace

`Plenty\Modules\Basket\Exceptions`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/int">int</a> $code = 404, <a target="_blank" href="http://php.net/string">string</a> $message = &quot;&quot;, <a href="miscellaneous#miscellaneous__exception">Exception</a>
 $previous = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
BasketItemCheckException constructor.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$code</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$message</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__exception">Exception</a>
</td>
        <td>$previous</td>
        <td></td>
    </tr>
</table>


# Events<a name="basket_events"></a>
    
## Basket<a name="basket_events_basket"></a>
### AfterBasketCreate<a name="basket_basket_afterbasketcreate"></a>

The event is triggered after the shopping cart is created.


#### Namespace

`Plenty\Modules\Basket\Events\Basket`





#### Methods

<pre>public <strong>getBasket</strong>():<a href="basket#basket_models_basket">Basket</a>
</pre>

    

    

### AfterBasketChanged<a name="basket_basket_afterbasketchanged"></a>

The event is triggered after the shopping cart is changed.


#### Namespace

`Plenty\Modules\Basket\Events\Basket`





#### Methods

<pre>public <strong>hasValidCoupon</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setHasValidCoupon</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $hasValidCoupon):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$hasValidCoupon</td>
        <td>Flag that indicates if a valid coupon has been used.</td>
    </tr>
</table>


<pre>public <strong>getBasket</strong>():<a href="basket#basket_models_basket">Basket</a>
</pre>

    

    
<pre>public <strong>getLocationId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $locationId):<a href="basket#basket_events_basket">Basket</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$locationId</td>
        <td>The ID of the location</td>
    </tr>
</table>


<pre>public <strong>getInvoiceAddress</strong>():<a href="account#account_models_address">Address</a>
</pre>

    

    
<pre>public <strong>setInvoiceAddress</strong>(<a href="account#account_models_address">Address</a>
 $invoiceAddress):<a href="basket#basket_events_basket">Basket</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="account#account_models_address">Address</a>
</td>
        <td>$invoiceAddress</td>
        <td>The invoice address</td>
    </tr>
</table>


<pre>public <strong>getMaxFsk</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>setMaxFsk</strong>(<a target="_blank" href="http://php.net/int">int</a> $maxFsk):<a href="basket#basket_events_basket">Basket</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$maxFsk</td>
        <td>The highest value for age restriction of an item in the shopping cart</td>
    </tr>
</table>


<pre>public <strong>getShippingCosts</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>

    

    
<pre>public <strong>setShippingCosts</strong>(<a target="_blank" href="http://php.net/float">float</a> $shippingCosts):<a href="basket#basket_events_basket">Basket</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$shippingCosts</td>
        <td>The shipping costs of the shopping cart</td>
    </tr>
</table>


## BasketItem<a name="basket_events_basketitem"></a>
### BeforeBasketItemAdd<a name="basket_basketitem_beforebasketitemadd"></a>

The event is triggered before an item is created in the shopping cart.


#### Namespace

`Plenty\Modules\Basket\Events\BasketItem`





#### Methods

<pre>public <strong>getBasketItem</strong>():<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    

    

### AfterBasketItemRemove<a name="basket_basketitem_afterbasketitemremove"></a>

The event is triggered after an item is deleted from the shopping cart.


#### Namespace

`Plenty\Modules\Basket\Events\BasketItem`





### BeforeBasketItemUpdate<a name="basket_basketitem_beforebasketitemupdate"></a>

The event is triggered before an item in the shopping cart is updated.


#### Namespace

`Plenty\Modules\Basket\Events\BasketItem`





#### Methods

<pre>public <strong>getBasketItem</strong>():<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    

    

### AfterBasketItemUpdate<a name="basket_basketitem_afterbasketitemupdate"></a>

The event is triggered after an item in the shopping cart is updated.


#### Namespace

`Plenty\Modules\Basket\Events\BasketItem`





#### Methods

<pre>public <strong>getBasketItem</strong>():<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    

    

### AfterBasketItemAdd<a name="basket_basketitem_afterbasketitemadd"></a>

The event is triggered after an item is added to the shopping cart.


#### Namespace

`Plenty\Modules\Basket\Events\BasketItem`





#### Methods

<pre>public <strong>getBasketItem</strong>():<a href="basket#basket_models_basketitem">BasketItem</a>
</pre>

    

    

### BeforeBasketItemRemove<a name="basket_basketitem_beforebasketitemremove"></a>

The event is triggered before an item is deleted from the shopping cart.


#### Namespace

`Plenty\Modules\Basket\Events\BasketItem`




