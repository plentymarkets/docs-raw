

# Seo<a name="webshop_seo"></a>
    
## Contracts<a name="webshop_seo_contracts"></a>
### RobotsRepositoryContract<a name="webshop_contracts_robotsrepositorycontract"></a>

Repository for robots.txt


#### Namespace

`Plenty\Modules\Webshop\Seo\Contracts`





#### Methods

<pre>public <strong>findByWebstoreId</strong>(<a target="_blank" href="http://php.net/int">int</a> $webstoreId):<a href="webshop#webshop_models_robots">Robots</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateByWebstoreId</strong>(<a target="_blank" href="http://php.net/int">int</a> $webstoreId, <a target="_blank" href="http://php.net/string">string</a> $data):<a href="webshop#webshop_models_robots">Robots</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### SitemapConfigurationRepositoryContract<a name="webshop_contracts_sitemapconfigurationrepositorycontract"></a>

Repository for sitemap configuration


#### Namespace

`Plenty\Modules\Webshop\Seo\Contracts`





#### Methods

<pre>public <strong>findByWebstoreId</strong>(<a target="_blank" href="http://php.net/int">int</a> $webstoreId):<a href="webshop#webshop_models_sitemapconfiguration">SitemapConfiguration</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateByWebstoreId</strong>(<a target="_blank" href="http://php.net/int">int</a> $webstoreId, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="webshop#webshop_models_sitemapconfiguration">SitemapConfiguration</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Models<a name="webshop_seo_models"></a>
### Robots<a name="webshop_models_robots"></a>

The robots model


#### Namespace

`Plenty\Modules\Webshop\Seo\Models`




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
            <td>value</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### SitemapConfiguration<a name="webshop_models_sitemapconfiguration"></a>

The sitemap configuration model


#### Namespace

`Plenty\Modules\Webshop\Seo\Models`




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
            <td>contentCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>item</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blog</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
