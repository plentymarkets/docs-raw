

# Tag<a name="tag_tag"></a>
    
## Contracts<a name="tag_tag_contracts"></a>
### TagNameRepositoryContract<a name="tag_contracts_tagnamerepositorycontract"></a>

Repository for TagName


#### Namespace

`Plenty\Modules\Tag\Contracts`





#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $tagId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="tag#tag_models_tagname">TagName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The name data. The properties that are required to update an name can be found in the TagName model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The tag ID</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the name</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="tag#tag_models_tagname">TagName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The name data. The properties that are required to update an name can be found in the TagName model.</td>
    </tr>
</table>


<pre>public <strong>findByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The tag name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language of the name</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### TagRepositoryContract<a name="tag_contracts_tagrepositorycontract"></a>

The TagRepositoryContract is the interface for the tag repository.


#### Namespace

`Plenty\Modules\Tag\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="tag#tag_models_tag">Tag</a>
</pre>

    
Create a new tag.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The tag name</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $tagId):<a href="tag#tag_models_tag">Tag</a>
</pre>

    
Update a tag.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The tag data. The properties that are required to update an tag can be found in the Tag model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The tag ID</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $tagId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a tag by given tagId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The tag ID</td>
    </tr>
</table>


<pre>public <strong>getTagByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $name):<a href="tag#tag_models_tag">Tag</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td>The name of the tag</td>
    </tr>
</table>


<pre>public <strong>getTagsByIds</strong>(<a target="_blank" href="http://php.net/array">array</a> $ids):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$ids</td>
        <td>The IDs of the tags</td>
    </tr>
</table>


<pre>public <strong>getTagById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="tag#tag_models_tag">Tag</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getTagsByAvailability</strong>(<a target="_blank" href="http://php.net/string">string</a> $availabilityType):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$availabilityType</td>
        <td>The type of the availability. The following types are available.
<ul>
<li>blog</li>
<li>category</li>
<li>content_page</li>
<li>variation</li>
<li>ticket</li>
<li>board</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>getTagsByRelationship</strong>(<a target="_blank" href="http://php.net/string">string</a> $relationshipType, $value, <a target="_blank" href="http://php.net/bool">bool</a> $isUUID = false):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipType</td>
        <td>The relationship type.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td>The relationship value (string if UUID, otherwise int)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isUUID</td>
        <td>Whether the value is a UUID5 or not.</td>
    </tr>
</table>


<pre>public <strong>listTags</strong>(<a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Returns all tags
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createTag</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="tag#tag_models_tag">Tag</a>
</pre>

    
Creates a new tag
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Creates up to 50 new tags
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateBulk</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Updates up to 50 tags
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
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
    

### TagAvailabilityRepositoryContract<a name="tag_contracts_tagavailabilityrepositorycontract"></a>

Repository for TagAvailability


#### Namespace

`Plenty\Modules\Tag\Contracts`





#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $tagId, <a target="_blank" href="http://php.net/string">string</a> $availabilityType):<a href="tag#tag_models_tagavailability">TagAvailability</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The availability data. The properties that are required to update an tag can be found in the TagAvailability model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The tag ID</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$availabilityType</td>
        <td>The type of the availability. The following types are available.
<ul>
<li>blog</li>
<li>category</li>
<li>content_page</li>
<li>variation</li>
<li>ticket</li>
</ul></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="tag#tag_models_tagavailability">TagAvailability</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The availability data. The properties that are required to update an tag can be found in the TagAvailability model.</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### TagRelationshipRepositoryContract<a name="tag_contracts_tagrelationshiprepositorycontract"></a>

Repository for TagRelationship


#### Namespace

`Plenty\Modules\Tag\Contracts`





#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $tagId, <a target="_blank" href="http://php.net/string">string</a> $availabilityType, <a target="_blank" href="http://php.net/int">int</a> $relationshipValue):<a href="tag#tag_models_tagrelationship">TagRelationship</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The relationship data. The properties that are required to update a relationship can be found in the TagRelationship model.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The ID of the tag</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$availabilityType</td>
        <td>The type of the availability. The following types are available:
<ul>
<li>category</li>
<li>variation</li>
<li>ticket</li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationshipValue</td>
        <td>The value of the relationship. This value is the ID of the data set the tag is linked to, e.g. item ID 1234.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="tag#tag_models_tagrelationship">TagRelationship</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The relationship data. The properties that are required to update a relationship can be found in the TagRelationship model.</td>
    </tr>
</table>


<pre>public <strong>deleteRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationshipValue, <a target="_blank" href="http://php.net/int">int</a> $tagId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationshipValue</td>
        <td>The value of the relationship. This value is the ID of the data set the tag is linked to, e.g. item ID 1234.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The ID of the tag</td>
    </tr>
</table>


<pre>public <strong>deleteOneRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationshipValue, <a target="_blank" href="http://php.net/string">string</a> $relationshipType, <a target="_blank" href="http://php.net/int">int</a> $tagId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationshipValue</td>
        <td>The value of the relationship. This value is the ID of the data set the tag is linked to, e.g. item ID 1234.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipType</td>
        <td>The type of the relationship, i.e. <b>category</b>, <b>item</b> or <b>ticket</b></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The ID of the tag</td>
    </tr>
</table>


<pre>public <strong>deleteOneRelationByUUID</strong>(<a target="_blank" href="http://php.net/string">string</a> $relationshipUUID, <a target="_blank" href="http://php.net/string">string</a> $relationshipType, <a target="_blank" href="http://php.net/int">int</a> $tagId):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Delete a tag relationship by the uuid5 value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipUUID</td>
        <td>The uuid5 value of the relationship.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipType</td>
        <td>The type of the relationship, i.e. <b>board</b></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The ID of the tag</td>
    </tr>
</table>


<pre>public <strong>findByValueId</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td>The value of the relationship. This value is the ID of the data set the tag is linked to, e.g. item ID 1234.</td>
    </tr>
</table>


<pre>public <strong>findByTagId</strong>(<a target="_blank" href="http://php.net/int">int</a> $tagId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td>The ID of the tag</td>
    </tr>
</table>


<pre>public <strong>findRelationship</strong>(<a target="_blank" href="http://php.net/int">int</a> $tagId, <a target="_blank" href="http://php.net/int">int</a> $relationshipValue, <a target="_blank" href="http://php.net/string">string</a> $relationshipType):<a href="tag#tag_models_tagrelationship">TagRelationship</a>
</pre>

    
Gets a specific tag relationship or returns null
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tagId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationshipValue</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationshipValue, <a target="_blank" href="http://php.net/string">string</a> $relationshipType):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes tag links by reference value and relationship type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationshipValue</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteByUUID</strong>(<a target="_blank" href="http://php.net/string">string</a> $relationshipValue, <a target="_blank" href="http://php.net/string">string</a> $relationshipType):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>

    
Deletes tag links by uuid5 reference value and relationship type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipValue</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$relationshipType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listRelationships</strong>(<a target="_blank" href="http://php.net/array">array</a> $with = []):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Returns all tagRelationships
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
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
    
## Models<a name="tag_tag_models"></a>
### TagRelationship<a name="tag_models_tagrelationship"></a>

The tag relationship model.


#### Namespace

`Plenty\Modules\Tag\Models`




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
            <td>tagId</td>
            <td>The ID of the tag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tagType</td>
            <td>The type of tag.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>relationshipValue</td>
            <td>The ID of the data record for which a tag relationship is created</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relationshipUUID5</td>
            <td>The ID of the data record for which a tag relationship is created. For models with uuid5 as primary key</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Tag<a name="tag_models_tag"></a>

The Tag model


#### Namespace

`Plenty\Modules\Tag\Models`




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
            <td>The tag ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tagName</td>
            <td>The name of the tag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>color</td>
            <td>The color for the tag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>availabilities</td>
            <td>The availabilities of the tag.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td>The names of the tag.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>relationships</td>
            <td>The relationships of the tag.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The updated at timestamp of the tag.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The created at timestamp of the tag.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TagName<a name="tag_models_tagname"></a>

The tag name model.


#### Namespace

`Plenty\Modules\Tag\Models`




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
            <td>The name ID of the tag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>tagId</td>
            <td>The tag ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tagLang</td>
            <td>The lang of the tag name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tagName</td>
            <td>The name of the tag.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TagAvailability<a name="tag_models_tagavailability"></a>

The tag availability model.


#### Namespace

`Plenty\Modules\Tag\Models`




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
            <td>tagId</td>
            <td>The Tag ID of the tag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tagType</td>
            <td>The type of the tag. The following types are available.
<ul>
<li>blog</li>
<li>category</li>
<li>content_page</li>
<li>variation</li>
<li>ticket</li>
<li>board</li>
<li>order</li>
</ul></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
