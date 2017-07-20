

# Listing<a name="listing_listing"></a>
    
## Contracts<a name="listing_listing_contracts"></a>
### ListingRepositoryContract<a name="listing_contracts_listingrepositorycontract"></a>

The contract for the listing repository.


#### Namespace

`Plenty\Modules\Listing\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_listing">Listing</a>
</pre>

    
Get a listing by a given ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the listing instance, one of "markets", "type", "stockDependenceType", "properties".</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing
    
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
        <td>The relations to load in the ListingMarket instance. The relations available are 'type', 'stockDependenceType' and 'markets'.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that could be applied: 'id', 'itemId', 'typeId', 'stockDependenceTypeId', 'unitCombinationId'</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listing">Listing</a>
</pre>

    
Create new listing
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing data as associative array.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listing">Listing</a>
</pre>

    
Update listing
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing data as associative array.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete listing
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing.</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_listing_models"></a>
### Listing<a name="listing_models_listing"></a>

The listing model.


#### Namespace

`Plenty\Modules\Listing\Models`


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
            <td>The ID of the listing.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing type. Possible types are:
<ul>
    <li>1 = Auction</li>
    <li>2 = Fixed</li>
    <li>3 = Shop item</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockDependenceTypeId</td>
            <td>The ID of the listing stock dependence. Possible stock dependence types are:
<ul>
    <li>1 = Unlimited with sync</li>
    <li>2 = Limited with reservation</li>
    <li>3 = Limited without reservation</li>
    <li>4 = Unlimited without sync</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitCombinationId</td>
            <td>The ID of the unit combination.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td>The listing properties of the listing.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingtype">ListingType</a>
</td>
            <td>type</td>
            <td>The type of the listing.</td>
        </tr><tr>
            <td><a href="listing#listing_models_stockdependencetype">StockDependenceType</a>
</td>
            <td>stockDependenceType</td>
            <td>The stock dependence type of the listing.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingmarket">ListingMarket</a>
</td>
            <td>markets</td>
            <td>The listing markets of the listing</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingProperty<a name="listing_models_listingproperty"></a>

The listing properties model. Each listing property has a type.


#### Namespace

`Plenty\Modules\Listing\Models`


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
            <td>The ID of the listing property.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingId</td>
            <td>The ID of the listing that the property belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing property type. The following types are available:
<ul>
<li>10 = Use item price</li>
<li>11 = Number per lot</li>
<li>12 = Transmit item number type</li>
</ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>value</td>
            <td>The value of the listing property. The value depends on the type.</td>
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
            <td><a href="listing#listing_models_listing">Listing</a>
</td>
            <td>listing</td>
            <td>The listing that the property belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Date<a name="listing_date"></a>
    
## Models<a name="listing_date_models"></a>
### ListingDateType<a name="listing_models_listingdatetype"></a>

The listing date type model. Each listing date type can have multiple names.


#### Namespace

`Plenty\Modules\Listing\Date\Models`


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
            <td>The ID of the listing date type. The following date types are available:
<ul>
<li>1 = Last price update</li>
<li>2 = Last listing attempt</li>
<li>3 = Start time</li>
<li>4 = End time</li>
<li>5 = Last market update</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if this type can be deleted or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>The listing date type names.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingDateTypeName<a name="listing_models_listingdatetypename"></a>

The listing date type name model.


#### Namespace

`Plenty\Modules\Listing\Date\Models`


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
            <td>The ID of the listing date type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The listing date type ID that the current name belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>name</td>
            <td>The name of the listing date type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of the listing date type name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# LayoutTemplate<a name="listing_layouttemplate"></a>
    
## Contracts<a name="listing_layouttemplate_contracts"></a>
### LayoutTemplateRepositoryContract<a name="listing_contracts_layouttemplaterepositorycontract"></a>

The LayoutTemplateRepositoryContract is the interface for the layout template repository. This interface allows you to get a single layout template or lists of layout templates as well as to create, update or delete a layout tempalte.


#### Namespace

`Plenty\Modules\Listing\LayoutTemplate\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_layouttemplate">LayoutTemplate</a>
</pre>

    
Get a layout template.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the layout template.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the LayoutTemplate instance, one of "additional".</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_layouttemplate">LayoutTemplate</a>
</pre>

    
Create a layout template.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The layout template data.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete layout template
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the layout template.</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_layouttemplate_models"></a>
### LayoutTemplate<a name="listing_models_layouttemplate"></a>

The layout template model.


#### Namespace

