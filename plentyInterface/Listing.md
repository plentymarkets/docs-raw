

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
        <td>The listing market ID the new lisitng market text belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language that should be updated.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The lisitng market text data as associative array.</td>
    </tr>
</table>


<pre>public <strong>updateOrCreate</strong>(<a target="_blank" href="http://php.net/int">int</a> $listingMarketId, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="listing#listing_models_listingmarkettext">ListingMarketText</a>
</pre>

    
Update or create listing market text
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$listingMarketId</td>
        <td>The lisitng market ID the new lisitng market text belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language that should be updated.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The lisitng market text data as associative array.</td>
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


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
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
            <td>The ID of the lisitng market text.</td>
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
    
