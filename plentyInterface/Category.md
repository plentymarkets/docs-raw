

# Category<a name="category_category"></a>
    
## Contracts<a name="category_category_contracts"></a>
### CategoryBranchMarketplaceRepositoryContract<a name="category_contracts_categorybranchmarketplacerepositorycontract"></a>

Repository for CategoryBranchMarketplace


#### Namespace

`Plenty\Modules\Category\Contracts`



#### Methods

<pre>public <strong>findCategoryBranchMarketplace</strong>(<a target="_blank" href="http://php.net/int">int</a> $branchId, <a target="_blank" href="http://php.net/int">int</a> $webstoreId, <a target="_blank" href="http://php.net/int">int</a> $marketplaceId, <a target="_blank" href="http://php.net/float">float</a> $marketplaceSubId = 0.0):<a href="category#category_models_categorybranchmarketplace">CategoryBranchMarketplace</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$branchId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketplaceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketplaceSubId</td>
        <td></td>
    </tr>
</table>



### CategoryBranchRepositoryContract<a name="category_contracts_categorybranchrepositorycontract"></a>

Repository Contract for CategoryBranch


#### Namespace

`Plenty\Modules\Category\Contracts`



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="category#category_models_categorybranch">CategoryBranch</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_contracts_paginationresponsecontract">PaginationResponseContract</a>
</pre>

    
Get category trees
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Filters restrict the list of results. Results can be filtered by the following parameters: 'type' - the category type. Available values: item, container, content, blog</td>
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
    

### CategoryRepositoryContract<a name="category_contracts_categoryrepositorycontract"></a>

Repository for categories


#### Namespace

`Plenty\Modules\Category\Contracts`



#### Methods

<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;):<a href="category#category_models_category">Category</a>
</pre>

    
Returns one category by id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The id of the category.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>Optional language of details.</td>
    </tr>
</table>


