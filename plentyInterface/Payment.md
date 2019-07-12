

# Payment<a name="payment_payment"></a>
    
## Contracts<a name="payment_payment_contracts"></a>
### PaymentMatcherRepositoryContract<a name="payment_contracts_paymentmatcherrepositorycontract"></a>

The PaymentMatcherRepositoryContract


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>checkMapFindAssignPayment</strong>(<a target="_blank" href="http://php.net/int">int</a> $mopId, $data):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mopId</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### PaymentPropertyTypeRepositoryContract<a name="payment_contracts_paymentpropertytyperepositorycontract"></a>

The PaymentPropertyTypeRepositoryContract is the interface for the payment property type repository. List, get, create and update payment properties.


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>allTypes</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payment property types. The language of the property type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the payment property type</td>
    </tr>
</table>


<pre>public <strong>findTypesById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets a payment property type. The ID of the property type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the payment property type. The following property types are available:
<ul>
    <li>Transaction ID = 1</li>
    <li>Reference ID = 2</li>
    <li>Booking text = 3</li>
    <li>Transaction password = 4</li>
    <li>Transaction code = 5</li>
    <li>Authorisation ID = 6</li>
    <li>Capture ID = 7</li>
    <li>Refund ID = 8</li>
    <li>Credit note ID = 9</li>
    <li>Order reference = 10</li>
    <li>Name of the sender = 11</li>
    <li>Email of the sender = 12</li>
    <li>The sender's sort code = 13</li>
    <li>The sender's bank name = 14</li>
    <li>The sender's bank account number = 15</li>
    <li>The holder of the bank account = 16</li>
    <li>The country of the sender's bank account = 17</li>
    <li>The sender's IBAN = 18</li>
    <li>The sender's BIC = 19</li>
    <li>Name of the recipient = 20</li>
    <li>The recipient's bank account = 21</li>
    <li>Reference text of the payment = 22</li>
    <li>Payment origin = 23</li>
    <li>Shipping address ID = 24</li>
    <li>Invoice address ID = 25</li>
    <li>Item buyer = 26</li>
    <li>Item number = 27</li>
    <li>Item transaction ID = 28</li>
    <li>External transaction type = 29</li>
    <li>External transaction status = 30</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the payment property type</td>
    </tr>
</table>


<pre>public <strong>createType</strong>($data):<a href="payment#payment_models_paymentpropertytype">PaymentPropertyType</a>
</pre>

    
Creates a payment property type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>changeProperty</strong>($data):<a href="payment#payment_models_paymentpropertytype">PaymentPropertyType</a>
</pre>

    
Updates a payment property type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### PaymentOrderRelationRepositoryContract<a name="payment_contracts_paymentorderrelationrepositorycontract"></a>

The PaymentOrderRelationRepositoryContract is the interface for the payment order relation repository. Create and delete relations between payments and orders.


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>createOrderRelation</strong>(<a href="payment#payment_models_payment">Payment</a>
 $payment, <a href="order#order_models_order">Order</a>
 $order):<a href="payment#payment_models_paymentorderrelation">PaymentOrderRelation</a>
</pre>

    
Creates a payment order relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_payment">Payment</a>
</td>
        <td>$payment</td>
        <td>The ID of the payment</td>
    </tr>
    <tr>
        <td><a href="order#order_models_order">Order</a>
</td>
        <td>$order</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>findOrderRelation</strong>(<a href="payment#payment_models_payment">Payment</a>
 $payment):<a href="payment#payment_models_paymentorderrelation">PaymentOrderRelation</a>
</pre>

    
Gets the payment order relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_payment">Payment</a>
</td>
        <td>$payment</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteOrderRelation</strong>(<a href="payment#payment_models_payment">Payment</a>
 $payment):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a payment order relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_payment">Payment</a>
</td>
        <td>$payment</td>
        <td>The ID of the payment</td>
    </tr>
</table>



### PaymentContactRelationRepositoryContract<a name="payment_contracts_paymentcontactrelationrepositorycontract"></a>

