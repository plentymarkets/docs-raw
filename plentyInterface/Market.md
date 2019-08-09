

# Settings<a name="market_settings"></a>
    
## Contracts<a name="market_settings_contracts"></a>
### SettingsRepositoryContract<a name="market_contracts_settingsrepositorycontract"></a>

Use this interface to store and retrieve market specific settings.


#### Namespace

`Plenty\Modules\Market\Settings\Contracts`





#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = \Plenty\Modules\Market\Settings\Models\Settings::MAX_ITEMS_PER_PAGE):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List settings.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Settings can be filtered by ID, marketplace ID.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>Current page of the response.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The requested amount of settings per result page.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $marketplaceId, <a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/array">array</a> $settings):<a href="market#market_models_settings">Settings</a>
</pre>

    
Create market settings.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$marketplaceId</td>
        <td>The marketplace ID that the settings belong to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The type of settings. Possible values: shipping, attribute, category, property.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$settings</td>
        <td>The settings that will be saved.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $settingsData, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update one market settings entry.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$settingsData</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_settings">Settings</a>
</pre>

    
Return the settings for a given settings ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The settings id.</td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/string">string</a> $marketplaceId, <a target="_blank" href="http://php.net/string">string</a> $type = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Find settings for a given marketplace ID and type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$marketplaceId</td>
        <td>The marketplace id for which to retrieve the settings</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The typo of settings that should be searched for. Possible values: shipping, attribute, category, property.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteAll</strong>(<a target="_blank" href="http://php.net/string">string</a> $marketplaceId, <a target="_blank" href="http://php.net/string">string</a> $type):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete all settings for a given type and marketplace ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="market_settings_models"></a>
### Settings<a name="market_models_settings"></a>

The market settings model.


#### Namespace

`Plenty\Modules\Market\Settings\Models`




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
            <td>The ID of the market settings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketplaceId</td>
            <td>The ID of the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the current market settings. Possible values are: attribute, attributeValue, property, category, shipping.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>settings</td>
            <td>The market settings for the current marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>category</td>
            <td>The category that these market settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>parcelServicePreset</td>
            <td>The parcel service preset that these market settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attribute</td>
            <td>The attribute that these market settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>property</td>
            <td>The property item that these market settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attributeValue</td>
            <td>The attributeValue that these market settings are related to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Factories<a name="market_settings_factories"></a>
### SettingsCorrelationFactory<a name="market_factories_settingscorrelationfactory"></a>

Factory that allows to store correlation between market settings and plentymarkets settings.


#### Namespace

`Plenty\Modules\Market\Settings\Factories`





#### Methods

<pre>public <strong>type</strong>(<a target="_blank" href="http://php.net/string">string</a> $type):<a href="market#market_factories_settingscorrelationfactory">SettingsCorrelationFactory</a>
</pre>

    
Set here the type of relation that should be created.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The relation type. Possible values: shipping, attribute, category, property</td>
    </tr>
</table>


<pre>public <strong>createRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $settingsId, <a target="_blank" href="http://php.net/int">int</a> $correlationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Use this method to create a relation of the chosen type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$settingsId</td>
        <td>The id of the market settings we want to create the relation for.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td>The id of the plentymarkets settings we want to create the relation to.</td>
    </tr>
</table>


