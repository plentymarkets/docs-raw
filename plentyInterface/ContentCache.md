

# ContentCache<a name="contentcache_contentcache"></a>
    
## Contracts<a name="contentcache_contentcache_contracts"></a>
### ContentCacheRepositoryContract<a name="contentcache_contracts_contentcacherepositorycontract"></a>

Save and retrieve values to or from the content cache


#### Namespace

`Plenty\Modules\ContentCache\Contracts`





#### Methods

<pre>public <strong>enableCacheForResponse</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Enable content caching for current response so next request on this resource will be delivered from content cache.
    
<pre>public <strong>linkVariationsToResponse</strong>(<a target="_blank" href="http://php.net/array">array</a> $variationIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Link variations to current response.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$variationIds</td>
        <td>Ids of variations referenced by the current response.</td>
    </tr>
</table>



### ContentCacheInvalidationRepositoryContract<a name="contentcache_contracts_contentcacheinvalidationrepositorycontract"></a>

Interface for content cache invalidation


#### Namespace

`Plenty\Modules\ContentCache\Contracts`





#### Methods

<pre>public <strong>invalidateVariationIds</strong>(<a target="_blank" href="http://php.net/array">array</a> $variationIds, <a target="_blank" href="http://php.net/int">int</a> $plentyId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Invalidate all cache entries related to given variation ids.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$variationIds</td>
        <td>Ids of the variation to invalidate cache entries for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>invalidateAll</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Invalidate all cache entries related to given plenty id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>invalidateUri</strong>(<a target="_blank" href="http://php.net/string">string</a> $uri):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Invalidate cache entries by URI
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uri</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>storeInvalidationStacks</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
# ContentCacheLink<a name="contentcache_contentcachelink"></a>
    
## Models<a name="contentcache_contentcachelink_models"></a>
### ContentCacheLink<a name="contentcache_models_contentcachelink"></a>

Eloquent model representing a Content Cache Link.


#### Namespace

`Plenty\Modules\ContentCache\ContentCacheLink\Models`




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
            <td>plentyId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>linkType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>cacheKey</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>linkId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