`Plenty\Modules\Listing\LayoutTemplate\Models`


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
            <td>The ID of the layout template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the layout template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>css</td>
            <td>The css of the layout template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>htmlStructure</td>
            <td>The html structure of the layout template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>mainFrame</td>
            <td>The main frame of the layout template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>additionalContent</td>
            <td>The additional content of the layout template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>appendixType</td>
            <td>The appendix type of the layout template.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Market<a name="listing_market"></a>
    
## Contracts<a name="listing_market_contracts"></a>
### ListingMarketRepositoryContract<a name="listing_contracts_listingmarketrepositorycontract"></a>

The ListingMarketRepositoryContract is the interface for the listing market repository. This interface allows you to get a single listing market or lists of listing markets as well as to create a listing market.


#### Namespace

`Plenty\Modules\Listing\Market\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_listingmarket">ListingMarket</a>
</pre>

    
Get a listing market
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ListingMarket instance, one of "listing", "prices", "dates", "properties", "texts", "infos".</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing markets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ListingMarket instance, one of "listing", "prices", "dates", "properties", "texts", "infos".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that should be applied. The filters that could be applied: 'id', 'variationId', 'allVariations', 'referrerId', 'credentialsId', 'directoryId', 'verified', 'duration', 'listingId', 'itemId', 'listingTypeId', 'stockDependenceTypeId', 'status', 'stockCondition', 'shippingProfileId', .</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Create a listing
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market data.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listingmarket">ListingMarket</a>
</pre>

    
Update listing market
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market data as associative array.</td>
    </tr>
</table>


<pre>public <strong>start</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Start listing markets on the designated markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td>The IDs of the listing markets that need to be started.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>The parameters that should be considered during start. Available values are 'startTime', 'startDistribution'</td>
    </tr>
</table>


<pre>public <strong>verify</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Verifies listing markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td>The IDs of the listing markets that need to be verified.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a listing market
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market.</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_market_models"></a>
### ListingMarket<a name="listing_models_listingmarket"></a>

The listing market model.


#### Namespace

`Plenty\Modules\Listing\Market\Models`


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
            <td>The ID of the listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingId</td>
            <td>The listing ID of the current listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The variation ID for this listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td>The ID of the referrer.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>credentialsId</td>
            <td>The credentials ID that this listing market belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directoryId</td>
            <td>The directory ID of the listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>enabled</td>
            <td>Indicates if the listing market is enabled.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>duration</td>
            <td>The duration of the listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>verified</td>
            <td>Indicates if the listing market has been verified. Possible values are: 'succeeded', 'failed', 'unknown'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The quantity set for this listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>allVariations</td>
            <td>Indicates if all variations should be included.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the listing was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the listing was last updated.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listing">Listing</a>
</td>
            <td>listing</td>
            <td>The listing that the listing market belongs to.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td>The listing market properties of the listing market. The following properties are available:
<ul>
<li>1 = Shipping profile ID</li>
<li>2 = Order status</li>
<li>3 = Layout template ID</li>
<li>4 = Maximum number of images</li>
<li>5 = Warehouse ID</li>
<li>6 = Basic price in text</li>
<li>7 = Vat value</li>
<li>8 = Vat country ID</li>
<li>9 = Main language</li>
<li>10 = Use item price</li>
<li>11 = Number per lot</li>
<li>12 = Transmit item number type</li>
<li>100 = eBay parts fitment ID</li>
<li>101 = eBay maximum online listings</li>
<li>102 = eBay first platform category ID</li>
<li>103 = eBay second platform category ID</li>
<li>104 = eBay first shop category ID</li>
<li>105 = eBay second shop category ID</li>
<li>106 = eBay private auction</li>
<li>107 = eBay gallery type</li>
<li>108 = eBay gallery duration</li>
<li>109 = eBay transmit MPR</li>
<li>110 = eBay counter type</li>
<li>111 = eBay condition ID</li>
<li>112 = eBay condition description</li>
<li>113 = eBay enhancements</li>
<li>114 = eBay best offer</li>
<li>115 = eBay best offer decline price</li>
<li>116 = eBay best offer accept price</li>
<li>117 = eBay is eBayPlus</li>
<li>118 = eBay is Click & Collect</li>
<li>200 = Hood first platform category</li>
<li>201 = Hood second platform category</li>
<li>202 = Hood first shop category</li>
<li>203 = Hood second shop category</li>
<li>204 = Hood third shop category</li>
<li>205 = Hood payment methods</li>
<li>206 = Hood enhancements</li>
<li>207 = Hood show on shop startpage</li>
<li>208 = Hood shipping discount</li>
<li>209 = Hood delivery days on stock from</li>
<li>210 = Hood delivery days on stock to</li>
<li>211 = Hood delivery days not on stock from</li>
<li>212 = Hood delivery days not on stock to</li>
<li>300 = Ricardo first platform category ID</li>
<li>301 = Ricardo warranty ID</li>
<li>302 = Ricardo delivery ID</li>
<li>303 = Ricardo availability ID</li>
<li>304 = Ricardo delivery cost</li>
<li>305 = Ricardo payment ID</li>
<li>306 = Ricardo price increment</li>
<li>307 = Ricardo payment methods</li>
<li>308 = Ricardo enhancements</li>
<li>309 = Ricardo item condition ID</li>
<li>310 = Ricardo max relist count</li>
<li>311 = Ricardo is cumulative shipping</li>
<li>312 = Ricardo delivery package size ID</li>
<li>313 = Ricardo use secondary language</li>
<li>314 = Ricardo template ID</li>
<li>315 = Ricardo is relist sold out</li>
</ul></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>itemSpecifics</td>
            <td>The listing market item specifics of the listing market.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>prices</td>
            <td>The listing market prices of the listing market.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dates</td>
            <td>The listing market dates of the listing market.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>texts</td>
            <td>The listing market texts of the listing market.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketDate<a name="listing_models_listingmarketdate"></a>

The listing market dates model. Each listing market date has a type.


#### Namespace

`Plenty\Modules\Listing\Market\Models`


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
            <td>The ID of the listing market date.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The ID of the listing market that the date belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing market date type. The following types are available:
<ul>
<li>1 = Last price update</li>
<li>2 = Last listing attempt</li>
<li>3 = Start time</li>
<li>4 = End time</li>
<li>5 = Last market update</li>
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
            <td>The date that the date was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the date was last updated.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingmarket">ListingMarket</a>
</td>
            <td>listingMarket</td>
            <td>The listing market that the date belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketItemSpecific<a name="listing_models_listingmarketitemspecific"></a>

The listing market item specific model.


#### Namespace

`Plenty\Modules\Listing\Market\Models`


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
            <td>The ID of the listing market item specific.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The ID of the listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the listing market item specific.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>value</td>
            <td>The value of the listing market item specific.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketPrice<a name="listing_models_listingmarketprice"></a>

The listing market price model.


#### Namespace

`Plenty\Modules\Listing\Market\Models`


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
            <td>The ID of the listing price.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The ID of the listing market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing price type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The value of the listing market price.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>listingMarket</td>
            <td>The listing market.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>type</td>
            <td>The listing price type.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketProperty<a name="listing_models_listingmarketproperty"></a>

The listing market properties model. Each listing market property has a type.


#### Namespace

`Plenty\Modules\Listing\Market\Models`


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
            <td>The ID of the listing market property.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The ID of the listing market that the property belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing market property type. The following types are available:
<ul>
<li>1 = Shipping profile ID</li>
<li>2 = Order status</li>
<li>3 = Layout template ID</li>
<li>4 = Maximum number of images</li>
<li>5 = Warehouse ID</li>
<li>6 = Basic price in text</li>
<li>7 = Vat value</li>
<li>8 = Vat country ID</li>
<li>9 = Main language</li>
<li>10 = Use item price</li>
<li>11 = Number per lot</li>
<li>12 = Transmit item number type</li>
<li>100 = eBay parts fitment ID</li>
<li>101 = eBay maximum online listings</li>
<li>102 = eBay first platform category ID</li>
<li>103 = eBay second platform category ID</li>
<li>104 = eBay first shop category ID</li>
<li>105 = eBay second shop category ID</li>
<li>106 = eBay private auction</li>
<li>107 = eBay gallery type</li>
<li>108 = eBay gallery duration</li>
<li>109 = eBay transmit MPR</li>
<li>110 = eBay counter type</li>
<li>111 = eBay condition ID</li>
<li>112 = eBay condition description</li>
<li>113 = eBay enhancements</li>
<li>114 = eBay best offer</li>
<li>115 = eBay best offer decline price</li>
<li>116 = eBay best offer accept price</li>
<li>117 = eBay is eBayPlus</li>
<li>118 = eBay is Click & Collect</li>
<li>200 = Hood first platform category</li>
<li>201 = Hood second platform category</li>
<li>202 = Hood first shop category</li>
<li>203 = Hood second shop category</li>
<li>204 = Hood third shop category</li>
<li>205 = Hood payment methods</li>
<li>206 = Hood enhancements</li>
<li>207 = Hood show on shop startpage</li>
<li>208 = Hood shipping discount</li>
<li>209 = Hood delivery days on stock from</li>
<li>210 = Hood delivery days on stock to</li>
<li>211 = Hood delivery days not on stock from</li>
<li>212 = Hood delivery days not on stock to</li>
<li>300 = Ricardo first platform category ID</li>
<li>301 = Ricardo warranty ID</li>
<li>302 = Ricardo delivery ID</li>
<li>303 = Ricardo availability ID</li>
<li>304 = Ricardo delivery cost</li>
<li>305 = Ricardo payment ID</li>
<li>306 = Ricardo price increment</li>
<li>307 = Ricardo payment methods</li>
<li>308 = Ricardo enhancements</li>
<li>309 = Ricardo item condition ID</li>
<li>310 = Ricardo max relist count</li>
<li>311 = Ricardo is cumulative shipping</li>
<li>312 = Ricardo delivery package size ID</li>
<li>313 = Ricardo use secondary language</li>
<li>314 = Ricardo template ID</li>
<li>315 = Ricardo is relist sold out</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the listing market property. The value depends on the type.</td>
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
            <td><a href="listing#listing_models_listingmarket">ListingMarket</a>
</td>
            <td>listingMarket</td>
            <td>The listing market that the property belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Directory<a name="listing_directory"></a>
    
## Contracts<a name="listing_directory_contracts"></a>
### ListingMarketDirectoryRepositoryContract<a name="listing_contracts_listingmarketdirectoryrepositorycontract"></a>

The contract for the listing market directory repository.


#### Namespace

`Plenty\Modules\Listing\Market\Directory\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="listing#listing_models_listingmarketdirectory">ListingMarketDirectory</a>
</pre>

    
Get a listing market directory
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market directory.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Create a listing market directory.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market directory data as associative array.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listingmarketdirectory">ListingMarketDirectory</a>
</pre>

    
Update listing market directory
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market directory.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market directory data as associative array.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a listing market directory
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market directory.</td>
    </tr>
