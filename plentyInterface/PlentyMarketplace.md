

# PlentyMarketplace<a name="plentymarketplace_plentymarketplace"></a>
    
## Contracts<a name="plentymarketplace_plentymarketplace_contracts"></a>
### SubscriptionInformationServiceContract<a name="plentymarketplace_contracts_subscriptioninformationservicecontract"></a>

Get information about plugin subscriptions. Only suitable for subscription plugins.


#### Namespace

`Plenty\Modules\PlentyMarketplace\Contracts`





#### Methods

<pre>public <strong>isPaid</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Takes the Name of a subscription plugin and returns true if the subscription has been paid for
in the current payment period on the current system.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>The plugin name. Must be exactly as provided in the plugin.json.</td>
    </tr>
</table>


<pre>public <strong>getSubscriptionInfo</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName):<a href="plentymarketplace#plentymarketplace_models_subscriptionorderinformation">SubscriptionOrderInformation</a>
</pre>

    
Takes the Name of a subscription plugin and returns information about the subscription.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>The plugin name. Must be exactly as provided in the plugin.json.</td>
    </tr>
</table>


## Models<a name="plentymarketplace_plentymarketplace_models"></a>
### SubscriptionChildOrderInformation<a name="plentymarketplace_models_subscriptionchildorderinformation"></a>

Eloquent model representing a SubscriptionChildOrderInformation.


#### Namespace

`Plenty\Modules\PlentyMarketplace\Models`




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
            <td>paymentStatus</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>paymentInformation</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SubscriptionOrderInformation<a name="plentymarketplace_models_subscriptionorderinformation"></a>

Eloquent model representing a SubscriptionOrderInformation.


#### Namespace

`Plenty\Modules\PlentyMarketplace\Models`




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
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isPaid</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>intervalType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>intervalValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>startDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>subscriptionLastRun</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>subscriptionNextRun</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>childOrders</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SubscriptionChildPaymentInformation<a name="plentymarketplace_models_subscriptionchildpaymentinformation"></a>

Eloquent model representing a SubscriptionChildPaymentInformation.


#### Namespace

`Plenty\Modules\PlentyMarketplace\Models`




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
            <td>The amount of the payment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>status</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses"  target="_blank">status</a> of the payment</td>
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
            <td>receivedAt</td>
            <td>The time the payment was received</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>importedAt</td>
            <td>The time the payment was imported</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
