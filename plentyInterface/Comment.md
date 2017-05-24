

# Comment<a name="comment_comment"></a>
    
## Contracts<a name="comment_comment_contracts"></a>
### CommentRepositoryContract<a name="comment_contracts_commentrepositorycontract"></a>

Get, create and delete comments.


#### Namespace

`Plenty\Modules\Comment\Contracts`



#### Methods

<pre>public <strong>getComment</strong>(<a target="_blank" href="http://php.net/int">int</a> $commentId):<a href="comment#comment_models_comment">Comment</a>
</pre>

    
Get a comment
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$commentId</td>
        <td>The ID of the comment</td>
    </tr>
</table>


<pre>public <strong>listComments</strong>():<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
List comments
    
<pre>public <strong>createComment</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="comment#comment_models_comment">Comment</a>
</pre>

    
Create a comment
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteComment</strong>(<a target="_blank" href="http://php.net/int">int</a> $commentId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a comment
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$commentId</td>
        <td>The ID of the comment</td>
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
    
## Models<a name="comment_comment_models"></a>
### Comment<a name="comment_models_comment"></a>

The comment model.


#### Namespace

`Plenty\Modules\Comment\Models`


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
            <td>The ID of the comment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceType</td>
            <td>The reference type. Valid types are:
<ul>
	<li>category</li>
	<li>contact</li>
	<li>order</li>
 <li>item_variation</li>
	</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referenceValue</td>
            <td>The reference value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the user</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the comment was created</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>text</td>
            <td>The comment text</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisibleForContact</td>
            <td>If true, the comment is visible for the associated contact.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