</table>


## Models<a name="listing_directory_models"></a>
### ListingMarketDirectory<a name="listing_models_listingmarketdirectory"></a>

The listing market directory model.


#### Namespace

`Plenty\Modules\Listing\Market\Directory\Models`


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
            <td>The ID of the listing market directory.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the listing market directory.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentId</td>
            <td>The parent ID of the listing market directory.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>level</td>
            <td>The level of the directory.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# History<a name="listing_history"></a>
    
## Contracts<a name="listing_history_contracts"></a>
### ListingMarketHistoryRepositoryContract<a name="listing_contracts_listingmarkethistoryrepositorycontract"></a>

The ListingMarketHistoryRepositoryContract is the interface for the listing market history repository. This interface allows you to get a single listing market history or to list several listing market histories.


#### Namespace

`Plenty\Modules\Listing\Market\History\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_listingmarkethistory">ListingMarketHistory</a>
</pre>

    
Get a listing market.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ListingMarket instance, one of "listing", "prices", "dates", "properties", "texts".</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing market histories
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ListingMarketHistory instance, one of "listingMarket", "dates", "properties", "texts".</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that should be applied. The filters that are available: 'listingMarketId', 'variationId', 'allVariations', 'referrerId', 'credentialsId', 'verified', 'duration', 'listingId', 'itemId', 'listingTypeId', 'stockDependenceTypeId', 'status', 'stockCondition' .</td>
    </tr>
</table>


<pre>public <strong>end</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
End the listing market histories on the designated markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td>The IDs of the listing market histories that need to be started.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>The parameters that should be considers during end. Available values are 'deleteOnSuccess'</td>
    </tr>
</table>


<pre>public <strong>relist</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Relist the listing market histories on the designated markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td>The IDs of the listing market histories that need to be started.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids, <a target="_blank" href="http://php.net/array">array</a> $options = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Update the listing market histories on the designated markets.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td>The IDs of the listing market histories that need to be updated.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$options</td>
        <td>The update options that should be considers during update. Available values are:
<ul>
<li>title - Updates the title
<li>subtitle - Updates the subtitle</li></li>
<li>itemSpecifics - Updates the item specifics</li>
<li>category - Updates the platform and shop category</li>
<li>productListingDetails - Updates the product data for the listing</li>
<li>listingEnhancements - Updates the enhancements information</li>
<li>duration - Updates the duration</li>
<li>shipping - Updates the shipping information</li>
<li>description - Updates the description</li>
<li>pictures - Updates the entry pictures</li>
<li>quantityPriceAndVariations - Updates the quantity and price (also for variations)</li>
<li>resetVariations - Reset the variations. The variation from the item are transmitted again</li>
<li>partsFitment - Updates the parts fitment information (only available for eBay)</li>
<li>loyaltyProgram - Updates the listing loyalty program information (only available for eBay Plus) </li>
<li>resetRrp - Reset the recommended retail price information</li>
<li>payment - Updates payment information (only available for Hood)</li>
</ul></td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_history_models"></a>
### ListingMarketHistory<a name="listing_models_listingmarkethistory"></a>

The listing market history model.


#### Namespace

`Plenty\Modules\Listing\Market\History\Models`


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
            <td>The listing market history ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The listing market ID of the current listing market history.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td>The referrer ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td>The external ID of the listing market history.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusId</td>
            <td>The status ID of the current listing market history. The following properties are available:
<ul>
<li>1 = Active</li>
<li>2 = Ended</li>
<li>3 = Relisted</li>
<li>4 = Hidden</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The quantity available for sale on the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantitySold</td>
            <td>The quantity sold currently on the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantitySoldDelta</td>
            <td>The difference between the sold quantity and orders imported for this listing market history.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantityRemain</td>
            <td>The quantity remaining on the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td>The price offered for this listing market. @see ListingMarketHistoryVariation if the listing market history contains variations.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sku</td>
            <td>The stock keeping unit of this listing market history.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the entry was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the entry was updated last.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingmarket">ListingMarket</a>
</td>
            <td>listingMarket</td>
            <td>The listing market that the listing market history belongs to.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>variations</td>
            <td>The listing market history variations that belong to this listing market history.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>properties</td>
            <td>The listing market history properties of the listing market.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dates</td>
            <td>The listing market history dates of the listing market history.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>texts</td>
            <td>The listing market history texts of the listing market history.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>status</td>
            <td>The listing market history status of the listing market history.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketHistoryDate<a name="listing_models_listingmarkethistorydate"></a>

The listing market history dates model. Each listing market history date has a type.


#### Namespace

`Plenty\Modules\Listing\Market\History\Models`


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
            <td>The ID of the listing market history date.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>historyId</td>
            <td>The ID of the listing market history that the date belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing date type. The following types are available:
<ul>
<li>Start time = 3</li>
<li>End time = 4</li>
<li>Start time = 3</li>
<li>End time = 4</li>
<li>Last market update = 5</li>
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
            <td>The date that the date was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the date was last updated.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingmarket">ListingMarket</a>
</td>
            <td>listingMarket</td>
            <td>The listing market that the date belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketHistoryProperty<a name="listing_models_listingmarkethistoryproperty"></a>

The listing market properties model. Each listing market property has a type.


#### Namespace

`Plenty\Modules\Listing\Market\History\Models`


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
            <td>The ID of the listing market history property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>historyId</td>
            <td>The ID of the listing market history that the property belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing market history property type. The following types are available:
<ul>
<li>Relisted external ID = 13</li>
<li>SCO Offer = 14</li>
<li>Promotion = 15</li>
<li>Unique user ID = 16</li>
<li>Update error = 17</li>
<li>Has variations = 18</li>
<li>End now = 19</li>
<li>Insert by type = 20</li>
<li>Is eBayPlus = 117</li>
<li>Is click & collect = 118</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the listing market history property. The value depends on the type.</td>
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
            <td><a href="listing#listing_models_listingmarkethistory">ListingMarketHistory</a>
</td>
            <td>history</td>
            <td>The listing market history that the property belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketHistoryText<a name="listing_models_listingmarkethistorytext"></a>

The listing market history text model.


#### Namespace

`Plenty\Modules\Listing\Market\History\Models`


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
            <td>The ID of the listing market history text.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>historyId</td>
            <td>The ID of the listing market history the text belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the listing market text. Available values: 'de', 'en', 'fr', 'it', 'es', 'tr', 'nl', 'pl', 'nn', 'da', 'se', 'cz', 'ru', 'sk', 'cn', 'vn', 'pt', 'bg', 'ro'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the listing market text.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingMarketHistoryVariation<a name="listing_models_listingmarkethistoryvariation"></a>

The listing market history model.


#### Namespace

`Plenty\Modules\Listing\Market\History\Models`


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
            <td>The listing market history variation ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>historyId</td>
            <td>The listing market history ID of the current listing market history variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The variation ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>attributeName</td>
            <td>The attribute name. This is an serialized array of the attribute-value data.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sku</td>
            <td>The stock keeping unit of this listing market history variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td>The quantity available for sale on the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantitySold</td>
            <td>The quantity sold currently on the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantitySoldDelta</td>
            <td>The difference between the sold quantity and orders imported for this listing market history variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantityRemain</td>
            <td>The quantity remaining on the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td>The price offered for this listing market history variation.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the entry was created.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date that the entry was updated last.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingmarkethistory">ListingMarketHistory</a>
</td>
            <td>history</td>
            <td>The listing market history variations that belong to this listing market history.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Info<a name="listing_info"></a>
    
## Contracts<a name="listing_info_contracts"></a>
### ListingMarketInfoRepositoryContract<a name="listing_contracts_listingmarketinforepositorycontract"></a>

The ListingMarketInfoRepositoryContract is the interface for the listing market info repository. This interface allows you to get information about one or many listing markets.


#### Namespace

`Plenty\Modules\Listing\Market\Info\Contracts`



#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing market infos by filter options
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ListingMarketInfo instance.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that should be applied. The filters that could be applied: 'id', 'listingMarketId', 'type', 'createdAtFrom', 'createdAtTo', 'code'.</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_info_models"></a>
### ListingMarketInfo<a name="listing_models_listingmarketinfo"></a>

The listing market info model.


#### Namespace

`Plenty\Modules\Listing\Market\Info\Models`


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
            <td>The listing market info ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The listing market ID that the current information belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The information type. Possible values: 'warning', 'error', 'info'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>code</td>
            <td>The information code.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>message</td>
            <td>The information message.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date that the listing market info was created.</td>
        </tr><tr>
            <td><a href="listing#listing_models_listingmarket">ListingMarket</a>
</td>
            <td>listingMarket</td>
            <td>The listing market that the listing market info belongs to.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Text<a name="listing_text"></a>
    
## Contracts<a name="listing_text_contracts"></a>
### ListingMarketTextRepositoryContract<a name="listing_contracts_listingmarkettextrepositorycontract"></a>

The contract for the listing market text repository.


#### Namespace

`Plenty\Modules\Listing\Market\Text\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="listing#listing_models_listingmarkettext">ListingMarketText</a>
</pre>

    
Get a listing market text
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market text.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/int">int</a> $listingMarketId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listingmarkettext">ListingMarketText</a>
</pre>

    
Create new listing market text
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$listingMarketId</td>
        <td>The listing market ID the new market listing text belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market text data as associative array.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $listingMarketId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listingmarkettext">ListingMarketText</a>