<pre>public <strong>getLinklistTree</strong>(<a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/string">string</a> $lang, <a target="_blank" href="http://php.net/int">int</a> $clientId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns all linklist categories as tree.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>'all','item','container','content' or 'blog'</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>Optional language of details.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The unique ID of the client (store)</td>
    </tr>
</table>


<pre>public <strong>getLinklistList</strong>(<a target="_blank" href="http://php.net/string">string</a> $type = &quot;all&quot;, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/int">int</a> $clientId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns all linklist categories as list.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>'all','item','container','content' or 'blog'</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>Optional language of details.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The unique ID of the client (store)</td>
    </tr>
</table>


<pre>public <strong>hasChildren</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/bool">bool</a> $onlySiteMapped = false, <a target="_blank" href="http://php.net/bool">bool</a> $onlyLinkListed = false):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Returns true if category has children.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The id of the category.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$onlySiteMapped</td>
        <td>Determines if the result has only sitemaps or all visible categories.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$onlyLinkListed</td>
        <td>Determines if the result has only linklists or all visible categories.</td>
    </tr>
</table>


<pre>public <strong>getChildren</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Returns children of the category.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The id of the category.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>Optional language of details.</td>
    </tr>
</table>


<pre>public <strong>getUrl</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $onlySitemaps = false):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Retrieves the url for a category.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The id of the category.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>Optional language of details.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$onlySitemaps</td>
        <td>Whether or not to only include categories with 'sitemaps' = 'Y'. Default false.</td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId = null, <a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Search for categories
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The id of the category.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The requested page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>Number of items per page.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations to be loaded.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>Filters restrict the list of results. Results can be filtered by the following parameters: 'type','lang','parentId', 'plentyId', 'linklist'</td>
    </tr>
</table>


<pre>public <strong>createCategories</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Creates new categories, including CategoryDetails. At least one CategoryDetails object for the default language is required. The data fields &#039;plentyId&#039;,&#039;lang&#039; and &#039;name&#039; are required. Client objects can also be specified to activate visibility for a client.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data fields for the new Categories, including the details data fields</td>
    </tr>
</table>


<pre>public <strong>updateCategories</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Update categories, including optional CategoryDetails. The data fields &#039;plentyId&#039;,&#039;lang&#039; are required for the CategoryDetails object. Client objects can also be specified to change visibility for a client.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data fields for the Categories, including the details and client data fields</td>
    </tr>
</table>


<pre>public <strong>createCategory</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="category#category_models_category">Category</a>
</pre>

    
Creates a new category
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes a category by given id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteCategoryDetails</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Delete category details for the specified languages
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteCategoryClients</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deactivate availability for clients
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
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
    
## Models<a name="category_category_models"></a>
### Category<a name="category_models_category"></a>

Category


#### Namespace

`Plenty\Modules\Category\Models`


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
            <td>The unique ID of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentCategoryId</td>
            <td>The ID of the category's parent category. Value is <strong>null</strong> if category level is 1.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>level</td>
            <td>The category level of this category. This information is used for the sitemap.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The category type of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>linklist</td>
            <td>Flag that indicates if the category will be displayed in the online store's navigation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>right</td>
            <td>Flag that indicates who can see this category. <ul><li>all = Category is
                                                 visible to all visitors of the online store.</li><li>customer = Category and all of its subcategories are visible to
                                                 visitors of the online store that have logged in only. Visitors that are not logged in are redirected to the login page.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sitemap</td>
            <td>Flag that indicates if the category will be included in the sitemap.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>clients</td>
            <td>Collection of the clients (stores) that belong to this category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>details</td>
            <td>Collection of the category details that belong to this category</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CategoryBranch<a name="category_models_categorybranch"></a>

Category Branch


#### Namespace

`Plenty\Modules\Category\Models`


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
            <td>categoryId</td>
            <td>The ID of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category1Id</td>
            <td>The ID of the category tree's 1st level. If 1st value is identical to category ID, category is of this level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category2Id</td>
            <td>The ID of the category tree's 2nd level. If 2nd level value is identical to category ID, category is of this level. If 2nd level value is <strong>null</strong>, category is of a higher level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category3Id</td>
            <td>The ID of the category tree's 3rd level. If 3rd level value is identical to category ID, category is of this level. If 2nd level value is <strong>null</strong>, category is of a higher level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category4Id</td>
            <td>The ID of the category tree's 4th level. If 4th level value is identical to category ID, category is of this level. If 2nd level value is <strong>null</strong>, category is of a higher level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category5Id</td>
            <td>The ID of the category tree's 5th level. If 5th level value is identical to category ID, category is of this level. If 2nd level value is <strong>null</strong>, category is of a higher level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>category6Id</td>
            <td>The ID of the category tree's 6th level. If 6th level value is identical to category ID, category is of this level. If 2nd level value is <strong>null</strong>, category is of a higher level.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CategoryBranchMarketplace<a name="category_models_categorybranchmarketplace"></a>

The CategoryBranchMarketplace model


#### Namespace

`Plenty\Modules\Category\Models`


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
            <td>plenty_category_branch_marketplace_branch_id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plenty_category_branch_marketplace_webstore_id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>plenty_category_branch_marketplace_marketplace_id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>plenty_category_branch_marketplace_marketplace_sub_id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plenty_category_branch_marketplace_delimiter</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plenty_category_branch_marketplace_value1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plenty_category_branch_marketplace_value2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plenty_category_branch_marketplace_last_update</td>
            <td></td>
        </tr><tr>
            <td><a href="category#category_models_categorybranch">CategoryBranch</a>
</td>
            <td>branch</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CategoryClient<a name="category_models_categoryclient"></a>

The Category Client


#### Namespace

`Plenty\Modules\Category\Models`


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
            <td>The ID of the client (store) in which the category is visible. Several IDs can be separated by commas. If a subcategory is linked to a client, its parent categories will be linked to this client as well.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CategoryDetails<a name="category_models_categorydetails"></a>

CategoryDetails


#### Namespace

`Plenty\Modules\Category\Models`


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
            <td>categoryId</td>
            <td>The unique ID of the category these category details belong to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The ID of the client (store) in which the category is visible. If a subcategory is linked to a client, its parent categories will be linked to this client as well.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The <a href="https://developers.plentymarkets.com/rest-doc/introduction#languages" target="_blank">language</a> of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the category. The same category name can be used more than once in different categories or on different category levels. However, category names must be unique within the same category or level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The category text. The description is inserted into the online store using template variables.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description2</td>
            <td>The category text 2. The description 2 is inserted into the online store using template variables.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td>The short description of the category. The short description can be inserted into the store's design using template variables.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaKeywords</td>
            <td>HTML meta keywords to tag the category for search engines. More than one keyword can be separated by commas.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td>The meta description of the category. This description is analysed by search engines and displayed in search results. This text should be treated as an advertising text to maximise click-through from search engine result pages. Current recommended limit is 156 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>nameUrl</td>
            <td>The category name to be used for the category's URL. The same URL name can be used more than once in different categories or on different category levels. However, URL names must be unique within the same category or level. The URL name should not be changed once the category is indexed by search engines. If no URL name is specified, the name will automatically be used as the URL name when the category is created.<br />Important: Name should contain ASCII code only and no special characters. The following character strings may not be used as prefixes to URL names: a-, b-, c-, f-, fa-, p-, t-. These prefixes will be removed automatically. For instance, a-class will be changed to class automatically. However, the URL name aclass can be used for a category named A-class.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaTitle</td>
            <td>This will be displayed as the title of a tab in the web browser and as a search result in search engines. If this is left blank, the category name will be used as the title. Current recommended limit is 50 characters. Longer titles will be cut off.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>image</td>
            <td>The path to the image1 of the category.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>image2</td>
            <td>The path to the image2 of the category.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the category within a category level.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemListView</td>
            <td>The template the category is linked to for the category overview. The template determines what the category overview will look like for this category. This option is available for categories of the type <strong>Item</strong> only. Possible values: ItemViewCategoriesList, ItemViewCategoriesList2 to ItemViewCategoriesList10.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>singleItemView</td>
            <td>The template the category is linked to for the single item view. The template determines the appearance of the single item design for this category. This option is available for categories of the type <strong>Item</strong> only. Possible values: ItemViewSingleItem, ItemViewSingleItem2 to ItemViewSingleItem5.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pageView</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>fulltext</td>
            <td>Flag that indicates if the complete category text, i.e. the complete description, will be searched.<ul><li>Y = Complete text will be searched.</li><li>N = Text will not be searched completely.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaRobots</td>
            <td>Values from the meta element Robots are analyzed by Web crawlers. These values tell the crawler what it should do with the page and with the links on the page.<ul><li>all = Include this category in the search engine index and follow the links on the page.</li><li>index = Include in the search engine index.</li><li>nofollow = Do not follow the links on the page.</li><li>noindex = Do not include in the search engine index.</li><li>nofollow, noindex = Do not follow the links and do not include the category in the search engine index.</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>canonicalLink</td>
            <td>The URL of any category that contains the same content. This
                                                     will avoid duplicate content.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the category details were last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedBy</td>
            <td>The user who last updated the category details</td>
        </tr><tr>
            <td><a href="category#category_models_category">Category</a>
</td>
            <td>category</td>
            <td>The category these category details are associated with.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CategoryTemplate<a name="category_models_categorytemplate"></a>

Category Template


#### Namespace

`Plenty\Modules\Category\Models`


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
            <td>categoryId</td>
            <td>The unique ID of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The ID of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the template</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>content</td>
            <td>The content of the template</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
