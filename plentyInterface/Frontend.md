

# Frontend<a name="frontend_frontend"></a>
    
## Contracts<a name="frontend_frontend_contracts"></a>
### Checkout<a name="frontend_contracts_checkout"></a>

checkout service

#### Namespace

Plenty\Modules\Frontend\Contracts



#### Methods

<pre>public <strong>setShippingCountryId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingCountryId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingCountryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPaymentMethodId</strong>(<a target="_blank" href="http://php.net/int">int</a> $paymentMethodId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setShippingProfileId</strong>(<a target="_blank" href="http://php.net/int">int</a> $shippingProfileId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingProfileId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setCurrency</strong>(<a target="_blank" href="http://php.net/string">string</a> $currency):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$currency</td>
        <td></td>
    </tr>
</table>


## Events<a name="frontend_frontend_events"></a>
### FrontendCurrencyChanged<a name="frontend_events_frontendcurrencychanged"></a>

currency changed event

#### Namespace

Plenty\Modules\Frontend\Events



#### Methods

<pre>public <strong>getCurrency</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>
    

    
<pre>public <strong>getCurrencyExchangeRatio</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>
    

    

### FrontendLanguageChanged<a name="frontend_events_frontendlanguagechanged"></a>

language changed event

#### Namespace

Plenty\Modules\Frontend\Events



#### Methods

<pre>public <strong>getLanguage</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>
    

    

### FrontendUpdateDeliveryAddress<a name="frontend_events_frontendupdatedeliveryaddress"></a>

delivery address changed event

#### Namespace

Plenty\Modules\Frontend\Events



#### Methods

<pre>public <strong>getAccountAddressId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    

### FrontendUpdatePaymentSettings<a name="frontend_events_frontendupdatepaymentsettings"></a>

payment settings changed event

#### Namespace

Plenty\Modules\Frontend\Events



#### Methods

<pre>public <strong>getPaymentMethodId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    

### FrontendUpdateShippingSettings<a name="frontend_events_frontendupdateshippingsettings"></a>

shipping settings changed event

#### Namespace

Plenty\Modules\Frontend\Events



#### Methods

<pre>public <strong>getShippingCosts</strong>():<a target="_blank" href="http://php.net/float">float</a></pre>
    

    
<pre>public <strong>getParcelServiceId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    
<pre>public <strong>getParcelServicePresetId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    
## Factories<a name="frontend_frontend_factories"></a>
### FrontendFactory<a name="frontend_factories_frontendfactory"></a>

Frontend-Factory

#### Namespace

Plenty\Modules\Frontend\Factories



#### Methods

<pre>public <strong>getAgent</strong>():<a href="frontend#frontend_services_agentservice">AgentService</a>
</pre>
    

    
<pre>public <strong>getSystem</strong>():<a href="frontend#frontend_services_systemservice">SystemService</a>
</pre>
    

    
<pre>public <strong>getAccount</strong>():<a href="frontend#frontend_services_accountservice">AccountService</a>
</pre>
    

    
<pre>public <strong>getFile</strong>():<a href="frontend#frontend_services_fileservice">FileService</a>
</pre>
    

    
## Services<a name="frontend_frontend_services"></a>
### AccountService<a name="frontend_services_accountservice"></a>

Frontend-service for customer information

#### Namespace

Plenty\Modules\Frontend\Services



#### Methods

<pre>public <strong>getIsAccountLoggedIn</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>
    

    
<pre>public <strong>getAccountContactId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    

### AgentService<a name="frontend_services_agentservice"></a>

Frontend-Service for agent information

#### Namespace

Plenty\Modules\Frontend\Services



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
    

    

### FileService<a name="frontend_services_fileservice"></a>

Frontend-service for file information

#### Namespace

Plenty\Modules\Frontend\Services



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


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
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
    

    

### SystemService<a name="frontend_services_systemservice"></a>

Frontend-service for system information

#### Namespace

Plenty\Modules\Frontend\Services



#### Methods

<pre>public <strong>getPlentyId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    
<pre>public <strong>getWebstoreId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>
    

    
# PaymentMethod<a name="frontend_paymentmethod"></a>
    
## Contracts<a name="frontend_paymentmethod_contracts"></a>
### FrontendPaymentMethodRepositoryContract<a name="frontend_contracts_frontendpaymentmethodrepositorycontract"></a>

Repository to load payment methods for the front end

#### Namespace

Plenty\Modules\Frontend\PaymentMethod\Contracts



#### Methods

<pre>public <strong>getCurrentPaymentMethodsList</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
<pre>public <strong>getPaymentMethodName</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/string">string</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodFee</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/float">float</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodIcon</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/string">string</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentMethodDescription</strong>(<a href="payment#payment_models_paymentmethod">PaymentMethod</a>
 $paymentMethod):<a target="_blank" href="http://php.net/string">string</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="payment#payment_models_paymentmethod">PaymentMethod</a>
</td>
        <td>$paymentMethod</td>
        <td></td>
    </tr>
</table>


# Storage<a name="frontend_storage"></a>
    
## Contracts<a name="frontend_storage_contracts"></a>
### FrontendSessionStorageFactoryContract<a name="frontend_contracts_frontendsessionstoragefactorycontract"></a>

session storage for frontend

#### Namespace

Plenty\Modules\Frontend\Session\Storage\Contracts



#### Methods

<pre>public <strong>getLocaleSettings</strong>():<a href="frontend#frontend_models_localesettings">LocaleSettings</a>
</pre>
    

    
<pre>public <strong>getCustomer</strong>():<a href="frontend#frontend_models_customer">Customer</a>
</pre>
    

    
<pre>public <strong>getOrder</strong>():<a href="frontend#frontend_models_order">Order</a>
</pre>
    

    
<pre>public <strong>getPlugin</strong>():<a href="frontend#frontend_models_plugin">Plugin</a>
</pre>
    

    
<pre>public <strong>getForum</strong>():<a href="frontend#frontend_models_forum">Forum</a>
</pre>
    

    
## Models<a name="frontend_storage_models"></a>
### Customer<a name="frontend_models_customer"></a>

session storage model for customer data

#### Namespace

Plenty\Modules\Frontend\Session\Storage\Models


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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>showNetPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ebaySellerAccount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>accountContactSign</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountContactClassId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sourceItemWishListAccountContactId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sourceItemWishListAccountAddressId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>salesAgent</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### Forum<a name="frontend_models_forum"></a>

session storage model for forum data

#### Namespace

Plenty\Modules\Frontend\Session\Storage\Models


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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forumUsername</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>forumConfig</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>forumPermissions</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>forumLastVisitTime</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### LocaleSettings<a name="frontend_models_localesettings"></a>

session storage model for locale settings

#### Namespace

Plenty\Modules\Frontend\Session\Storage\Models


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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>currencyExchange</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>language</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### Order<a name="frontend_models_order"></a>

session storage model for order data

#### Namespace

Plenty\Modules\Frontend\Session\Storage\Models


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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parcelServiceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parcelServicePresetId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>methodOfPayment</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingCosts</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderinfoText</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>payDataComplete</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemOrderParams</td>
            <td></td>
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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>couponDisplay</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>activePaymentMethodsList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerPriceColumn</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerItemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerIntervalId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerOrderExecutionId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerFirstDeliveryDate</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### Plugin<a name="frontend_models_plugin"></a>

session storage model for plugins

#### Namespace

Plenty\Modules\Frontend\Session\Storage\Models



#### Methods

<pre>public <strong>setValue</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
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
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