<pre>public <strong>createRelationWithParent</strong>(<a target="_blank" href="http://php.net/int">int</a> $settingsId, <a target="_blank" href="http://php.net/int">int</a> $correlationId, <a target="_blank" href="http://php.net/int">int</a> $parentSettingsId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Use this method to create a relation of the chosen type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$settingsId</td>
        <td>The id of the market settings we want to create the relation for.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td>The id of the plentymarkets settings we want to create the relation to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parentSettingsId</td>
        <td>The id of the parent market settings we want to create the relation to.</td>
    </tr>
</table>


<pre>public <strong>clear</strong>($marketplaceId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clear all relations for a given correlation type.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>($marketplaceId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all correlations for a given marketplace ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSettingsByCorrelation</strong>($marketplaceId, <a target="_blank" href="http://php.net/int">int</a> $correlationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a specific settings by marketplace id and correlation id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAllSettingsByCorrelation</strong>($marketplaceId, <a target="_blank" href="http://php.net/int">int</a> $correlationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a specific settings by marketplace id and correlation id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSettingsByCorrelationAndParent</strong>($marketplaceId, <a target="_blank" href="http://php.net/int">int</a> $correlationId, <a target="_blank" href="http://php.net/int">int</a> $parentSettingsId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a specific settings by marketplace id and correlation id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parentSettingsId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSettingsByParent</strong>($marketplaceId, <a target="_blank" href="http://php.net/int">int</a> $parentSettingsId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List settings by marketplace id and parent settings id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parentSettingsId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAllSettingsByCorrelationAndParent</strong>($marketplaceId, <a target="_blank" href="http://php.net/int">int</a> $correlationId, <a target="_blank" href="http://php.net/int">int</a> $parentSettingsId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a specific settings by marketplace id and correlation id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$correlationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$parentSettingsId</td>
        <td></td>
    </tr>
</table>


# Transaction<a name="market_transaction"></a>
    
## Contracts<a name="market_transaction_contracts"></a>
### TransactionRepositoryContract<a name="market_contracts_transactionrepositorycontract"></a>

The contract for the ebay transaction repository.


#### Namespace

`Plenty\Modules\Market\Ebay\Transaction\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_transaction">Transaction</a>
</pre>

    
Gets a transaction.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the ebay transaction.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Search ebay transactions
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that could be applied: 'orderId', 'externalOrderId'.</td>
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
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
## Models<a name="market_transaction_models"></a>
### Transaction<a name="market_models_transaction"></a>

The ebay transaction model.


#### Namespace

`Plenty\Modules\Market\Ebay\Transaction\Models`




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
            <td>The ID of the transaction.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderId</td>
            <td>The ID of the plentymarkets order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>market</td>
            <td>The market. Possible values are: 'ebay', 'hood', 'ricardo'</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalListingId</td>
            <td>The ID of the external listing.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>credentialsId</td>
            <td>The ID of the credentials.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>buyerUserId</td>
            <td>The ID of the ebay buyer.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedback</td>
            <td>The feedback.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>transactionId</td>
            <td>The ID of the ebay transaction.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>endTime</td>
            <td>The date that the item was bought.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The purchased quantity.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the purchased item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td>The price of the transaction.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingAddressCountry</td>
            <td>The shipping address country.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td>The ID of the order referrer.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the transaction was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>notification</td>
            <td>Flag that indicates if the transaction import was by notification.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderRowId</td>
            <td>The ID of the order row.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sku</td>
            <td>The SKU.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lastUpdate</td>
            <td>The date that the transaction was last updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalOrderId</td>
            <td>The ID of the external order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalReferenceNo</td>
            <td>The external reference number.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>cancelId</td>
            <td>The ID of the cancellation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isEbayPlus</td>
            <td>The transaction is ebay plus. Possible values are: 'YES', 'NO'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isClickAndCollect</td>
            <td>The transaction is click and collect. Possible values are: 'YES', 'NO'.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Category<a name="market_category"></a>
    
## Contracts<a name="market_category_contracts"></a>
### CategoryRepositoryContract<a name="market_contracts_categoryrepositorycontract"></a>

The contract for the Ebay category repository.


#### Namespace

`Plenty\Modules\Market\Ebay\Category\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="market#market_models_category">Category</a>
</pre>

    
Get category
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the category.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that could be applied: 'marketplaceId'.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations that should be loaded: 'path'</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/array">array</a> $with = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all categories
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Categories can be filtered by ID and marketplace ID. The filters that could be applied: 'marketplaceId', 'categoryId'.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations that should be loaded: 'path'</td>
    </tr>
</table>


## Models<a name="market_category_models"></a>
### Category<a name="market_models_category"></a>

The category model


#### Namespace

`Plenty\Modules\Market\Ebay\Category\Models`




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
            <td>The ID of the category.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentId</td>
            <td>The parent category ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the category.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isLeaf</td>
            <td>Tells if the category is leaf.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>children</td>
            <td>Child categories.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>path</td>
            <td>The category path.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Auth<a name="market_auth"></a>
    
## Contracts<a name="market_auth_contracts"></a>
### AuthServiceContract<a name="market_contracts_authservicecontract"></a>

The contract for the eBay authentication service.


#### Namespace

`Plenty\Modules\Market\Ebay\Auth\Contracts`





#### Methods

<pre>public <strong>refreshTokenByCredentialsId</strong>(<a target="_blank" href="http://php.net/int">int</a> $credentialsId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Refresh credentials token and update.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$credentialsId</td>
        <td></td>
    </tr>
</table>


# AccountPolicy<a name="market_accountpolicy"></a>
    
## Contracts<a name="market_accountpolicy_contracts"></a>
### ReturnPolicyRepositoryContract<a name="market_contracts_returnpolicyrepositorycontract"></a>

The contract for the eBay return policy repository.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $id, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="market#market_models_returnpolicy">ReturnPolicy</a>
</pre>

    
Get a stored return policy based on ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td>The ID of the policy that we want to get</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>A list of filters that are needed to get the corresponding policy. Available: `marketplaceId´, `credentialsId´.</td>
    </tr>
</table>



### FulfillmentPolicyRepositoryContract<a name="market_contracts_fulfillmentpolicyrepositorycontract"></a>

The contract for the eBay fulfillment policy repository.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $id, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</pre>

    
Get a stored fulfillment policy based on ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td>The ID of the policy that we want to get</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>A list of filters that are needed to get the corresponding policy. Available: `marketplaceId´, `credentialsId´.</td>
    </tr>
</table>



### PaymentPolicyRepositoryContract<a name="market_contracts_paymentpolicyrepositorycontract"></a>

The contract for the eBay payment policy repository.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $id, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</pre>

    
Get a stored payment policy based on ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$id</td>
        <td>The ID of the payment policy.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>A list of filters that are needed to get the corresponding policy. Available: `marketplaceId´, `credentialsId´.</td>
    </tr>
</table>


## Models<a name="market_accountpolicy_models"></a>
### PaymentMethod<a name="market_models_paymentmethod"></a>

The eBay payment method model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>brands</td>
            <td>A list of credit card brands accepted by the seller. This field is required if the paymentMethodType is set to CREDIT_CARD.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paymentMethodType</td>
            <td>The payment method, selected from the supported payment method types..</td>
        </tr><tr>
            <td><a href="market#market_models_recipientaccountreference">RecipientAccountReference</a>
</td>
            <td>recipientAccountReference</td>
            <td>Information that is used to identify the recipient's account to which electronic funds are sent. This field is required if the payment method is set to PAYPAL, and the field must contain the email address associated with the PayPal account selected by the seller.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Deposit<a name="market_models_deposit"></a>

The eBay deposit model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>amount</td>
            <td>Deposits are used only with Motors listings and the amount value indicates the initial deposit that a buyer must make to purchase a motor vehicle. Deposits on motor vehicles can only be paid using PayPal, so if you specify a deposit amount, then you must also set the paymetMethodType value to 'PayPal'.</td>
        </tr><tr>
            <td><a href="market#market_models_timeduration">TimeDuration</a>
</td>
            <td>dueIn</td>
            <td>Indicates the number of hours the buyer has (after they commit to buy) to make an initial deposit to the seller as a down payment on a motor vehicle.</td>
        </tr><tr>
            <td><a href="market#market_models_paymentmethod">PaymentMethod</a>
</td>
            <td>paymentMethods</td>
            <td>A list of accepted payment methods. For deposits (which are applicable to only motor listings), the paymentMethodType must be set to 'PayPal'</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ShippingService<a name="market_models_shippingservice"></a>

The eBay shipping service model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>additionalShippingCost</td>
            <td>The cost of shipping each additional item if the same buyer purchases a multiple quantity of the same line item. This field is applicable for policies that cover multiple-quantity, fixed-price listings and is not applicable for policies that apply to single-quantity listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>buyerResponsibleForPickup</td>
            <td>This field is only applicable to vehicle categories on eBay Motors (US and Canada). If set to true, the buyer is responsible for picking up the vehicle. Otherwise, the seller should specify the vehicle pickup arrangements in the item description.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>buyerResponsibleForShipping</td>
            <td>This field is applicable for only items listed in vehicle categories on eBay Motors (US and Canada). If set to true, the buyer is responsible for the shipment of the vehicle. Otherwise, the seller should specify the vehicle shipping arrangements in the item description.</td>
        </tr><tr>
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>cashOnDeliveryFee</td>
            <td>The value indicates the Cash on Delivery (COD) fee that the seller charges if the buyer uses the CASH_ON_DELIVERY payment method.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>freeShipping</td>
            <td>The seller can set this flag to true if they want to offer free shipping to the buyer. This field can only be included and set to 'true' for the first domestic shipping service option specified in the shippingServices container</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingCarrierCode</td>
            <td>The shipping carrier, such as 'USPS', 'FedEx', 'UPS', and so on.</td>
        </tr><tr>
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>shippingCost</td>
            <td>For shipping options that use a FLAT_RATE cost type, the amount is the shipping cost for the selected shipping carrier and service. The amount supplied must exclude any additional shipping charges (such as the seller's handling charges or insurance).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingServiceCode</td>
            <td>The shipping service that the shipping carrier uses to ship an item. For example, an overnight, two-day delivery, or other type of service.</td>
        </tr><tr>
            <td><a href="market#market_models_regionset">RegionSet</a>
</td>
            <td>shipToLocations</td>
            <td>This object contains the regionIncluded and regionExcluded fields that define the list of geographical regions that the seller ships to and the list of regions where they do not ship.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sortOrder</td>
            <td>This integer value controls the order that this shipping service option appears in the View Item and Checkout pages, as related to the other specified shipping service options.</td>
        </tr><tr>
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>surcharge</td>
            <td>A fee that can be charged to US buyers when they have an item shipped via UPS or FedEx to Alaska, Hawaii or Puerto Rico.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Region<a name="market_models_region"></a>

The eBay region model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>regionName</td>
            <td>A string that indicates the name of a region, as defined by eBay. A "region" can be either a 'world region' (e.g., the "Middle East" or "Southeast Asia") or a country, as represented with a two-letter country code.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>regionType</td>
            <td>Available values: `COUNTRY`, `COUNTRY_REGION`, `STATE_OR_PROVINCE`, `WORLD_REGION`, `WORLDWIDE`.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### AmountType<a name="market_models_amounttype"></a>

The eBay amount type model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>The base currency applied to the value field to establish a monetary amount. The currency is represented as a 3-letter ISO4217 currency code. For example, the code for the Canadian Dollar is CAD.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The value of the monetary amount in the specified currency.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PaymentPolicy<a name="market_models_paymentpolicy"></a>

The eBay payment policy model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>paymentPolicyId</td>
            <td>The ID of the payment policy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>categoryTypes</td>
            <td>The CategoryTypeEnum value to which this policy applies. The category type discerns whether the policy covers the sale of motor vehicles (via eBay Motors), or the sale of everything except motor vehicles.</td>
        </tr><tr>
            <td><a href="market#market_models_deposit">Deposit</a>
</td>
            <td>deposit</td>
            <td>A container that describes the details of a deposit. Used only with motor listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>An optional seller-defined description of the payment policy. (Max length: 250)</td>
        </tr><tr>
            <td><a href="market#market_models_timeduration">TimeDuration</a>
</td>
            <td>fullPaymentDueIn</td>
            <td>Indicates the number of days that a buyer has to make their full payment to the seller, and close the remaining balance on a motor vehicle transaction. The period starts when the buyer commits to buy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>immediatePay</td>
            <td>Indicate if the payment is due upon receipt or not. (eBay generates a receipt when the buyer agrees to purchase an item)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketplaceId</td>
            <td>The ID of the eBay marketplace to which this return policy applies. If this value is not specified, value defaults to the seller's eBay registration site.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>A user-defined name for this payment policy. Names must be unique for policies assigned to the same marketplace. (Max length: 64)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>paymentInstructions</td>
            <td>Allows the seller to give payment instructions to the buyer. These instructions appear on the eBay View Item and Checkout pages.</td>
        </tr><tr>
            <td><a href="market#market_models_paymentmethod">PaymentMethod</a>
</td>
            <td>paymentMethods</td>
            <td>A list of the payment methods accepted by the seller. Each payment policy must specify at least one payment method.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ShippingOption<a name="market_models_shippingoption"></a>

The eBay shipping option model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>costType</td>
            <td>Defines whether the shipping cost is `FLAT_RATE`, `CALCULATED`, or `NOT_SPECIFIED` (for use with freight shipping and local pickup)</td>
        </tr><tr>
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>insuranceFee</td>
            <td>Sellers can offer international shipping insurance only when they ship to AU, FR, or IT. This value indicates the cost the buyer must pay to purchase shipping insurance for the items being shipped.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>insuranceOffered</td>
            <td>When set to true, it indicates the seller offers shipping insurance.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>optionType</td>
            <td>Use this field to set the ShippingOption element to either `DOMESTIC` or `INTERNATIONAL`</td>
        </tr><tr>
            <td><a href="market#market_models_amounttype">AmountType</a>
</td>
            <td>packageHandlingCost</td>
            <td>A fee a seller can add to cover package and handling costs. This fee is in addition to the amount of the selected shipping service and this fee is included in the final shipping service costs in the output.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>rateTableId</td>
            <td>A unique eBay-assigned ID associated with a user-created shipping rate table.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>shippingServices</td>
            <td>Contains a list of shipping services offered for either `DOMESTIC` or `INTERNATIONAL` shipments.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CategoryType<a name="market_models_categorytype"></a>

The eBay category type model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>default</td>
            <td>If this value is set to true, it indicates that this policy is the default policy for the associated categoryTypes.name and marketplaceId pair</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The category type to which the policy applies (motor vehicles or non-motor vehicles). Available values: `MOTORS_VEHICLES`, `ALL_EXCLUDING_MOTORS_VEHICLES`</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FulfillmentPolicy<a name="market_models_fulfillmentpolicy"></a>

The eBay fulfillment policy model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>fulfillmentPolicyId</td>
            <td>The ID of the fulfillment policy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>categoryTypes</td>
            <td>The CategoryTypeEnum value to which this policy applies. Used to discern accounts that sell motor vehicles from those that don't. (Currently, each policy can be set to only one categoryTypes value at a time.)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>An optional seller-defined description of the fulfillment policy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>freightShipping</td>
            <td>Set this value to true to indicate the seller offers freight shipping.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>globalShipping</td>
            <td>If this value is set to true, it indicates the seller has opted-in to the eBay Global Shipping Program and that they use that service for thier internation shipments.</td>
        </tr><tr>
            <td><a href="market#market_models_timeduration">TimeDuration</a>
</td>
            <td>handlingTime</td>
            <td>Specifies the maximum number of business days the seller commits to for preparing and shipping an order after receiving a cleared payment for the order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>localPickup</td>
            <td>If this value is set to true, it indicates the seller offers local pickup of their items.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketplaceId</td>
            <td>The ID of the eBay marketplace to which this fulfillment policy applies. If this value is not specified, value defaults to the seller's eBay registration site.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>A user-defined name for this fulfillment policy. Names must be unique for policies assigned to the same marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>pickupDropOff</td>
            <td>If this value is set to true, it indicates the seller offers the "Click and Collect" feature.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>shippingOptions</td>
            <td>A list that defines the seller's shipping configurations for DOMESTIC and INTERNATIONAL order shipments.</td>
        </tr><tr>
            <td><a href="market#market_models_regionset">RegionSet</a>
</td>
            <td>shipToLocations</td>
            <td>This object contains the regionIncluded and regionExcluded fields, which indicate the areas to where the seller does and dosen't ship.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ReturnPolicy<a name="market_models_returnpolicy"></a>

The eBay return policy model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>returnPolicyId</td>
            <td>The ID of the return policy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>categoryTypes</td>
            <td>For return policies, this field can be set to only `ALL_EXCLUDING_MOTORS_VEHICLES (returns on motor vehicles are not processed through eBay flows.)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>An optional seller-defined description of the return policy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>extendedHolidayReturnsOffered</td>
            <td>If this value is set to true, it indicates the seller offers an Extended Holiday Returns policy for their listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketplaceId</td>
            <td>The ID of the eBay marketplace to which this return policy applies. If this value is not specified, value defaults to the seller's eBay registration site.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>A user-defined name for this fulfillment policy. Names must be unique for policies assigned to the same marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>refundMethod</td>
            <td>Indicates the method the seller uses to compensate the buyer for returned items. The return method specified applies only to remorse returns. Available options: `MERCHANDISE_CREDIT`, `MONEY_BACK`.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>restockingFeePercentage</td>
            <td>Sellers who accept returns should include this field if they charge buyers a restocking fee when items are returned.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>returnInstruction</td>
            <td>This optional free-form string field lets the seller provide a detailed explanation of the return policy.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>returnMethod</td>
            <td>This field indicates the method in which the seller handles non-money back return requests for remorse returns. Sellers can specify they either exchange or replace items. Available options: `EXCHANGE`, `REPLACEMENT`.</td>
        </tr><tr>
            <td><a href="market#market_models_timeduration">TimeDuration</a>
</td>
            <td>returnPeriod</td>
            <td>This value indicates the length of time the seller accepts returns, the duration of which starts when the buyer receives the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>returnsAccepted</td>
            <td>Set this value to true to indicate the seller accepts returns.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>returnShippingCostPayer</td>
            <td>The seller uses this value to specify whether the buyer or the seller is responsible for paying return shipping charges. The field can be set to either `BUYER` or `SELLER`.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RegionSet<a name="market_models_regionset"></a>

The eBay region set model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>regionExcluded</td>
            <td>A list of one or more regionsName fields that specify the areas to where a seller does not ship. Populate regionExcluded in only the top-level shipToLocations container.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>regionIncluded</td>
            <td>A list of one or more regionsName fields that specify the areas to where a seller ships.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TimeDuration<a name="market_models_timeduration"></a>

The eBay time duration model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>unit</td>
            <td>A time-measurement unit used to specify a period of time. Available values: `MONTH`, `DAY`, `HOUR`, `CALENDAR_DAY`, `BUSINESS_DAY`, `MINUTE`, `SECOND`, `MILLISECOND`</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>An amount of time, as measured by the time-measurement units specified in the unit field.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### RecipientAccountReference<a name="market_models_recipientaccountreference"></a>

The eBay recipient account reference model


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Models`




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
            <td>referenceId</td>
            <td>The recipient's reference.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceType</td>
            <td>The reference type of a recipient's account.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="market_accountpolicy_events"></a>
### ReturnPolicyDeleted<a name="market_events_returnpolicydeleted"></a>

An event class fired after a new return policy is deleted.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_returnpolicy">ReturnPolicy</a>
 $returnPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_returnpolicy">ReturnPolicy</a>
</td>
        <td>$returnPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getReturnPolicy</strong>():<a href="market#market_models_returnpolicy">ReturnPolicy</a>
</pre>

    
Get the ReturnPolicy instance.
    

### FulfillmentPolicyDeleted<a name="market_events_fulfillmentpolicydeleted"></a>

An event class fired after a new fulfillment policy is deleted.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
 $fulfillmentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</td>
        <td>$fulfillmentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFulfillmentPolicy</strong>():<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</pre>

    
Get the FulfillmentPolicy instance.
    

### FulfillmentPolicyEvent<a name="market_events_fulfillmentpolicyevent"></a>

A base event class for all fulfillment policy events. Each fulfillment policy events expects an FulfillmentPolicy model.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
 $fulfillmentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</td>
        <td>$fulfillmentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFulfillmentPolicy</strong>():<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</pre>

    
Get the FulfillmentPolicy instance.
    

### PaymentPolicyDeleted<a name="market_events_paymentpolicydeleted"></a>

An event class fired after a new payment policy is deleted.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
 $paymentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</td>
        <td>$paymentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentPolicy</strong>():<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</pre>

    
Get the PaymentPolicy instance.
    

### PaymentPolicyEvent<a name="market_events_paymentpolicyevent"></a>

A base event class for all payment policy events. Each payment policy events expects an PaymentPolicy model.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
 $paymentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</td>
        <td>$paymentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentPolicy</strong>():<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</pre>

    
Get the PaymentPolicy instance.
    

### ReturnPolicyCreated<a name="market_events_returnpolicycreated"></a>

An event class fired after a new return policy is created.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_returnpolicy">ReturnPolicy</a>
 $returnPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_returnpolicy">ReturnPolicy</a>
</td>
        <td>$returnPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getReturnPolicy</strong>():<a href="market#market_models_returnpolicy">ReturnPolicy</a>
</pre>

    
Get the ReturnPolicy instance.
    

### PaymentPolicyUpdated<a name="market_events_paymentpolicyupdated"></a>

An event class fired after a new payment policy is updated.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
 $paymentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</td>
        <td>$paymentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentPolicy</strong>():<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</pre>

    
Get the PaymentPolicy instance.
    

### FulfillmentPolicyCreated<a name="market_events_fulfillmentpolicycreated"></a>

An event class fired after a new fulfillment policy is created.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
 $fulfillmentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</td>
        <td>$fulfillmentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFulfillmentPolicy</strong>():<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</pre>

    
Get the FulfillmentPolicy instance.
    

### ReturnPolicyUpdated<a name="market_events_returnpolicyupdated"></a>

An event class fired after a new return policy is updated.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_returnpolicy">ReturnPolicy</a>
 $returnPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_returnpolicy">ReturnPolicy</a>
</td>
        <td>$returnPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getReturnPolicy</strong>():<a href="market#market_models_returnpolicy">ReturnPolicy</a>
</pre>

    
Get the ReturnPolicy instance.
    

### PaymentPolicyCreated<a name="market_events_paymentpolicycreated"></a>

An event class fired after a new payment policy is created.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
 $paymentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</td>
        <td>$paymentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPaymentPolicy</strong>():<a href="market#market_models_paymentpolicy">PaymentPolicy</a>
</pre>

    
Get the PaymentPolicy instance.
    

### ReturnPolicyEvent<a name="market_events_returnpolicyevent"></a>

A base event class for all return policy events. Each return policy events expects an ReturnPolicy model.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_returnpolicy">ReturnPolicy</a>
 $returnPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_returnpolicy">ReturnPolicy</a>
</td>
        <td>$returnPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getReturnPolicy</strong>():<a href="market#market_models_returnpolicy">ReturnPolicy</a>
</pre>

    
Get the ReturnPolicy instance.
    

### FulfillmentPolicyUpdated<a name="market_events_fulfillmentpolicyupdated"></a>

An event class fired after a new fulfillment policy is updated.


#### Namespace

`Plenty\Modules\Market\Ebay\AccountPolicy\Events`





#### Methods

<pre>public <strong>__construct</strong>(<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
 $fulfillmentPolicy):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</td>
        <td>$fulfillmentPolicy</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFulfillmentPolicy</strong>():<a href="market#market_models_fulfillmentpolicy">FulfillmentPolicy</a>
</pre>

    
Get the FulfillmentPolicy instance.
    
# Marketplace<a name="market_marketplace"></a>
    
## Contracts<a name="market_marketplace_contracts"></a>
### MarketplaceRepositoryContract<a name="market_contracts_marketplacerepositorycontract"></a>

The contract for the Ebay marketplace repository.


#### Namespace

`Plenty\Modules\Market\Ebay\Marketplace\Contracts`





#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the list of all available eBay marketplaces.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>You can pass multiple filters to search only custom marketplaces. Available filters: `referrerId`, `marketplaceId`, `marketId`, `siteId`.</td>
    </tr>
</table>


<pre>public <strong>allEbay</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the list of all available eBay marketplaces.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>You can pass multiple filters to search only custom marketplaces. Available filters: `referrerId`, `marketplaceId`, `marketId`, `siteId`.</td>
    </tr>
</table>


## Models<a name="market_marketplace_models"></a>
### Marketplace<a name="market_models_marketplace"></a>

The eBay marketplace model.


#### Namespace

`Plenty\Modules\Market\Ebay\Marketplace\Models`




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
            <td>siteId</td>
            <td>The ID of the site exactly as eBay specifies it in the docs. This value is/was used in the old eBay SOAP APIs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>marketplaceId</td>
            <td>The ID of the marketplace exactly as eBay specifies it in the docs. This value is used in the new eBay REST APIs. Eg. `EBAY_DE` or `EBAY-DE`</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketId</td>
            <td>System-Listing wide internal ID for the listing marketplace. This id occurs only in correlation with the listing DB tables.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>System wide internal ID for the marketplace. Use this instead of `marketId` whenever possible!</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortcut</td>
            <td>The marketplace shortcut name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency used for the marketplace</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Helpers<a name="market_marketplace_helpers"></a>
### MarketplaceHelper<a name="market_helpers_marketplacehelper"></a>

Helper class that allows getting information about an eBay marketplace more easily.


#### Namespace

`Plenty\Modules\Market\Ebay\Marketplace\Helpers`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a href="market#market_models_marketplace">Marketplace</a>
</pre>

    
Get marketplace data model based on filters.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMarketplaceId</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the marketplace ID based on given filters. Possible filters: `marketplaceId`, `referrerId`, `marketId`, `siteId`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMarketplaceIds</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all available marketplace IDs.
    
<pre>public <strong>getReferrerId</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the referrer ID based on given filters. Possible filters: `marketplaceId`, `referrerId`, `marketId`, `siteId`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getReferrerIds</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all available referrer IDs.
    
<pre>public <strong>getSiteId</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the site ID based on given filters. Possible filters: `marketplaceId`, `referrerId`, `marketId`, `siteId`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getSiteIds</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all available site IDs.
    
<pre>public <strong>getMarketId</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the market ID based on given filters. Possible filters: `marketplaceId`, `referrerId`, `marketId`, `siteId`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMarketIds</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all available market IDs.
    
<pre>public <strong>getCurrency</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the currency based on given filters. Possible filters: `marketplaceId`, `referrerId`, `marketId`, `siteId`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getShortcut</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the shortcut based on given filters. Possible filters: `marketplaceId`, `referrerId`, `marketId`, `siteId`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


# Api<a name="market_api"></a>
    
## Types<a name="market_api_types"></a>
### Base64BinaryType<a name="market_types_base64binarytype"></a>

The service for eBay Base64BinaryType.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### TokenType<a name="market_types_tokentype"></a>

The service for token type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### RepeatableType<a name="market_types_repeatabletype"></a>

The service for repeatable type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/string">string</a> $property, <a target="_blank" href="http://php.net/string">string</a> $expectedType):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class that the property is a member of.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$property</td>
        <td>The name of the property that acts like an array.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expectedType</td>
        <td>The type that values assigned to the array should be.</td>
    </tr>
</table>


<pre>public <strong>offsetExists</strong>(<a target="_blank" href="http://php.net/int">int</a> $offset):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Determines if the offset exists in the array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td>The array index to check.</td>
    </tr>
</table>


<pre>public <strong>offsetGet</strong>(<a target="_blank" href="http://php.net/int">int</a> $offset):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the value of the given offset.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td>The array index.</td>
    </tr>
</table>


<pre>public <strong>offsetSet</strong>($offset, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets a value for the given offset.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$offset</td>
        <td>The array index or null to add the value to the end of the array.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>The value to add.</td>
    </tr>
</table>


<pre>public <strong>offsetUnset</strong>(<a target="_blank" href="http://php.net/int">int</a> $offset):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Unsets the value of the given offset.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td>The array index.</td>
    </tr>
</table>


<pre>public <strong>count</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>current</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>key</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
<pre>public <strong>next</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Move onto the next array index.
    
<pre>public <strong>rewind</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Reset the array index to the start of the array.
    
<pre>public <strong>valid</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### DecimalType<a name="market_types_decimaltype"></a>

The service for decimal type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### BooleanType<a name="market_types_booleantype"></a>

The service for boolean type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### DoubleType<a name="market_types_doubletype"></a>

The service for double type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### IntegerType<a name="market_types_integertype"></a>

The service for integer type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### URIType<a name="market_types_uritype"></a>

The service for uri type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>



### BaseType<a name="market_types_basetype"></a>

The service for base type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Can pass an associative array that will set the objects properties.</td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>



### StringType<a name="market_types_stringtype"></a>

The service for string type.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Types`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>xmlNamespaces</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>requestXmlRootElementNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Optional properties and values to assign to the object.</td>
    </tr>
</table>


<pre>public static <strong>getParentValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties, <a target="_blank" href="http://php.net/array">array</a> $values):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper function to remove the properties and values that belong to a object&#039;s parent.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>__get</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when getting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__set</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called when setting a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>Value assigned to the property.</td>
    </tr>
</table>


<pre>public <strong>__isset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
PHP magic function that is called to determine if a property is set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>__unset</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
PHP magic function that is called to unset a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The property name.</td>
    </tr>
</table>


<pre>public <strong>toRequestXml</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Converts the object to a XML request string.
    
<pre>public <strong>elementMeta</strong>(<a target="_blank" href="http://php.net/string">string</a> $elementName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the meta data for a property.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$elementName</td>
        <td>The element name.</td>
    </tr>
</table>


<pre>public <strong>attachment</strong>($data = null, <a target="_blank" href="http://php.net/string">string</a> $mimeType = &quot;application/octet-stream&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get or set the object&#039;s attachment. Overrides any existing attachment is setting.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>If a string it is assumed to be the contents of the attachment. If an array copy its values across.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mimeType</td>
        <td>The MIME type of the attachment that will be used in the request. Defaults to application/octet-stream.</td>
    </tr>
</table>


<pre>public <strong>hasAttachment</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Helper method to check if an object has an attachment.
    
<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Helper method that returns an associative array of the object&#039;s properties and values.
    
<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>A valid JMESPath expression</td>
    </tr>
</table>


<pre>public <strong>setValues</strong>(<a target="_blank" href="http://php.net/string">string</a> $class, <a target="_blank" href="http://php.net/array">array</a> $values = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign multiple values to an object.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$class</td>
        <td>The name of the class the properties belong to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td>Associative array of property names and their values.</td>
    </tr>
</table>


## Exceptions<a name="market_api_exceptions"></a>
### UnknownPropertyException<a name="market_exceptions_unknownpropertyexception"></a>

InvalidPropertyTypeException.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Exceptions`





#### Methods

<pre>public <strong>getMessage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getLine</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTrace</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getPrevious</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTraceAsString</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### InvalidEndPointException<a name="market_exceptions_invalidendpointexception"></a>

InvalidEndPointException.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Exceptions`





#### Methods

<pre>public <strong>getMessage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getLine</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTrace</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getPrevious</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTraceAsString</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### InvalidPropertyTypeException<a name="market_exceptions_invalidpropertytypeexception"></a>

InvalidPropertyTypeException.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Exceptions`





#### Methods

<pre>public <strong>getMessage</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCode</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getFile</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getLine</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTrace</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getPrevious</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getTraceAsString</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Services<a name="market_api_services"></a>
### BaseRestService<a name="market_services_baserestservice"></a>

The service for making eBay REST calls.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Services`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $config):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$config</td>
        <td>Configuration option values.</td>
    </tr>
</table>


<pre>public static <strong>getConfigDefinitions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns definitions for each configuration option that is supported.
    
<pre>public <strong>getConfig</strong>(<a target="_blank" href="http://php.net/string">string</a> $option = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get the service&#039;s configuration.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$option</td>
        <td>The name of the option whos value will be returned.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>callOperation</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a href="market#market_types_basetype">BaseType</a>
 $request = null):<a href="market#market_types_basetype">BaseType</a>
</pre>

    
Build API request and send.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The name of the operation.</td>
    </tr>
    <tr>
        <td><a href="market#market_types_basetype">BaseType</a>
</td>
        <td>$request</td>
        <td>Request object containing the request information.</td>
    </tr>
</table>


<pre>public <strong>getEbayHeaders</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Derived classes must implement this method that will build the needed eBay http headers.
    

### BaseWsdlService<a name="market_services_basewsdlservice"></a>

The service for making eBay WSDL calls.


#### Namespace

`Plenty\Modules\Market\Ebay\Api\Services`





#### Methods

<pre>public <strong>__construct</strong>(<a target="_blank" href="http://php.net/array">array</a> $config):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$config</td>
        <td>Configuration option values.</td>
    </tr>
</table>


<pre>public static <strong>getConfigDefinitions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns definitions for each configuration option that is supported.
    
<pre>public <strong>getConfig</strong>(<a target="_blank" href="http://php.net/string">string</a> $option = null, $default = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Method to get the service&#039;s configuration.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$option</td>
        <td>The name of the option whos value will be returned.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>callOperation</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a href="market#market_types_basetype">BaseType</a>
 $request, <a target="_blank" href="http://php.net/string">string</a> $responseClass):<a href="market#market_types_basetype">BaseType</a>
</pre>

    
Build API request and send.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The name of the operation.</td>
    </tr>
    <tr>
        <td><a href="market#market_types_basetype">BaseType</a>
</td>
        <td>$request</td>
        <td>Request object containing the request information.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$responseClass</td>
        <td>The name of the PHP class that will be created from the XML response.</td>
    </tr>
</table>


<pre>public <strong>getEbayHeaders</strong>(<a target="_blank" href="http://php.net/string">string</a> $operationName):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Derived classes must implement this method that will build the needed eBay http headers.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operationName</td>
        <td>The name of the operation been called.</td>
    </tr>
</table>


# ShopCategory<a name="market_shopcategory"></a>
    
## Contracts<a name="market_shopcategory_contracts"></a>
### ShopCategoryRepositoryContract<a name="market_contracts_shopcategoryrepositorycontract"></a>

The contract for the eBay shop categories.


#### Namespace

`Plenty\Modules\Market\Ebay\ShopCategory\Contracts`





#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $credentialsId, <a target="_blank" href="http://php.net/string">string</a> $viewType = &quot;list&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns a fitment by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$credentialsId</td>
        <td>The credentials ID for whom we want to load the eBay shop categories.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$viewType</td>
        <td>How should the eBay shop categories be returned. Possible values: 'list' or 'tree'. Default is 'list'.</td>
    </tr>
</table>


# PartsFitment<a name="market_partsfitment"></a>
    
## Contracts<a name="market_partsfitment_contracts"></a>
### FitmentRepositoryContract<a name="market_contracts_fitmentrepositorycontract"></a>

The contract for the fitment repository.


#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`





#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="market#market_models_fitment">Fitment</a>
</pre>

    
Returns a fitment by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be found.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Fitment instance. The relations available are 'items', 'items.properties'.</td>
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


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a fitment. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be deleted.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Search fitments
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the Fitment instance. The relations available are 'items', 'items.properties'.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that could be applied: 'id', 'categoryId', 'marketId', 'name', 'property', 'propertyName', 'propertyValue'.</td>
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


## Models<a name="market_partsfitment_models"></a>
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

    
Returns this model as an array.
    

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
            <td>A collection of this fitment item properties. Available names are 'Make', 'Model', 'Platform', 'Type', 'Production Period', 'Engine', 'FitmentComments', 'KType'.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

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

    
Returns this model as an array.
    
# ItemSpecific<a name="market_itemspecific"></a>
    
## Contracts<a name="market_itemspecific_contracts"></a>
### ItemSpecificRepositoryContract<a name="market_contracts_itemspecificrepositorycontract"></a>

The contract for the Ebay category repository.


#### Namespace

`Plenty\Modules\Market\Ebay\ItemSpecific\Contracts`





#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List item specifics.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that could be applied: 'categoryId', 'marketplaceId'.</td>
    </tr>
</table>


## Models<a name="market_itemspecific_models"></a>
### ItemSpecific<a name="market_models_itemspecific"></a>

The eBay item specific model.


#### Namespace

`Plenty\Modules\Market\Ebay\ItemSpecific\Models`




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
            <td>name</td>
            <td>A recommended Item Specific name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minValues</td>
            <td>Minimum number of values that you can specify for this Item Specific.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxValues</td>
            <td>Maximum number of values that you can specify for this Item Specific.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>selectionMode</td>
            <td>Controls whether you can specify your own name and value in listing requests, or if you need to use a name and/or value that eBay has defined.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueType</td>
            <td>The data type (e.g., date) that eBay expects the value to adhere to in listing requests. Only returned if the data type is not Text. In some cases, more details about the data type are returned in the `valueFormat` field.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueFormat</td>
            <td>The format of the data type (e.g., date format) that eBay expects the item specific's value to adhere to in listing requests. A data type identified by the `valueType` field may have different representations, and `valueFormat` specifies the precise format that is required.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>helpText</td>
            <td>Help-text defines the purpose of the Item Specific. The help text will be shown only when it is available for the particular Item Specific.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>helpUrl</td>
            <td>A page on the eBay Web site with context-specific help tips that provide useful information about this Item Specific. Only returned when an applicable page is available in the system.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationPicture</td>
            <td>Indicates whether the name (e.g., Color) can (or must) be used to classify the variation pictures</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationSpecifics</td>
            <td>Indicates whether the recommended name/value pair can be used as variation attributes in a fixed-price listing call. For example, a given category could disable a name like Brand in variation specifics (if Brand is only allowed in the item specifics at the Item level). The same category could enable a name like Size for variation specifics (in addition to recommending it for item specifics). If not returned, then the name/value can be used for both variation specifics and item specifics.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>values</td>
            <td>The available values.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Helper<a name="market_helper"></a>
    
## Contracts<a name="market_helper_contracts"></a>
### MarketAttributeHelperRepositoryContract<a name="market_contracts_marketattributehelperrepositorycontract"></a>

The contract for the market attribute helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`





#### Methods

<pre>public <strong>getAttributeName</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the attribute name for the given attribute id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeValueName</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the attribute value name for the given attribute value id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeNames</strong>(<a href="item#item_models_record">Record</a>
 $record, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/string">string</a> $delimiter = &quot;,&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns all attribute names for the given language as a string delimited by the given delimiter.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_record">Record</a>
</td>
        <td>$record</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeValueSetShortFrontendName</strong>(<a href="item#item_models_record">Record</a>
 $record, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/string">string</a> $delimiter = &quot;, &quot;, <a target="_blank" href="http://php.net/array">array</a> $attributeNameCombination = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the attribute value set short frontend name. Ex.: blue, XL
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_record">Record</a>
</td>
        <td>$record</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeNameCombination</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttributeNameAndValueCombination</strong>(<a target="_blank" href="http://php.net/string">string</a> $attributeNames, <a target="_blank" href="http://php.net/string">string</a> $attributeValues, <a target="_blank" href="http://php.net/string">string</a> $delimiter = &quot;,&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the combination of attribute names with their attribute values.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeNames</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$attributeValues</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$delimiter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getVariationNameAndAttributeNameAndValueCombination</strong>(<a href="item#item_models_record">Record</a>
 $record, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the name for a variation with all attribute names and attribute values. Ex.: T-Shirt (Size: L, Color: red)
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="item#item_models_record">Record</a>
</td>
        <td>$record</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>



### MarketPropertyHelperRepositoryContract<a name="market_contracts_marketpropertyhelperrepositorycontract"></a>

The contract for the market property helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`





#### Methods

<pre>public <strong>getMarketProperty</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrerId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns a list of the market properties
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td></td>
    </tr>
</table>



### MarketCategoryHelperRepositoryContract<a name="market_contracts_marketcategoryhelperrepositorycontract"></a>

The contract for the market category helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`





#### Methods

<pre>public <strong>getCategoryBranchName</strong>(<a target="_blank" href="http://php.net/int">int</a> $branchId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/string">string</a> $separator = &quot;&gt;&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the category bread crumbs as string for a given branchId, lang and plentyId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$branchId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$separator</td>
        <td>default</td>
    </tr>
</table>



### MarketItemHelperRepositoryContract<a name="market_contracts_marketitemhelperrepositorycontract"></a>

The contract for the item helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`





#### Methods

<pre>public <strong>getExternalManufacturerName</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the external manufacturer name.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>generateSku</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/float">float</a> $marketId, <a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/bool">bool</a> $setLastExportedTimestamp):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Generates or updates the sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$setLastExportedTimestamp</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $availabilityId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/bool">bool</a> $returnAvailabilityName):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the availability name or the availability average days
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$availabilityId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$returnAvailabilityName</td>
        <td></td>
    </tr>
</table>



### MarketAccountHelperRepositoryContract<a name="market_contracts_marketaccounthelperrepositorycontract"></a>

The contract for the market account helper repository.


#### Namespace

`Plenty\Modules\Market\Helper\Contracts`





#### Methods

<pre>public <strong>listMarketAccounts</strong>(<a target="_blank" href="http://php.net/float">float</a> $marketId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List market accounts
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
</table>


# Credentials<a name="market_credentials"></a>
    
## Contracts<a name="market_credentials_contracts"></a>
### CredentialsRepositoryContract<a name="market_contracts_credentialsrepositorycontract"></a>

The contract for the fitment repository.


#### Namespace

`Plenty\Modules\Market\Credentials\Contracts`





#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_credentials">Credentials</a>
</pre>

    
Get credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the credentials.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="market#market_models_credentials">Credentials</a>
</pre>

    
Create credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The credentials data. The properties that are required to update credentials can be found in the credentials model.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="market#market_models_credentials">Credentials</a>
</pre>

    
Update credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the credentials.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The credentials data. The properties that are required to update credentials can be found in the credentials model.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the credentials.</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Credentials can be filtered by ID, market, status, environment.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = \Plenty\Modules\Market\Credentials\Models\Credentials::MAX_ITEMS_PER_PAGE):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List credentials
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Credentials can be filtered by ID, market, status, environment.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>Current page of the response.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The requested amount of credentials per result page.</td>
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
    
## Models<a name="market_credentials_models"></a>
### Credentials<a name="market_models_credentials"></a>

The credentials model


#### Namespace

`Plenty\Modules\Market\Credentials\Models`




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
            <td>The ID of the credentials.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>environment</td>
            <td>The environment for the credentials. Possible values: sandbox, production</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>status</td>
            <td>The status of the credentials. Possible values: active, inactive, pending</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>data</td>
            <td>The data of the credentials.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>market</td>
            <td>The market for the current credentials.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the credentials was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the credentials was updated last.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