</pre>

    
Update listing market text
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$listingMarketId</td>
        <td>The listing market ID the new listing market text belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language that should be updated.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market text data as associative array.</td>
    </tr>
</table>


<pre>public <strong>updateOrCreate</strong>(<a target="_blank" href="http://php.net/int">int</a> $listingMarketId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listingmarkettext">ListingMarketText</a>
</pre>

    
Update or create listing market text
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$listingMarketId</td>
        <td>The listing market ID the new listing market text belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language that should be updated.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The listing market text data as associative array.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete listing market text
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing market text.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing market text
    
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
        <td>The filters that should be applied: 'id', 'language', 'contains'</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_text_models"></a>
### ListingMarketText<a name="listing_models_listingmarkettext"></a>

The listing market text model.


#### Namespace

`Plenty\Modules\Listing\Market\Text\Models`


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
            <td>The ID of the listing market text.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>listingMarketId</td>
            <td>The ID of the listing market the text belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the listing market text. Available values: 'de', 'en', 'fr', 'it', 'es', 'tr', 'nl', 'pl', 'nn', 'da', 'se', 'cz', 'ru', 'sk', 'cn', 'vn', 'pt', 'bg', 'ro'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the listing market text.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>subtitle</td>
            <td>The subtitle of the listing market text.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the listing market text.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# OptionTemplate<a name="listing_optiontemplate"></a>
    
## Contracts<a name="listing_optiontemplate_contracts"></a>
### OptionTemplateRepositoryContract<a name="listing_contracts_optiontemplaterepositorycontract"></a>

The contract for the listing option template repository.


#### Namespace

`Plenty\Modules\Listing\OptionTemplate\Contracts`



#### Methods

<pre>public <strong>preview</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get a preview list of all listing option templates
    
<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="listing#listing_models_optiontemplate">OptionTemplate</a>
</pre>

    
Get option template
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the option template.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_optiontemplate">OptionTemplate</a>
</pre>

    
Create option template
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The option template data as associative array.</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update option template
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the option template.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The option template data as associative array.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete option template
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the option template.</td>
    </tr>
</table>


## Models<a name="listing_optiontemplate_models"></a>
### OptionTemplate<a name="listing_models_optiontemplate"></a>

The option template model.


#### Namespace

`Plenty\Modules\Listing\OptionTemplate\Models`


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
            <td>The ID of the option template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the option template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>listing</td>
            <td>The listing options of the option template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>listingMarket</td>
            <td>The listing market options of the option template.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketOptions</td>
            <td>The market options of the option template.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Price<a name="listing_price"></a>
    
## Models<a name="listing_price_models"></a>
### ListingPriceType<a name="listing_models_listingpricetype"></a>

The listing price type model.


#### Namespace

`Plenty\Modules\Listing\Price\Models`


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
            <td>The ID of the listing price type. The following date types are available:
<ul>
<li>1 = Start price</li>
<li>2 = Fixed price</li>
<li>3 = Reserved price</li>
<li>4 = SCO minimum price</li>
<li>5 = Market fee</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that states if this type can be deleted or not.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The listing price type names.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingPriceTypeName<a name="listing_models_listingpricetypename"></a>

The listing price type name model.


#### Namespace

`Plenty\Modules\Listing\Price\Models`


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
            <td>The ID of the listing price type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing price type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>name</td>
            <td>The name of the listing price type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of the listing price type name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Property<a name="listing_property"></a>
    
## Models<a name="listing_property_models"></a>
### ListingPropertyType<a name="listing_models_listingpropertytype"></a>

The listing properties model. Each listing property has a type.


#### Namespace

`Plenty\Modules\Listing\Property\Models`


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
            <td>The ID of the listing property. The following types are available:
<ul>
<li>1 = Shipping profile ID</li>
<li>2 = Order status</li>
<li>3 = Layout template ID</li>
<li>4 = Maximum number of images</li>
<li>5 = Warehouse ID</li>
<li>6 = Basic price in text</li>
<li>7 = Vat value</li>
<li>8 = Vat country ID</li>
<li>9 = Main language</li>
<li>10 = Use item price</li>
<li>11 = Number per lot</li>
<li>12 = Transmit item number type</li>
<li>100 = eBay parts fitment ID</li>
<li>101 = eBay maximum online listings</li>
<li>102 = eBay first platform category ID</li>
<li>103 = eBay second platform category ID</li>
<li>104 = eBay first shop category ID</li>
<li>105 = eBay second shop category ID</li>
<li>106 = eBay private auction</li>
<li>107 = eBay gallery type</li>
<li>108 = eBay gallery duration</li>
<li>109 = eBay transmit MPR</li>
<li>110 = eBay counter type</li>
<li>111 = eBay condition ID</li>
<li>112 = eBay condition description</li>
<li>113 = eBay enhancements</li>
<li>114 = eBay best offer</li>
<li>115 = eBay best offer decline price</li>
<li>116 = eBay best offer accept price</li>
<li>117 = eBay is eBayPlus</li>
<li>118 = eBay is Click & Collect</li>
<li>200 = Hood first platform category</li>
<li>201 = Hood second platform category</li>
<li>202 = Hood first shop category</li>
<li>203 = Hood second shop category</li>
<li>204 = Hood third shop category</li>
<li>205 = Hood payment methods</li>
<li>206 = Hood enhancements</li>
<li>207 = Hood show on shop startpage</li>
<li>208 = Hood shipping discount</li>
<li>209 = Hood delivery days on stock from</li>
<li>210 = Hood delivery days on stock to</li>
<li>211 = Hood delivery days not on stock from</li>
<li>212 = Hood delivery days not on stock to</li>
<li>300 = Ricardo first platform category ID</li>
<li>301 = Ricardo warranty ID</li>
<li>302 = Ricardo delivery ID</li>
<li>303 = Ricardo availability ID</li>
<li>304 = Ricardo delivery cost</li>
<li>305 = Ricardo payment ID</li>
<li>306 = Ricardo price increment</li>
<li>307 = Ricardo payment methods</li>
<li>308 = Ricardo enhancements</li>
<li>309 = Ricardo item condition ID</li>
<li>310 = Ricardo max relist count</li>
<li>311 = Ricardo is cumulative shipping</li>
<li>312 = Ricardo delivery package size ID</li>
<li>313 = Ricardo use secondary language</li>
<li>314 = Ricardo template ID</li>
<li>315 = Ricardo is relist sold out</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if this type can be deleted or not.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingPropertyTypeName<a name="listing_models_listingpropertytypename"></a>

The listing property type name model.


#### Namespace

`Plenty\Modules\Listing\Property\Models`


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
            <td>The ID of the listing property type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing property type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>name</td>
            <td>The name of the listing property type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of the listing property type name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# ShippingProfile<a name="listing_shippingprofile"></a>
    
## Contracts<a name="listing_shippingprofile_contracts"></a>
### ShippingProfileRepositoryContract<a name="listing_contracts_shippingprofilerepositorycontract"></a>

The ShippingProfileRepositoryContract is the interface for the listing shipping profile repository. This interface allows you to get a shipping profile.


#### Namespace

`Plenty\Modules\Listing\ShippingProfile\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_shippingprofile">ShippingProfile</a>
</pre>

    
Get a shipping profile
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the shipping profile.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ShippingProfile instance.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Search shipping profiles
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of entries to be displayed per page. The default number of entries per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the ShippingProfile instance.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters that should be applied. The filters that could be applied: 'id', 'referrerId', 'credentialsId'.</td>
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
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="listing_shippingprofile_models"></a>
### ShippingProfile<a name="listing_models_shippingprofile"></a>

The listing shipping profile model.


#### Namespace

`Plenty\Modules\Listing\ShippingProfile\Models`


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
            <td>The listing shipping profile ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The listing shipping profile name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>credentialsId</td>
            <td>The credentials ID that this listing shipping profile belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerId</td>
            <td>The referrer ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdBy</td>
            <td>Who created the shipping profile. Possible values: 'migration','customer','external'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isDefault</td>
            <td>Tells if the current listing shipping profile is set as default.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Status<a name="listing_status"></a>
    
## Models<a name="listing_status_models"></a>
### ListingStatus<a name="listing_models_listingstatus"></a>

The listing status model.


#### Namespace

`Plenty\Modules\Listing\Status\Models`


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
            <td>The ID of the listing status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if the status can be deleted.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The listing status names.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingStatusName<a name="listing_models_listingstatusname"></a>

The listing status name model.


#### Namespace

`Plenty\Modules\Listing\Status\Models`


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
            <td>The ID of the listing status name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusId</td>
            <td>The ID of the listing status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the listing status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the listing status name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# StockDependenceType<a name="listing_stockdependencetype"></a>
    
## Contracts<a name="listing_stockdependencetype_contracts"></a>
### StockDependenceTypeRepositoryContract<a name="listing_contracts_stockdependencetyperepositorycontract"></a>

The contract for the listing stock dependence type repository.


#### Namespace

`Plenty\Modules\Listing\StockDependenceType\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_stockdependencetype">StockDependenceType</a>
</pre>

    
Get a listing stock dependence type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing stock dependence type.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the StockDependenceType instance, available values are: "names".</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing stock dependence types
    
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
        <td>The relations to load in the ListingMarket instance. The relations available are 'names'.</td>
    </tr>
</table>


## Models<a name="listing_stockdependencetype_models"></a>
### StockDependenceType<a name="listing_models_stockdependencetype"></a>

The listing stock dependence type model.


#### Namespace

`Plenty\Modules\Listing\StockDependenceType\Models`


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
            <td>The ID of the listing stock dependence type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if the type can be deleted.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The listing stock dependence type names.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### StockDependenceTypeName<a name="listing_models_stockdependencetypename"></a>

The listing stock dependence type name model.


#### Namespace

`Plenty\Modules\Listing\StockDependenceType\Models`


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
            <td>The ID of the listing stock dependence type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing stock type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the listing stock dependence type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the listing stock dependence type name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Type<a name="listing_type"></a>
    
## Contracts<a name="listing_type_contracts"></a>
### ListingTypeRepositoryContract<a name="listing_contracts_listingtyperepositorycontract"></a>

The contract for the listing type repository.


#### Namespace

`Plenty\Modules\Listing\Type\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="listing#listing_models_listingtype">ListingType</a>
</pre>

    
Get a listing type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the listing type.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to load in the type instance, available values are: "names".</td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List listing types
    
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
        <td>The relations to load in the ListingMarket instance. The relations available are 'names'.</td>
    </tr>
</table>


## Models<a name="listing_type_models"></a>
### ListingType<a name="listing_models_listingtype"></a>

The listing type model.


#### Namespace

`Plenty\Modules\Listing\Type\Models`


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
            <td>The ID of the listing type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isErasable</td>
            <td>Flag that indicates if the type can be deleted.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position for sorting.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>names</td>
            <td>The listing type names.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ListingTypeName<a name="listing_models_listingtypename"></a>

The listing type name model.


#### Namespace

`Plenty\Modules\Listing\Type\Models`


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
            <td>The ID of the listing type name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The ID of the listing type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the listing type.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the listing type name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