The PaymentContactRelationRepositoryContract is the interface for the payment contact relation repository. Create and delete relations between payments and contact.


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>createContactRelation</strong>(<a href="payment#payment_models_payment">Payment</a>
 $payment, <a href="account#account_models_contact">Contact</a>
 $contact):<a href="payment#payment_models_paymentcontactrelation">PaymentContactRelation</a>
</pre>

    
Creates a payment contact relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_payment">Payment</a>
</td>
        <td>$payment</td>
        <td>The ID of the payment</td>
    </tr>
    <tr>
        <td><a href="account#account_models_contact">Contact</a>
</td>
        <td>$contact</td>
        <td>The ID of the contact</td>
    </tr>
</table>


<pre>public <strong>deleteContactRelation</strong>(<a href="payment#payment_models_payment">Payment</a>
 $payment):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a payment contact relation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_payment">Payment</a>
</td>
        <td>$payment</td>
        <td>The ID of the payment</td>
    </tr>
</table>



### PaymentRepositoryContract<a name="payment_contracts_paymentrepositorycontract"></a>

The PaymentRepositoryContract is the interface for the payment repository. List, get, create and update payments. Payments can come into plentymarkets automatically or can be booked manually. Existing payments can be filtered by payment method, by ID, by payment status, by transaction type, by order or by date. Existing payments can also be updated.


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>getAll</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>getPaymentById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentId):<a href="payment#payment_models_payment">Payment</a>
</pre>

    
Gets a payment. The ID of the payment must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentId</td>
        <td>The ID of the payment</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByMethodId</strong>(<a target="_blank" href="http://php.net/int">int</a> $methodId, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments of a payment method. The ID of the payment method must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$methodId</td>
        <td>The ID of the payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByStatusId</strong>(<a target="_blank" href="http://php.net/int">int</a> $statusId, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments of a payment status. The ID of the payment status must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$statusId</td>
        <td>The ID of the payment status</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByTransactionType</strong>(<a target="_blank" href="http://php.net/int">int</a> $transactionType, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments of a transaction type. The transaction type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$transactionType</td>
        <td>The transaction type of the payment</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments of an order. The ID of the order must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByImportDateInterval</strong>(<a target="_blank" href="http://php.net/string">string</a> $startDate, <a target="_blank" href="http://php.net/string">string</a> $endDate, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments by import date. The start and the end of the date range must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startDate</td>
        <td>The start date of the date range for the import date of the payment</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$endDate</td>
        <td>The end date of the date range for the import date of the payment</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByEntryDateInterval</strong>(<a target="_blank" href="http://php.net/string">string</a> $startDate, <a target="_blank" href="http://php.net/string">string</a> $endDate, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments by entry date. The start and the end of the date range must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startDate</td>
        <td>The start date of the date range for the entry date of the payment</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$endDate</td>
        <td>The end date of the date range for the entry date of the payment</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>getPaymentsByPropertyTypeAndValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyTypeId, $propertyValue, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payments by payment property type and value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyTypeId</td>
        <td>The property type</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$propertyValue</td>
        <td>The property value</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of items to list per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page of results to search for</td>
    </tr>
</table>


<pre>public <strong>createPayment</strong>($data):<a href="payment#payment_models_payment">Payment</a>
</pre>

    
Creates a payment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updatePayment</strong>($data):<a href="payment#payment_models_payment">Payment</a>
</pre>

    
Updates a payment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getStatusConstants</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getOriginConstants</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### PaymentPropertyRepositoryContract<a name="payment_contracts_paymentpropertyrepositorycontract"></a>

The PaymentPropertyRepositoryContract is the interface for the payment property repository. List, get, create and update payment properties.


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists properties.
    
<pre>public <strong>findByPropertyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets a property. The ID of the payment property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td>The ID of the payment property</td>
    </tr>
</table>


<pre>public <strong>allByPaymentId</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists properties of a payment. The ID of the payment must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentId</td>
        <td>The ID of the payment</td>
    </tr>
</table>


<pre>public <strong>allByTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists properties of a property type. The ID of the property type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the payment property type. The following property types are available:
<ul>
    <li>Transaction ID = 1</li>
    <li>Reference ID = 2</li>
    <li>Booking text = 3</li>
    <li>Transaction password = 4</li>
    <li>Transaction code = 5</li>
    <li>Authorisation ID = 6</li>
    <li>Capture ID = 7</li>
    <li>Refund ID = 8</li>
    <li>Credit note ID = 9</li>
    <li>Order reference = 10</li>
    <li>Name of the sender = 11</li>
    <li>Email of the sender = 12</li>
    <li>The sender's sort code = 13</li>
    <li>The sender's bank name = 14</li>
    <li>The sender's bank account number = 15</li>
    <li>The holder of the bank account = 16</li>
    <li>The country of the sender's bank account = 17</li>
    <li>The sender's IBAN = 18</li>
    <li>The sender's BIC = 19</li>
    <li>Name of the recipient = 20</li>
    <li>The recipient's bank account = 21</li>
    <li>Reference text of the payment = 22</li>
    <li>Payment origin = 23</li>
    <li>Shipping address ID = 24</li>
    <li>Invoice address ID = 25</li>
    <li>Item buyer = 26</li>
    <li>Item number = 27</li>
    <li>Item transaction ID = 28</li>
    <li>External transaction type = 29</li>
    <li>External transaction status = 30</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>findByCreatedDateInterval</strong>(<a target="_blank" href="http://php.net/string">string</a> $startDate, <a target="_blank" href="http://php.net/string">string</a> $endDate):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists properties by creation date. The start and the end of the date range must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startDate</td>
        <td>The start date of the date range for the date of creation of the property</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$endDate</td>
        <td>The end date of the date range for the date of creation of the property</td>
    </tr>
</table>


<pre>public <strong>createProperty</strong>($data):<a href="payment#payment_models_paymentproperty">PaymentProperty</a>
</pre>

    
Creates a payment property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>changeProperty</strong>(<a href="payment#payment_models_paymentproperty">PaymentProperty</a>
 $data):<a href="payment#payment_models_paymentproperty">PaymentProperty</a>
</pre>

    
Updates a payment property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentproperty">PaymentProperty</a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### PaymentPropertyTypeNameRepositoryContract<a name="payment_contracts_paymentpropertytypenamerepositorycontract"></a>

The PaymentPropertyTypeNameRepositoryContract is the interface for the repository of payment property type names. List, get, create and update payment property names.


#### Namespace

`Plenty\Modules\Payment\Contracts`





#### Methods

<pre>public <strong>allTypeNames</strong>(<a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payment property type names. The language of the property type names must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the payment property type name</td>
    </tr>
</table>


<pre>public <strong>findByNameId</strong>(<a target="_blank" href="http://php.net/int">int</a> $nameId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Finds a payment property type name. The ID of the payment property type name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$nameId</td>
        <td>The ID of the payment property type name</td>
    </tr>
</table>


<pre>public <strong>createTypeName</strong>($data):<a href="payment#payment_models_paymentpropertytypename">PaymentPropertyTypeName</a>
</pre>

    
Creates a payment property type name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>changeProperty</strong>($data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Updates a payment property type name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Models<a name="payment_payment_models"></a>
### Payment<a name="payment_models_payment"></a>

The payment model


#### Namespace

`Plenty\Modules\Payment\Models`




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
            <td>The ID of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>amount</td>
            <td>The amount of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRatio</td>
            <td>The exchange rate. Exchange rates are used if the default currency saved in plentymarkets differs from the currency of the order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentId</td>
            <td>The ID of the parent payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deleted</td>
            <td>A deleted payment. Deleted payments have the value 1 and are not displayed in the plentymarkets back end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unaccountable</td>
            <td>An unassigned payment. Unassigned payments have the value 1.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency of the payment in ISO 4217 code.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The payment type. Available types are credit and debit.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>hash</td>
            <td>The hash code of the payment. The hash code consists of 32 characters and is automatically generated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>origin</td>
            <td>The origin of the payment. The following origins are available:
<ul>
    <li>Undefined = 0</li>
    <li>System = 1</li>
    <li>Manually = 2</li>
    <li>SOAP = 3</li>
    <li>Import = 4</li>
    <li>Split payment = 5</li>
    <li>Plugin = 6</li>
    <li>POS = 7</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>receivedAt</td>
            <td>The time the payment was received</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>importedAt</td>
            <td>The time the payment was imported</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>status</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses"  target="_blank">status</a> of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>transactionType</td>
            <td>The transaction type of the payment. The following transaction types are available:
<ul>
    <li>Interim transaction report = 1</li>
    <li>Booked payment = 2</li>
    <li>Split payment = 3</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mopId</td>
            <td>The ID of the payment method</td>
        </tr><tr>
            <td><a href="payment#payment_models_payment">Payment</a>
</td>
            <td>parent</td>
            <td>The parent payment</td>
        </tr><tr>
            <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
            <td>method</td>
            <td>The payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>histories</td>
            <td>The payment history</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>properties</td>
            <td>The properties of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>regenerateHash</td>
            <td>If $regenerateHash is true, regenerate the payment hash value. Default is false.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>updateOrderPaymentStatus</td>
            <td>If $updateOrderPaymentStatus is true, update the order payment status. Default is false.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSystemCurrency</td>
            <td>If $isSystemCurrency is false, the value will be converted to the standard currency with the provided exchange rate. If $isSystemCurrency is false, the value is not converted. Default is true.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentPropertyTypeName<a name="payment_models_paymentpropertytypename"></a>

The payment property type name model


#### Namespace

`Plenty\Modules\Payment\Models`




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
            <td>The ID of the name of the property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the name of the property type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentProperty<a name="payment_models_paymentproperty"></a>

The payment property model


#### Namespace

`Plenty\Modules\Payment\Models`




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
            <td>The ID of the payment property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentId</td>
            <td>The ID of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the property type. The following property types are available:
<ul>
    <li>Transaction ID = 1</li>
    <li>Reference ID = 2</li>
    <li>Booking text = 3</li>
    <li>Transaction password = 4</li>
    <li>Transaction code = 5</li>
    <li>Authorisation ID = 6</li>
    <li>Capture ID = 7</li>
    <li>Refund ID = 8</li>
    <li>Credit note ID = 9</li>
    <li>Order reference = 10</li>
    <li>Name of the sender = 11</li>
    <li>Email of the sender = 12</li>
    <li>The sender's sort code = 13</li>
    <li>The sender's bank name = 14</li>
    <li>The sender's bank account number = 15</li>
    <li>The holder of the bank account = 16</li>
    <li>The country of the sender's bank account = 17</li>
    <li>The sender's IBAN = 18</li>
    <li>The sender's BIC = 19</li>
    <li>Name of the recipient = 20</li>
    <li>The recipient's bank account = 21</li>
    <li>Reference text of the payment = 22</li>
    <li>Payment origin = 23</li>
    <li>Shipping address ID = 24</li>
    <li>Invoice address ID = 25</li>
    <li>Item buyer = 26</li>
    <li>Item number = 27</li>
    <li>Item transaction ID = 28</li>
    <li>External transaction type = 29</li>
    <li>External transaction status = 30</li>
    <li>The receiver's IBAN = 31</li>
    <li>The receiver's BIC = 32</li>
    <li>Transaction fee = 33</li>
    <li>Transaction lifespan = 34</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentPropertyType<a name="payment_models_paymentpropertytype"></a>

The payment property type model


#### Namespace

`Plenty\Modules\Payment\Models`




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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>erasable</td>
            <td>Specifies whether the property type can be deleted. Property types that can be deleted have the value 1. Default property types cannot be deleted.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position number of the property type</td>
        </tr><tr>
            <td><a href="payment#payment_models_paymentpropertytypename">PaymentPropertyTypeName</a>
</td>
            <td>name</td>
            <td>The name of the property type</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentContactRelation<a name="payment_models_paymentcontactrelation"></a>

The payment contact relation model


#### Namespace

`Plenty\Modules\Payment\Models`




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
            <td>The ID of the payment order relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentId</td>
            <td>The ID of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>assignedAt</td>
            <td>The time the payment contact relation was assigned</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentOrderRelation<a name="payment_models_paymentorderrelation"></a>

The payment order relation model


#### Namespace

`Plenty\Modules\Payment\Models`




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
            <td>The ID of the payment order relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentId</td>
            <td>The ID of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>assignedAt</td>
            <td>The time the payment order relation was assigned</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# History<a name="payment_history"></a>
    
## Contracts<a name="payment_history_contracts"></a>
### PaymentHistoryRepositoryContract<a name="payment_contracts_paymenthistoryrepositorycontract"></a>

The PaymentHistoryRepositoryContract is the interface for the payment history repository. Get and create the payment history.


#### Namespace

`Plenty\Modules\Payment\History\Contracts`





#### Methods

<pre>public <strong>getByPaymentId</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentId, <a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Gets the payment history for a payment. The ID of the payment and the ID of the payment type must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentId</td>
        <td>The ID of the payment</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td>The ID of the history type. The following types are available:
<ul>
    <li>Created = 1</li>
    <li>Status updated = 2</li>
    <li>Assigned = 3</li>
    <li>Detached = 4</li>
    <li>Deleted = 5</li>
    <li>Updated = 6</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>createHistory</strong>($data):<a href="payment#payment_models_paymenthistory">PaymentHistory</a>
</pre>

    
Creates the payment history.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Models<a name="payment_history_models"></a>
### PaymentHistory<a name="payment_models_paymenthistory"></a>

The payment history model


#### Namespace

`Plenty\Modules\Payment\History\Models`




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
            <td>The ID of the payment history</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentId</td>
            <td>The ID of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the history type. The following types are available:
<ul>
    <li>Created = 1</li>
    <li>Status updated = 2</li>
    <li>Assigned = 3</li>
    <li>Detached = 4</li>
    <li>Deleted = 5</li>
    <li>Updated = 6</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The language of the payment history</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>user</td>
            <td>The user who initiated the action</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Events<a name="payment_events"></a>
    
## Checkout<a name="payment_events_checkout"></a>
### ExecutePayment<a name="payment_checkout_executepayment"></a>

The event is triggered when a payment is executed.


#### Namespace

`Plenty\Modules\Payment\Events\Checkout`





#### Methods

<pre>public <strong>setOrderId</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the ID of the order in the checkout. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>


<pre>public <strong>getOrderId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the order.
    
<pre>public <strong>setMop</strong>(<a target="_blank" href="http://php.net/int">int</a> $mop):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the ID of the payment method. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mop</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


<pre>public <strong>getMop</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the payment method.
    
<pre>public <strong>setType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the content type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The <a href="https://developers.plentymarkets.com/dev-doc/payment-plugins#payment-prepare-payment">content type</a> of the payment plugin</td>
    </tr>
</table>


<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the content type.
    
<pre>public <strong>setValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $value):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the value of the content type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td>The value of the content type</td>
    </tr>
</table>


<pre>public <strong>getValue</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the value of the content type.
    

### GetPaymentMethodContent<a name="payment_checkout_getpaymentmethodcontent"></a>

The event is triggered after the payment method is selected in the checkout.


#### Namespace

`Plenty\Modules\Payment\Events\Checkout`





#### Methods

<pre>public <strong>setMop</strong>(<a target="_blank" href="http://php.net/int">int</a> $mop):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the ID of the payment method. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mop</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


<pre>public <strong>getMop</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the payment method.
    
<pre>public <strong>setType</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the content type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The <a href="https://developers.plentymarkets.com/dev-doc/payment-plugins#payment-prepare-payment">content type</a> of the payment plugin</td>
    </tr>
</table>


<pre>public <strong>getType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the content type.
    
<pre>public <strong>setValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $value):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the value of the content type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td>The value of the content type</td>
    </tr>
</table>


<pre>public <strong>getValue</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the value of the content type.
    
<pre>public <strong>setParams</strong>($params):<a href="payment#payment_events_checkout">Checkout</a>
</pre>

    
Updates the parameters. The parameters must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$params</td>
        <td>The parameters</td>
    </tr>
</table>


<pre>public <strong>getParams</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Gets the parameters.
    
# Method<a name="payment_method"></a>
    
## Contracts<a name="payment_method_contracts"></a>
### PaymentMethodRepositoryContract<a name="payment_contracts_paymentmethodrepositorycontract"></a>

The PaymentMethodRepositoryContract is the interface for the payment method repository. List, get, create and update payment methods.


#### Namespace

`Plenty\Modules\Payment\Method\Contracts`





#### Methods

<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payment methods.
    
<pre>public <strong>allForPlugin</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginKey):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists payment methods for a plugin key. The plugin key must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginKey</td>
        <td>The plugin key</td>
    </tr>
</table>


<pre>public <strong>allPluginPaymentMethods</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>allOldPaymentMethods</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>findByPaymentMethodId</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId):<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</pre>

    
Gets a payment method. The ID of the payment method must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


<pre>public <strong>getPreviewList</strong>(<a target="_blank" href="http://php.net/string">string</a> $language = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get an array with all payment methods with the ID as key and the name as value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td>The names will be returned in this language.</td>
    </tr>
</table>


<pre>public <strong>createPaymentMethod</strong>($paymentMethodData):<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</pre>

    
Creates a payment method.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$paymentMethodData</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateName</strong>($paymentMethodData):<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</pre>

    
Updates the payment method name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$paymentMethodData</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>preparePaymentMethod</strong>(<a target="_blank" href="http://php.net/int">int</a> $mop):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Prepares a payment method. The ID of the payment method must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mop</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


<pre>public <strong>executePayment</strong>(<a target="_blank" href="http://php.net/int">int</a> $mop, <a target="_blank" href="http://php.net/int">int</a> $orderId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Executes a payment. The ID of the payment method and the ID of the order must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$mop</td>
        <td>The ID of the payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
</table>



### PaymentMethodContainer<a name="payment_contracts_paymentmethodcontainer"></a>

The payment method container


#### Namespace

`Plenty\Modules\Payment\Method\Contracts`





#### Methods

<pre>public <strong>register</strong>(<a target="_blank" href="http://php.net/string">string</a> $paymentKey, <a target="_blank" href="http://php.net/string">string</a> $paymentMethodServiceClass, <a target="_blank" href="http://php.net/array">array</a> $rebuildEventClassesList):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$paymentKey</td>
        <td>The unique key of a payment plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$paymentMethodServiceClass</td>
        <td>The class of the payment method. This class contains information of the payment plugin, such as the name and whether the payment method is active.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$rebuildEventClassesList</td>
        <td>A list of events. It is checked again for the list of events whether the payment method is active.</td>
    </tr>
</table>


<pre>public <strong>isRegistered</strong>(<a target="_blank" href="http://php.net/string">string</a> $paymentKey):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$paymentKey</td>
        <td></td>
    </tr>
</table>



### PaymentMethodService<a name="payment_contracts_paymentmethodservice"></a>

The payment method service


#### Namespace

`Plenty\Modules\Payment\Method\Contracts`




## Models<a name="payment_method_models"></a>
### PaymentMethod<a name="payment_models_paymentmethod"></a>

The payment method model


#### Namespace

`Plenty\Modules\Payment\Method\Models`




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
            <td>The ID of the payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pluginKey</td>
            <td>The plugin key of the payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paymentKey</td>
            <td>The payment key of the payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the payment method</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# MethodName<a name="payment_methodname"></a>
    
## Models<a name="payment_methodname_models"></a>
### PaymentMethodName<a name="payment_models_paymentmethodname"></a>

The payment method name model


#### Namespace

`Plenty\Modules\Payment\MethodName\Models`




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
            <td>paymentMethodId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
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
    
