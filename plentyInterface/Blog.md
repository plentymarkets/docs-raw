

# Blog<a name="blog_blog"></a>
    
## Contracts<a name="blog_blog_contracts"></a>
### BlogPostRepositoryContract<a name="blog_contracts_blogpostrepositorycontract"></a>

This interface provides methods to create, read, list, update and delete blog posts


#### Namespace

`Plenty\Modules\Blog\Contracts`





#### Methods

<pre>public <strong>createPost</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="blog#blog_models_blogpost">BlogPost</a>
</pre>

    
Creates a new blog post.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Blog post data</td>
    </tr>
</table>


<pre>public <strong>getPost</strong>(<a target="_blank" href="http://php.net/string">string</a> $blogPostId):<a href="blog#blog_models_blogpost">BlogPost</a>
</pre>

    
Get a single blog post by its ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$blogPostId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listPosts</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists all blog posts for current plenty ID.
    
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
        <td></td>
    </tr>
</table>


<pre>public <strong>updatePost</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/string">string</a> $blogPostId):<a href="blog#blog_models_blogpost">BlogPost</a>
</pre>

    
Update data for a post
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$blogPostId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deletePost</strong>(<a target="_blank" href="http://php.net/string">string</a> $blogPostId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a single blog post by its ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$blogPostId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>migratePosts</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Migrate old posts to new
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getOldPostById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get old blog post by its ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
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
    
## Models<a name="blog_blog_models"></a>
### BlogPost<a name="blog_models_blogpost"></a>

The blog post model.


#### Namespace

`Plenty\Modules\Blog\Models`




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
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>data</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="blog_blog_services"></a>
### BlogPluginService<a name="blog_services_blogpluginservice"></a>

Blog plugin service


#### Namespace

`Plenty\Modules\Blog\Services`





#### Methods

<pre>public <strong>getPluginSetIdFromConfig</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get plugin set ID
    
<pre>public <strong>findCategoryByUrl</strong>(<a target="_blank" href="http://php.net/string">string</a> $level1, <a target="_blank" href="http://php.net/string">string</a> $level2 = null, <a target="_blank" href="http://php.net/string">string</a> $level3 = null, <a target="_blank" href="http://php.net/string">string</a> $level4 = null, <a target="_blank" href="http://php.net/string">string</a> $level5 = null, <a target="_blank" href="http://php.net/string">string</a> $level6 = null, <a target="_blank" href="http://php.net/int">int</a> $webstoreId = null, <a target="_blank" href="http://php.net/string">string</a> $lang = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$level1</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$level2</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$level3</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$level4</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$level5</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$level6</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


