

# PartsFitment<a name="market_partsfitment"></a>
    
## Contracts<a name="market_partsfitment_contracts"></a>
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



### FitmentRepositoryContract<a name="market_contracts_fitmentrepositorycontract"></a>

The contract for the fitment repository.

#### Namespace

`Plenty\Modules\Market\Ebay\PartsFitment\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="market#market_models_fitment">Fitment</a>
</pre>
    
Returns a fitment by an ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be found.</td>
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


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Deletes a fitment. Returns `true` if the deletion was successful, otherwise `false`.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the fitment that should be deleted.</td>
    </tr>
</table>


<pre>public <strong>pushSortingOrder</strong>(<a target="_blank" href="http://php.net/string">string</a> $field, <a target="_blank" href="http://php.net/string">string</a> $direction = &quot;asc&quot;):<a href="miscellaneous#miscellaneous_repositories_contracts">Contracts</a>
</pre>
    
Pushes a sorting order to a collection.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$field</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$direction</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>applySortingOrder</strong>():<a href="miscellaneous#miscellaneous_repositories_contracts">Contracts</a>
</pre>
    
Applies the sorting order on the underlying builder instance
    
<pre>public <strong>clearSortingOrder</strong>():<a href="miscellaneous#miscellaneous_repositories_contracts">Contracts</a>
</pre>
    
Clears the sorting order on the underlying builder instance
    
## Models<a name="market_partsfitment_models"></a>
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
    
returns this model as an array
    

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
            <td>A collection of this fitment item properties.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

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
    
returns this model as an array
    
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


<pre>public <strong>generateSku</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/float">float</a> $marketId, <a target="_blank" href="http://php.net/int">int</a> $accountId, <a target="_blank" href="http://php.net/boolean">boolean</a> $setLastExportedTimestamp):<a target="_blank" href="http://php.net/string">string</a></pre>
    
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
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$setLastExportedTimestamp</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $availabilityId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/boolean">boolean</a> $returnAvailabilityName):<a target="_blank" href="http://php.net/string">string</a></pre>
    
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
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$returnAvailabilityName</td>
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


# Settings<a name="market_settings"></a>
    
## Contracts<a name="market_settings_contracts"></a>
### SettingsRepositoryContract<a name="market_contracts_settingsrepositorycontract"></a>

Use this interface to store and retrieve market specific settings.

#### Namespace

`Plenty\Modules\Market\Settings\Contracts`



#### Methods

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


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    
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
            <td>The id of the market settings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketplaceId</td>
            <td>The id of the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the current settings. Possible values are: attribute, property, category, shipping.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>settings</td>
            <td>The settings for the current marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>category</td>
            <td>The category that this settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>parcelServicePreset</td>
            <td>The parcel service preset that this settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attribute</td>
            <td>The attribute that this settings are related to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>propertyItem</td>
            <td>The property item that this settings are related to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
