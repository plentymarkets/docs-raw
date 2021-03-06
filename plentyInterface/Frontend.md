

# PaymentMethod<a name="frontend_paymentmethod"></a>
    
## Contracts<a name="frontend_paymentmethod_contracts"></a>
### FrontendPaymentMethodRepositoryContract<a name="frontend_contracts_frontendpaymentmethodrepositorycontract"></a>

The FrontendPaymentMethodRepositoryContract is the interface for the front end payment method repository. Get the payment method information to be displayed in the online store.


#### Namespace

`Plenty\Modules\Frontend\PaymentMethod\Contracts`





#### Methods

<pre>public <strong>getCurrentPaymentMethodsList</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all payment methods of the current customer session.
    
<pre>public <strong>getCurrentPaymentMethodsListForSwitch</strong>(<a target="_blank" href="http://php.net/int">int</a> $currentPaymentMethodId, <a target="_blank" href="http://php.net/int">int</a> $orderId = null, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all payment methods for switch.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$currentPaymentMethodId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCurrentPaymentMethodsForExpressCheckout</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all payment methods if express checkout is available
    
<pre>public <strong>getPaymentMethodName</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the name of the payment method in the specified language.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td>The payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodFee</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/float">float</a></pre>

    
Gets additional costs for the payment method. Additional costs can be entered in the config.json.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td>The payment method</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodIcon</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the icon of the payment method. The path of the icon can be entered in the config.json.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td>The payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodDescription</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the description of the payment method. The description can be entered in the config.json.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodSourceUrl</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the detail link of the payment method. The detail link can be entered in the config.json.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getIsSwitchableTo</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Gets the detail link of the payment method. The detail link can be entered in the config.json.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getIsSwitchableFrom</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Gets the detail link of the payment method. The detail link can be entered in the config.json.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodIsSelectable</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Get true if the payment method can be selected in the payment method list
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodNameById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the name of the payment method by ID and language. The ID of the payment method and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodFeeById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId):<a target="_blank" href="http://php.net/float">float</a></pre>

    
Gets additional costs for the payment method by ID. The ID of the payment method must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodIconById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the icon of the payment method by ID and language. The ID of the payment method and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodDescriptionById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the description of the payment method by ID and language. The ID of the payment method and the language must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodSwitchToById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/int">int</a> $orderId = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodSwitchFromById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/int">int</a> $orderId = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodSwitchableToById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/int">int</a> $orderId = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodSwitchableFromById</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId, <a target="_blank" href="http://php.net/int">int</a> $orderId = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAllowedPaymentMethodListForContact</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
# Frontend<a name="frontend_frontend"></a>
    
## Contracts<a name="frontend_frontend_contracts"></a>
### CurrencyExchangeRepositoryContract<a name="frontend_contracts_currencyexchangerepositorycontract"></a>

The CurrencyExchangeRatioRepositoryContract is the interface for the currency exchange repository. This interface allows you to get the default system currency, to get exchange ratios for every currency and to convert an amount from the default currency into a given currency or from a given currency into the default currency.


#### Namespace

`Plenty\Modules\Frontend\Contracts`





#### Methods

<pre>public <strong>getExchangeRatioByCurrency</strong>(<a target="_blank" href="http://php.net/string">string</a> $currency):<a target="_blank" href="http://php.net/float">float</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getDefaultCurrency</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the default currency.
    
<pre>public <strong>convertFromDefaultCurrency</strong>(<a target="_blank" href="http://php.net/string">string</a> $currency, <a target="_blank" href="http://php.net/float">float</a> $amount, <a target="_blank" href="http://php.net/float">float</a> $exchangeRatio = 0.0):<a target="_blank" href="http://php.net/float">float</a></pre>

    
Converts the given value from the default currency to the given currency.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$amount</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$exchangeRatio</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>convertToDefaultCurrency</strong>(<a target="_blank" href="http://php.net/string">string</a> $currency, <a target="_blank" href="http://php.net/float">float</a> $amount, <a target="_blank" href="http://php.net/float">float</a> $exchangeRatio = 0.0):<a target="_blank" href="http://php.net/float">float</a></pre>

    
Converts the given value to the default currency from the given currency.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$amount</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$exchangeRatio</td>
        <td></td>
    </tr>
</table>



### Checkout<a name="frontend_contracts_checkout"></a>

The CheckoutContract is the interface for the checkout repository. This interface allows to set the shipping country ID, the payment method ID, the shipping profile ID and the currency in the checkout.


#### Namespace

`Plenty\Modules\Frontend\Contracts`





#### Methods

<pre>public <strong>getShippingCountryId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the shipping country ID.
    
<pre>public <strong>setShippingCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingCountryId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the ID of the shipping country. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingCountryId</td>
        <td>The ID of the shipping country</td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the payment method id of the current shopping cart.
    
<pre>public <strong>setPaymentMethodId</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the ID of the payment method. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td>The ID of the payment method</td>
    </tr>
</table>


<pre>public <strong>getShippingProfileId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the shipping profile id of the current shopping cart.
    
<pre>public <strong>setShippingProfileId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingProfileId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the ID of the shipping profile. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingProfileId</td>
        <td>The ID of the shipping profile</td>
    </tr>
</table>


<pre>public <strong>setCurrency</strong>(<a target="_blank" href="http://php.net/string">string</a> $currency):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the currency. The currency must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td>The currency</td>
    </tr>
</table>


<pre>public <strong>setBasketReferrerId</strong>(<a target="_blank" href="http://php.net/int">int</a> $referrerId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the ID of the order referrer. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$referrerId</td>
        <td>The ID of the order referrer. The <a href="https://www.plentymarkets.co.uk/manual/settings/orders/order-referrer/" target="_blank">order referrer</a> settings can be changed in the plentymarkets back end.</td>
    </tr>
</table>


<pre>public <strong>getCustomerInvoiceAddressId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the invoice address id of the current shopping cart.
    
<pre>public <strong>setCustomerInvoiceAddressId</strong>(<a target="_blank" href="http://php.net/int">int</a> $invoiceAddressId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the invoice address id for the current shopping cart.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$invoiceAddressId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCustomerShippingAddressId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the shipping address id of the current shopping cart.
    
<pre>public <strong>setCustomerShippingAddressId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingAddressId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the shipping address id for the current shopping cart.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingAddressId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>validateCheckout</strong>():<a href="frontend#frontend_events_validatecheckoutevent">ValidateCheckoutEvent</a>
</pre>

    

    
## Models<a name="frontend_frontend_models"></a>
### TotalVat<a name="frontend_models_totalvat"></a>

frontend total vat model


#### Namespace

`Plenty\Modules\Frontend\Models`




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
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatAmount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatValue</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Factories<a name="frontend_frontend_factories"></a>
### FrontendFactory<a name="frontend_factories_frontendfactory"></a>

Frontend-Factory


#### Namespace

`Plenty\Modules\Frontend\Factories`





#### Methods

<pre>public <strong>getLocale</strong>():<a href="frontend#frontend_services_localeservice">LocaleService</a>
</pre>

    

    
<pre>public <strong>getAgent</strong>():<a href="frontend#frontend_services_agentservice">AgentService</a>
</pre>

    

    
<pre>public <strong>getSystem</strong>():<a href="frontend#frontend_services_systemservice">SystemService</a>
</pre>

    

    
<pre>public <strong>getAccount</strong>():<a href="frontend#frontend_services_accountservice">AccountService</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="frontend#frontend_services_fileservice">FileService</a>
</pre>

    

    
## Events<a name="frontend_frontend_events"></a>
### FrontendCurrencyChanged<a name="frontend_events_frontendcurrencychanged"></a>

The event is triggered when the currency is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getCurrency</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the currency.
    
<pre>public <strong>getCurrencyExchangeRatio</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>

    
Gets the exchange rate used for converting the currency.
    

### FrontendCustomerAddressChanged<a name="frontend_events_frontendcustomeraddresschanged"></a>

The event is triggered when a customer address is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





### FrontendUpdatePaymentSettings<a name="frontend_events_frontendupdatepaymentsettings"></a>

The event is triggered when the payment method is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getPaymentMethodId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the payment method.
    

### FrontendUpdateInvoiceAddress<a name="frontend_events_frontendupdateinvoiceaddress"></a>

The event is triggered when the invoice address is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getAccountAddressId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the address saved for the account.
    

### FrontendShippingProfileChanged<a name="frontend_events_frontendshippingprofilechanged"></a>

The event is triggered when the shipping profile is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getShippingProfileId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Gets the ID of the shipping profile.
    
<pre>public <strong>setShippingProfileId</strong>($shippingProfileId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the ID of the shipping profile. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$shippingProfileId</td>
        <td></td>
    </tr>
</table>



### FrontendUpdateDeliveryAddress<a name="frontend_events_frontendupdatedeliveryaddress"></a>

The event is triggered when the delivery address is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getAccountAddressId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the address saved for the account.
    

### FrontendLanguageChanged<a name="frontend_events_frontendlanguagechanged"></a>

The event is triggered when the language is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getLanguage</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Gets the language of the online store.
    

### FrontendShippingCountryChanged<a name="frontend_events_frontendshippingcountrychanged"></a>

The event is triggered when the shipping country is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getShippingCountryId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the shipping country.
    
<pre>public <strong>setShippingCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingCountryId):<a href="frontend#frontend_events_frontendshippingcountrychanged">FrontendShippingCountryChanged</a>
</pre>

    
Updates the ID of the shipping country. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingCountryId</td>
        <td>The ID of the shipping country</td>
    </tr>
</table>



### FrontendPaymentMethodChanged<a name="frontend_events_frontendpaymentmethodchanged"></a>

The event is triggered when the payment method is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getPaymentMethodId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Gets the ID of the payment method.
    
<pre>public <strong>setPaymentMethodId</strong>($paymentMethodId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the ID of the payment method. The ID must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
</table>



### ValidateCheckoutEvent<a name="frontend_events_validatecheckoutevent"></a>

validation event


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getErrorKeysList</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addErrorKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $errorKey):<a href="frontend#frontend_frontend_events">Events</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$errorKey</td>
        <td></td>
    </tr>
</table>



### FrontendUpdateShippingSettings<a name="frontend_events_frontendupdateshippingsettings"></a>

The event is triggered when the shipping method is updated in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getShippingCosts</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>

    
Gets the shipping costs.
    
<pre>public <strong>getParcelServiceId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the ID of the shipping service provider.
    
<pre>public <strong>getParcelServicePresetId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Gets the preset ID of the shipping service provider.
    

### FrontendReferrerChanged<a name="frontend_events_frontendreferrerchanged"></a>

The event is triggered when the referrer id  is changed in the online store.


#### Namespace

`Plenty\Modules\Frontend\Events`





#### Methods

<pre>public <strong>getReferrerId</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setReferrerId</strong>($referrerId):<a href="frontend#frontend_events_frontendreferrerchanged">FrontendReferrerChanged</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$referrerId</td>
        <td></td>
    </tr>
</table>


## Services<a name="frontend_frontend_services"></a>
### AgentService<a name="frontend_services_agentservice"></a>

Frontend-Service for agent information


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>getLanguages</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getBrowser</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getPlatform</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDevice</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getIsDesktop</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getRobotName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getIsRobot</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getHttpHeaders</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getIsMobile</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getIsTablet</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### AccountService<a name="frontend_services_accountservice"></a>

Frontend-service for customer information


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>getIsAccountLoggedIn</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getAccountContactId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    

### FileService<a name="frontend_services_fileservice"></a>

Frontend-service for file information


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>addJsFile</strong>(<a target="_blank" href="http://php.net/string">string</a> $jsFile):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$jsFile</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasGetMutator</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if a get mutator exists for an attribute.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setAttributes</strong>($attributes):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$attributes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setAttribute</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous_repositories_models">Models</a>
</pre>

    
Set a given attribute on the model.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasSetMutator</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if a set mutator exists for an attribute.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>changeValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/callable">callable</a> $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>offsetExists</strong>($offset):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$offset</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>offsetGet</strong>($offset):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$offset</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>offsetSet</strong>($offset, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$offset</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>offsetUnset</strong>($offset):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$offset</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $translate = false):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$translate</td>
        <td>Flag indicating if values should be translated.</td>
    </tr>
</table>


<pre>public <strong>toJson</strong>(<a target="_blank" href="http://php.net/int">int</a> $options):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$options</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>jsonSerialize</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>fill</strong>(<a target="_blank" href="http://php.net/array">array</a> $attributes):<a href="miscellaneous#miscellaneous_repositories_models">Models</a>
</pre>

    
Fill the model with an array of attributes.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributes</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isFillable</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine if the given attribute may be mass assigned.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFillable</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the fillable attributes for the model.
    
<pre>public <strong>fillable</strong>(<a target="_blank" href="http://php.net/array">array</a> $fillable):<a href="miscellaneous#miscellaneous_repositories_models">Models</a>
</pre>

    
Set the fillable attributes for the model.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fillable</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>hasCast</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $types = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determine whether an attribute should be cast to a native type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$types</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>fromJson</strong>(<a target="_blank" href="http://php.net/string">string</a> $value, <a target="_blank" href="http://php.net/bool">bool</a> $asObject = false):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Decode the given JSON back into an array or object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$asObject</td>
        <td></td>
    </tr>
</table>



### SystemService<a name="frontend_services_systemservice"></a>

Frontend-service for system information


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getWebstoreId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    

### OrderPropertyFileService<a name="frontend_services_orderpropertyfileservice"></a>

Frontend-service for customer information


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>uploadFile</strong>(<a target="_blank" href="http://php.net/array">array</a> $fileData):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$fileData</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFileURL</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFile</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a href="cloud#cloud_models_storageobject">StorageObject</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>copyBasketFileToOrder</strong>(<a target="_blank" href="http://php.net/string">string</a> $filename):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filename</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteFile</strong>(<a target="_blank" href="http://php.net/string">string</a> $filename):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filename</td>
        <td></td>
    </tr>
</table>



### LocaleService<a name="frontend_services_localeservice"></a>

frontend service for changing current language


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>setLanguage</strong>(<a target="_blank" href="http://php.net/string">string</a> $newLanguage, <a target="_blank" href="http://php.net/bool">bool</a> $fireEvents = true):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$newLanguage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$fireEvents</td>
        <td></td>
    </tr>
</table>



### VatService<a name="frontend_services_vatservice"></a>

Frontend-service for vat information


#### Namespace

`Plenty\Modules\Frontend\Services`





#### Methods

<pre>public <strong>getCountryVatId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>getCurrentTotalVats</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getVat</strong>(<a target="_blank" href="http://php.net/string">string</a> $taxIdNumber = &quot;&quot;):<a href="accounting#accounting_models_vat">Vat</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taxIdNumber</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getLocationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $countryId = null):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the ID of the location
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$countryId</td>
        <td></td>
    </tr>
</table>


# LegalInformation<a name="frontend_legalinformation"></a>
    
## Contracts<a name="frontend_legalinformation_contracts"></a>
### LegalInformationRepositoryContract<a name="frontend_contracts_legalinformationrepositorycontract"></a>

Repository contract for LegalInformation model.


#### Namespace

`Plenty\Modules\Frontend\LegalInformation\Contracts`





#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="frontend#frontend_models_legalinformation">LegalInformation</a>
</pre>

    
Get legal information of an online store
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The ID of the online store</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the legal information text as ISO 639-1 code, e.g. e.g. en for English</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of the legal information text. The types available are:
<ul>
<li>TermsConditions</li>
<li>CancellationRights</li>
<li>PrivacyPolicy</li>
<li>LegalDisclosure</li>
<li>WithdrawalForm</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>save</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="frontend#frontend_models_legalinformation">LegalInformation</a>
</pre>

    
Save legal information for an online store
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Array of data for 'plainText' and 'htmlText'</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The plenty ID of the online store</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the legal information text as ISO 639-1 code, e.g. en for English</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of the legal information text. The types available are:
<ul>
<li>TermsConditions</li>
<li>CancellationRights</li>
<li>PrivacyPolicy</li>
<li>LegalDisclosure</li>
<li>WithdrawalForm</li>
</ul></td>
    </tr>
</table>


## Models<a name="frontend_legalinformation_models"></a>
### LegalInformation<a name="frontend_models_legalinformation"></a>

The legal information model.


#### Namespace

`Plenty\Modules\Frontend\LegalInformation\Models`




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
            <td>plentyId</td>
            <td>The unique identifier of the plenty client</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the legal information text</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the legal information text. The types available are:
<ul>
<li>TermsConditions</li>
<li>CancellationRights</li>
<li>PrivacyPolicy</li>
<li>LegalDisclosure</li>
<li>WithdrawalForm</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plainText</td>
            <td>The text value of the legal information text</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>htmlText</td>
            <td>The html value of the legal information text</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Storage<a name="frontend_storage"></a>
    
## Contracts<a name="frontend_storage_contracts"></a>
### FrontendSessionStorageFactoryContract<a name="frontend_contracts_frontendsessionstoragefactorycontract"></a>

The FrontendSessionStorageFactoryContract is the interface for the front end session storage repository. This interface allows to get information about the locale, the customer, the order, the plugin and the forum from the session.


#### Namespace

`Plenty\Modules\Frontend\Session\Storage\Contracts`





#### Methods

<pre>public <strong>getLocaleSettings</strong>():<a href="frontend#frontend_models_localesettings">LocaleSettings</a>
</pre>

    
Get the locale settings from the session storage.
    
<pre>public <strong>getCustomer</strong>():<a href="frontend#frontend_models_customer">Customer</a>
</pre>

    
Get the customer data from the session storage.
    
<pre>public <strong>getOrder</strong>():<a href="frontend#frontend_models_order">Order</a>
</pre>

    
Get the order data from the session storage.
    
<pre>public <strong>getPlugin</strong>():<a href="frontend#frontend_models_plugin">Plugin</a>
</pre>

    
Get the plugin data from the session storage.
    
<pre>public <strong>getForum</strong>():<a href="frontend#frontend_models_forum">Forum</a>
</pre>

    
Get the forum data from the session storage.
    
## Models<a name="frontend_storage_models"></a>
### Forum<a name="frontend_models_forum"></a>

The session storage model for forum data.


#### Namespace

`Plenty\Modules\Frontend\Session\Storage\Models`




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
            <td>forumGroupId</td>
            <td>The ID of the forum group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forumUsername</td>
            <td>The name of the user in the forum</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>forumConfig</td>
            <td>The forum configuration</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>forumPermissions</td>
            <td>The forum permissions</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>forumLastVisitTime</td>
            <td>The time the forum was visited last</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Order<a name="frontend_models_order"></a>

The session storage model for order data.


#### Namespace

`Plenty\Modules\Frontend\Session\Storage\Models`




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
            <td>deliveryAddressId</td>
            <td>The ID of the delivery address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>invoiceAddressId</td>
            <td>The ID of the invoice address</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parcelServiceId</td>
            <td>The ID of the parcel service</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parcelServicePresetId</td>
            <td>The preset ID of the parcel service</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>methodOfPayment</td>
            <td>The payment method</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isNet</td>
            <td>Flag that indicates if the shown price is the net price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingCosts</td>
            <td>The shipping costs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderinfoText</td>
            <td>Additional information specified by the customer in the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>payDataComplete</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemOrderParams</td>
            <td>The parameters of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>uploadedFileStack</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>trustedShopBuyerProtection</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopApplicationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>coupon</td>
            <td>The coupon code</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>couponDisplay</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>activePaymentMethodsList</td>
            <td>A list of active payment methods</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td>The ID of the order referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerPriceColumn</td>
            <td>The price column for the order referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerItemId</td>
            <td>The ID of the item referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerId</td>
            <td>The ID of the subscription</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerIntervalId</td>
            <td>The ID of the interval of a subscription</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerOrderExecutionId</td>
            <td>The ID for the execution of the order</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerFirstDeliveryDate</td>
            <td>The date for the first delivery of a subscription</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Plugin<a name="frontend_models_plugin"></a>

The session storage model for plugins.


#### Namespace

`Plenty\Modules\Frontend\Session\Storage\Models`





#### Methods

<pre>public <strong>setValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Updates the value of a key. The key and the new value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Gets a value for a key. The key must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>unsetKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $key):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Unsets a key. The key must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>



### LocaleSettings<a name="frontend_models_localesettings"></a>

The session storage model for locale settings.


#### Namespace

`Plenty\Modules\Frontend\Session\Storage\Models`




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
            <td>The currency</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>currencyExchange</td>
            <td>The exchange rate for the currency</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>language</td>
            <td>The language</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Customer<a name="frontend_models_customer"></a>

The session storage model for customer data.


#### Namespace

`Plenty\Modules\Frontend\Session\Storage\Models`




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
            <td>deliveryCountryId</td>
            <td>The ID of the country of delivery</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>showNetPrice</td>
            <td>Flag that indicates if the shown price is the net price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ebaySellerAccount</td>
            <td>The eBay seller account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountContactSign</td>
            <td>The reference sign specified by the contact</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountContactClassId</td>
            <td>The ID of the contact class</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sourceItemWishListAccountContactId</td>
            <td>The ID of the contact that created the wish list</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sourceItemWishListAccountAddressId</td>
            <td>The ID of the address that created the wish list</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>salesAgent</td>
            <td>The sales representative</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
