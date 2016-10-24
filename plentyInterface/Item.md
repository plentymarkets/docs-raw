

# Attribute<a name="item_attribute"></a>
    
## Contracts<a name="item_attribute_contracts"></a>
### AttributeNameRepositoryContract<a name="item_contracts_attributenamerepositorycontract"></a>

Repository for AttributeName

#### Namespace

Plenty\Modules\Item\Attribute\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="item#item_models_attributename">AttributeName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributename">AttributeName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributename">AttributeName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByAttributeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="item#item_models_attributename">AttributeName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
</table>



### AttributeRepositoryContract<a name="item_contracts_attributerepositorycontract"></a>

Repository for Attribute

#### Namespace

Plenty\Modules\Item\Attribute\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_attribute">Attribute</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attribute">Attribute</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attribute">Attribute</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>



### AttributeValueNameRepositoryContract<a name="item_contracts_attributevaluenamerepositorycontract"></a>

Repository for AttributeValueName

#### Namespace

Plenty\Modules\Item\Attribute\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
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


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>findByValueId</strong>(<a target="_blank" href="http://php.net/int">int</a> $valueId):<a href="item#item_models_attributevaluename">AttributeValueName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$valueId</td>
        <td></td>
    </tr>
</table>



### AttributeValueRepositoryContract<a name="item_contracts_attributevaluerepositorycontract"></a>

Repository for AttributeValue

#### Namespace

Plenty\Modules\Item\Attribute\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId):<a href="item#item_models_attributevalue">AttributeValue</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByAttributeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $attributeId, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_attributevalue">AttributeValue</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$attributeId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_attribute_models"></a>
### Attribute<a name="item_models_attribute"></a>

The Attribute model including AttributeName and AttributeValue

#### Namespace

Plenty\Modules\Item\Attribute\Models


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
            <td>The unique ID of the attribute. The ID is assigned automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The back end name of the attribute. The name must be unique and must not contain commas, colons, semicolons or quotation marks. It is not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the attribute. Attributes are displayed in the attribute overview in ascending order by position.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSurchargePercental</td>
            <td>Flag that indicates if the surcharge is percental.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isLinkableToImage</td>
            <td>Flag that indicates if an image can be linked to the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazonAttribute</td>
            <td>The attribute of the market Amazon that this attribute is liked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fruugoAttribute</td>
            <td>The attribute of the market Fruugo that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pixmaniaAttribute</td>
            <td>The attribute of the market PIXmania that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ottoAttribute</td>
            <td>The attribute of the market OTTO that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>googleShoppingAttribute</td>
            <td>The attribute of the market Google Shopping that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannAtEpAttribute</td>
            <td>The component of the market neckermann AT EP that this attribute is linked to. To list variations on this market, attributes must be linked to one of the components specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>typeOfSelectionInOnlineStore</td>
            <td>How customers can select the attribute in the front end of a client. To allow attribute selection by check mark, attribute availability must be checked on the client side.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>laRedouteAttribute</td>
            <td>The attribute of the market La Redoute that this attribute is linked to. To list variations on this market, attributes must be linked to one of the attributes specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isGroupable</td>
            <td>Flag that indicates if the attribute can be grouped in item lists. If yes, variations with this attribute can be shown in the ItemViewCategoriesList template first. Other attributes are nested and can only be selected after this attribute has been selected.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>langs</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>values</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### AttributeName<a name="item_models_attributename"></a>

The AttributeName model including Attribute

#### Namespace

Plenty\Modules\Item\Attribute\Models


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
            <td>attributeId</td>
            <td>The id of the attribute.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>Language code of the attribute. Supported languages:
<ul>
<li><strong>de</strong> = German</li>
<li><strong>en</strong> = English</li>
<li><strong>fr</strong> = French</li>
<li><strong>it</strong> = Italian</li>
<li><strong>es</strong> = Spanish</li>
<li><strong>tr</strong> = Turkish</li>
<li><strong>nl</strong> = Dutch</li>
<li><strong>pl</strong> = Polish</li>
<li><strong>pt</strong> = Portuguese</li>
<li><strong>nn</strong> = Norwegian</li>
<li><strong>da</strong> = Danish</li>
<li><strong>se</strong> = Swedish</li>
<li><strong>cz</strong> = Czech</li>
<li><strong>ru</strong> = Russian</li>
<li><strong>sk</strong> = Slovak</li>
<li><strong>cn</strong> = Chinese</li>
<li><strong>vn</strong> = Vietnamese</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute. This attribute name is displayed in the online store.</td>
        </tr><tr>
            <td><a href="item#item_models_attribute">Attribute</a>
</td>
            <td>attribute</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### AttributeValue<a name="item_models_attributevalue"></a>

The AttributeValue model including Attribute and AttributeValueName

#### Namespace

Plenty\Modules\Item\Attribute\Models


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
            <td>The unique ID of the attribute value. The ID is assigned automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeId</td>
            <td>The unique ID of the attribute associated with the attribute value. The ID is assigned automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The back end name of the attribute value. This name can only be assigned once per attribute. It is not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the attribute value. Attribute values are sorted in ascending order by position.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>image</td>
            <td>The name of the image associated with the attribute value; naming pattern is attr\_\{valueId\}.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>comment</td>
            <td>Optional comment on the attribute value. Comments are not visible in the plentymarkets front end.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazonValue</td>
            <td>The attribute value of the market Amazon that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the values specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ottoValue</td>
            <td>The attribute value of the market OTTO that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the attribute values specified by the market.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>neckermannAtEpValue</td>
            <td>The attribute value of the market Neckermann AT EP that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the attribute values specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>laRedouteValue</td>
            <td>The attribute value of the market La Redoute that this attribute value maps to. To list variations on this market, attribute values must be linked to one of the attribute values specified by the market. Check documentation of the market for permitted values.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tracdelightValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>percentageDistribution</td>
            <td>The percentage for automatic stock distribution of attribute values. When reordering an item, the quantities of attribute values is automatically distributed among the total quantity.</td>
        </tr><tr>
            <td><a href="item#item_models_attribute">Attribute</a>
</td>
            <td>attribute</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>valueNames</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### AttributeValueName<a name="item_models_attributevaluename"></a>

The AttributeValueName model including AttributeValue

#### Namespace

Plenty\Modules\Item\Attribute\Models


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
            <td>valueId</td>
            <td>The unique ID of the attribute value. The ID is assigned automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>Language code of the attribute value. Supported languages:
<ul>
<li><strong>de</strong> = German</li>
<li><strong>en</strong> = English</li>
<li><strong>fr</strong> = French</li>
<li><strong>it</strong> = Italian</li>
<li><strong>es</strong> = Spanish</li>
<li><strong>tr</strong> = Turkish</li>
<li><strong>nl</strong> = Dutch</li>
<li><strong>pl</strong> = Polish</li>
<li><strong>pt</strong> = Portuguese</li>
<li><strong>nn</strong> = Norwegian</li>
<li><strong>da</strong> = Danish</li>
<li><strong>se</strong> = Swedish</li>
<li><strong>cz</strong> = Czech</li>
<li><strong>ru</strong> = Russian</li>
<li><strong>sk</strong> = Slovak</li>
<li><strong>cn</strong> = Chinese</li>
<li><strong>vn</strong> = Vietnamese</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the attribute value. This attribute value name is displayed in the online store.</td>
        </tr><tr>
            <td><a href="item#item_models_attributevalue">AttributeValue</a>
</td>
            <td>attributeValue</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Availability<a name="item_availability"></a>
    
## Contracts<a name="item_availability_contracts"></a>
### AvailabilityRepositoryContract<a name="item_contracts_availabilityrepositorycontract"></a>

Repository for item availability.

#### Namespace

Plenty\Modules\Item\Availability\Contracts



#### Methods

<pre>public <strong>findAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_availability">Availability</a>
</pre>
    
Find an availability configuration by a given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The item availability id that needs to be found.</td>
    </tr>
</table>


## Models<a name="item_availability_models"></a>
### Availability<a name="item_models_availability"></a>

The item availability model

#### Namespace

Plenty\Modules\Item\Availability\Models


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
            <td>The id of this availability.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>icon</td>
            <td>The icon of this availability.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>averageDays</td>
            <td>The average days for this availability.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>languages</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### AvailabilityLanguage<a name="item_models_availabilitylanguage"></a>

The item availability lang model

#### Namespace

Plenty\Modules\Item\Availability\Models


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
            <td>availabilityId</td>
            <td>The availability ID this language belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>language</td>
            <td>The language key ('en', 'de' etc.).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The given name for this translation.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Barcode<a name="item_barcode"></a>
    
## Contracts<a name="item_barcode_contracts"></a>
### BarcodeRepositoryContract<a name="item_contracts_barcoderepositorycontract"></a>

Repository for Barcode

#### Namespace

Plenty\Modules\Item\Barcode\Contracts



#### Methods

<pre>public <strong>showBarcode</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Show an barcode by given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createBarcode</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_barcode">Barcode</a>
</pre>
    
Create new barcode
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateBarcode</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcode">Barcode</a>
</pre>
    
Update an existing barcode
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteBarcode</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Delete an barcode by given id. If at least one relation exists, throws an exception.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findBarcodeById</strong>(<a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcode">Barcode</a>
</pre>
    
Find an existing barcode by given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findBarcodesByType</strong>(<a target="_blank" href="http://php.net/string">string</a> $barcodeType, <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Get list of barcodes from type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$barcodeType</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>allBarcodes</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>
    
Get list of barcodes
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createBarcodeReferrerRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a href="item#item_models_barcodelinkreferrer">BarcodeLinkReferrer</a>
</pre>
    
Create new barcode referrer for given referrer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteBarcodeReferrerRelation</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrer, <a target="_blank" href="http://php.net/int">int</a> $barcodeId):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Delete existing barcode referrer with given referrer.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrer</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$barcodeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findBarcodesByReferrerRelation</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrer, <a target="_blank" href="http://php.net/int">int</a> $perPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Get barcode referrer with given referrer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrer</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_barcode_models"></a>
### Barcode<a name="item_models_barcode"></a>

The barcode model including barcode referrer

#### Namespace

Plenty\Modules\Item\Barcode\Models


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
            <td>The ID of the barcode. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the barcode</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the barcode. Possible values: EAN_8, EAN_13, EAN_14, EAN_128, ISBN, QR, CODE_128, UPC</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>referrers</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### BarcodeLinkReferrer<a name="item_models_barcodelinkreferrer"></a>

The barcode link referrer model including the barcode

#### Namespace

Plenty\Modules\Item\Barcode\Models


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
            <td>barcodeId</td>
            <td>The ID of the barcode. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The ID of the referrer. To activate all referrers, the value <strong>-1</strong> must be specified. This value activates all referrers in the system by default, including any referrers added at a later stage.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the barcode was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the barcode was last updated.</td>
        </tr><tr>
            <td><a href="item#item_models_barcode">Barcode</a>
</td>
            <td>barcode</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# DataLayer<a name="item_datalayer"></a>
    
## Contracts<a name="item_datalayer_contracts"></a>
### ItemDataLayerRepositoryContract<a name="item_contracts_itemdatalayerrepositorycontract"></a>



#### Namespace

Plenty\Modules\Item\DataLayer\Contracts



#### Methods

<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="item#item_models_recordlist">RecordList</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>searchWithPagination</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns, <a target="_blank" href="http://php.net/array">array</a> $filter = [], <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_datalayer_models"></a>
### DataLayerModel<a name="item_models_datalayermodel"></a>



#### Namespace

Plenty\Modules\Item\DataLayer\Models



#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemBase<a name="item_models_itembase"></a>

ItemDataLayer - ItemBase

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>abo</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addCmsPage</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonFba</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonProductType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>apiCondition</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storeSpecial</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>bestofferAutoDeclinePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>condition</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>crossSellingCharacter</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customsTariffNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>defaultShippingCost</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directCrossArticle</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayPreset</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>epid</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fedas</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>markingOne</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>markingTwo</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>flashFile</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flashHeight</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flashWidth</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free3</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free4</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free5</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free6</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free7</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free8</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free9</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free10</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free11</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free12</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free13</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free14</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free15</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free16</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free17</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free18</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free19</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>free20</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ageRestriction</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>hasAttribute</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>inactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>isPacket</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketStockBuffer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>noCoupon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>producingCountryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceOnly4orderby</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>producer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>producerId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rating</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>revenueAccount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>scoActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>scoMinPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>scoMinStockNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>serialNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shippingWithAmazonFba</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sitemapPublished</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storingPosition</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>votes</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>tradoriaCategory</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemCrossSelling<a name="item_models_itemcrossselling"></a>

ItemCrossSelling

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>crossItemId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>relationship</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dynamic</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemDescription<a name="item_models_itemdescription"></a>

ItemDescription

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>characterCache</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>characterCacheXml</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>characterUpdate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keywords</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>technicalData</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlContent</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemProperty<a name="item_models_itemproperty"></a>

ItemProperty

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>itemPropertyId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>propertyValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>propertyValueType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isOrderProperty</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>propertyOrderMarkup</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemShippingProfiles<a name="item_models_itemshippingprofiles"></a>

ItemShippingProfiles

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>tags</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### Record<a name="item_models_record"></a>

Record

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td><a href="item#item_models_itembase">ItemBase</a>
</td>
            <td>itemBase</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemPropertyList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemCrossSellingList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_itemdescription">ItemDescription</a>
</td>
            <td>itemDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemShippingProfilesList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationAttributeValueList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationbarcode">VariationBarcode</a>
</td>
            <td>variationBarcode</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBarcodeList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationbase">VariationBase</a>
</td>
            <td>variationBase</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBundleComponentList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationCategoryList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationImageList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationLinkMarketplace</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationLinkWebstore</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationmarketstatus">VariationMarketStatus</a>
</td>
            <td>variationMarketStatus</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationretailprice">VariationRetailPrice</a>
</td>
            <td>variationRecommendedRetailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationRecommendedRetailPriceList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationretailprice">VariationRetailPrice</a>
</td>
            <td>variationRetailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationRetailPriceList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationstandardcategory">VariationStandardCategory</a>
</td>
            <td>variationStandardCategory</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationstock">VariationStock</a>
</td>
            <td>variationStock</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationstockbuffer">VariationStockBuffer</a>
</td>
            <td>variationStockBuffer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationStockList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSupplierList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationwarehouse">VariationWarehouse</a>
</td>
            <td>variationWarehouse</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationWarehouseList</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_variationspecialofferretailprice">VariationSpecialOfferRetailPrice</a>
</td>
            <td>variationSpecialOfferRetailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSpecialOfferRetailPriceList</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### RecordList<a name="item_models_recordlist"></a>

RecordList

#### Namespace

Plenty\Modules\Item\DataLayer\Models



#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationAttributeValue<a name="item_models_variationattributevalue"></a>

VariationAttributeValue

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>attributeId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationBarcode<a name="item_models_variationbarcode"></a>

VariationBarcode

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>code</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>barcodeId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>barcodeType</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationBase<a name="item_models_variationbase"></a>

VariationBase

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>active</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueSetId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockInvisible</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>bundleTyp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockNoStockIcon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockPositiveStockIcon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>autoStockVisible</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>availability</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>averageOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>content</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitCombinationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>estimatedAvailability</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>heightMm</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lengthMm</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>limitOrderByStockSelect</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainWarehouse</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>model</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>operatingCostsPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnits</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnitType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>parentItemVariationQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>picking</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customsPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceCalculationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>primaryVariation</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>primaryVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>storageCosts</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>transportationCosts</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>unitId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitLoadDevice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitsContained</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightG</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightNetG</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>maximumOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>minimumOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>intervalOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>availableUntil</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>releaseDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>widthMm</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationBundleComponent<a name="item_models_variationbundlecomponent"></a>

VariationBundleComponent

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>componentVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>componentQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>CreatedTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>LastUpdateTimestamp</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationCategory<a name="item_models_variationcategory"></a>

VariationCategory

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>neckermannPrimary</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationImage<a name="item_models_variationimage"></a>

VariationImage

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>imageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>cleanImageName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationLinkMarketplace<a name="item_models_variationlinkmarketplace"></a>

VariationLinkMarketplace

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>created</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketplaceId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationLinkWebstore<a name="item_models_variationlinkwebstore"></a>

VariationLinkWebstore

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>created</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationMarketStatus<a name="item_models_variationmarketstatus"></a>

VariationMarketStatus

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketAccountId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>initialSku</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>sku</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>active</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastExportTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>deletedTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>marketStatus</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>additionalInformation</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationRetailPrice<a name="item_models_variationretailprice"></a>

VariationRetailPrice

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>priceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>retailPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>basePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkup</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkupNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>classRebatePercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>classRebate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>classRebateNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryRebatePercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryRebate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>categoryRebateNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRatio</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationSpecialOfferRetailPrice<a name="item_models_variationspecialofferretailprice"></a>

VariationSpecialOfferRetailPrice

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>retailPriceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>retailPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>retailPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>basePriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitPriceNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkup</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>orderParamsMarkupNet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>vatValue</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>currency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>exchangeRatio</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationStandardCategory<a name="item_models_variationstandardcategory"></a>

VariationStandardCategory

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>manually</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationStock<a name="item_models_variationstock"></a>

VariationStock

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>warehouseId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>stockPhysical</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedStock</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedEbay</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reorderDelta</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockNet</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updateAmazon</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatePixmania</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>warehouseType</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reordered</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedBundle</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>averagePurchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>warehousePriority</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>lastCalculateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedOutOfStock</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>reservedBasket</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationStockBuffer<a name="item_models_variationstockbuffer"></a>

VariationStockBuffer

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>stockBuffer</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationSupplier<a name="item_models_variationsupplier"></a>

VariationSupplier

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>createdTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>deliveryTimeInDays</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>discount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>discountable</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemNumber</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>itemVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastPriceQuery</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minimumOrderValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>packagingUnit</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>supplierId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationWarehouse<a name="item_models_variationwarehouse"></a>

VariationWarehouse

#### Namespace

Plenty\Modules\Item\DataLayer\Models


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
            <td>variationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseZoneId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reorderLevel</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maximumStock</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockBuffer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockTurnoverInDays</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storageLocationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# DefaultShippingCost<a name="item_defaultshippingcost"></a>
    
## Contracts<a name="item_defaultshippingcost_contracts"></a>
### DefaultShippingCostRepositoryContract<a name="item_contracts_defaultshippingcostrepositorycontract"></a>

Repository for DefaultShippingCost

#### Namespace

Plenty\Modules\Item\DefaultShippingCost\Contracts



#### Methods

<pre>public <strong>findShippingCost</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/float">float</a> $referrerId, <a target="_blank" href="http://php.net/int">int</a> $shippingDestinationId, <a target="_blank" href="http://php.net/int">int</a> $paymentMethodId):<a target="_blank" href="http://php.net/float">float</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$shippingDestinationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paymentMethodId</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_defaultshippingcost_models"></a>
### DefaultShippingCost<a name="item_models_defaultshippingcost"></a>

The default shipping cost model

#### Namespace

Plenty\Modules\Item\DefaultShippingCost\Models


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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>profileId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Item<a name="item_item"></a>
    
## Contracts<a name="item_item_contracts"></a>
### ItemRepositoryContract<a name="item_contracts_itemrepositorycontract"></a>

Repository for item basket

#### Namespace

Plenty\Modules\Item\Item\Contracts



#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId, <a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/string">string</a> $lang = &quot;de&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
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
    
## Models<a name="item_item_models"></a>
### Item<a name="item_models_item"></a>

The item model

#### Namespace

Plenty\Modules\Item\Item\Models


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
            <td>The ID of the item. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the item. Because Set items are managed using a separate route, this valid is always Default.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockType</td>
            <td>The stock type of the item. Possible values:<ul><li>0 = Stocked item (default)</li><li>1 = Production item</li><li>2 = Colli</li><li>3 = Special order item</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storeSpecial</td>
            <td>Option to present items more prominently in the online store.<ul><li>1 = Special offer</li><li>2 = New items</li><li>3 = Top items</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ownerId</td>
            <td>The plentymarkets user that is assigned as owner of this item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>manufacturerId</td>
            <td>The ID of the manufacturer of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>producingCountryId</td>
            <td>The ID of the country in which the item was manufactured.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainVariationId</td>
            <td>The ID of the main variation of the item. The ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customsTariffNumber</td>
            <td>The customs tariff number of the item; usually a 11 digit code number based on the Harmonised System</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>revenueAccount</td>
            <td>The revenue account the item is linked to. An individual revenue account can be saved for each item in plentymarkets. If this is not done, plentymarkets automatically determines a revenue account based on the VAT rate.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>couponRestriction</td>
            <td>Indicates if the item can be purchased using a coupon.<ul><li>0 = Permitted</li><li>1 = Not permitted</li><li>2 = Purchasable with coupon only</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>condition</td>
            <td>The condition of the item. Possible values:<ul><li>0 = New</li><li>1 = Used</li><li>2 = Boxed as new</li><li>3 = New with label</li><li>4 = Factory seconds</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>conditionApi</td>
            <td>The condition of the item that is transferred to markets via API.<ul><li>0 = New</li><li>1 = Used but as new</li><li>2 = Used but very good</li><li>3 = Used but good</li><li>4 = Used but acceptable</li><li>5 = Factory seconds</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>Timestamp of the date and time the item was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>Timestamp of the last date and time the item was updated.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSubscribable</td>
            <td>Flag that indicates if the item can be ordered as a subscription item. If yes, the item can be ordered for delivery at regular intervals.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonFbaPlatform</td>
            <td>Indicates the platform used for Fulfilment by Amazon (FBA). <ul><li>0 = Do not use</li><li>1 = AMAZON EU (Europe)</li><li>2 = AMAZON FE (Far East)</li><li>3 = AMAZON NA (North America)</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isShippableByAmazon</td>
            <td>Flag that indicates if the item can be shipped with Amazon Multi-Channel. Amazon Multi-Channel Fulfillment is a service for fulfilling orders from sales channels other than Amazon platforms using inventory stored in the Amazon fulfillment center.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>amazonProductType</td>
            <td>The Amazon product type of the item. List of IDs: https://www.plentymarkets.co.uk/manual/data-exchange/data-formats/item/</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>amazonFedas</td>
            <td>The FEDAS product classification key of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayPresetId</td>
            <td>The eBay preset ID. This plentymarkets ID must be specified to save values for $ebayCategory, $ebayCategory2, $ebayStoreCategory and $ebayStoreCategory2.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory</td>
            <td>The eBay category 1 of the item. This category is used when a new listing is created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayCategory2</td>
            <td>The eBay category 2 of the item. This category is used when a new listing is created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory</td>
            <td>The ID of the eBay store category 1 of the item. This value is used for new listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayStoreCategory2</td>
            <td>The ID of the eBay store category 2 of the item. This value is used for new listings.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>rakutenCategoryId</td>
            <td>The ID of the Rakuten category of this item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flagOne</td>
            <td>Flag 1 of the item. Flags can be used to organise and filter items. Each item can be assigned up to two flags. Possible values: 1 to 31, 0 = no flag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flagTwo</td>
            <td>Flag 2 of the item. Flags can be used to organise and filter items. Each item can be assigned up to two flags. Possible values: 1 to 31, 0 = no flag</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ageRestriction</td>
            <td>The age customers must be to purchase the item. Items with an age rating of 18+ must be linked to a shipping profile for which the PostIdent option is activated.<ul><li>0 = None available</li><li>3 = Released for ages 3 and up</li><li>6 = Ages 6 and up</li><li>12 = Ages 12 and up</li><li>16 = Ages 16 and up</li><li>18 = Ages 18 and up</li><li>50 = Not marked</li><li>88 = Not required</li><li>99 = Unknown</li></ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedback</td>
            <td>The feedback, i.e. rating, that this item received. Possible values are 1 to 5 or 1 to 10 depending on the maximum rating setting. An initial feedback can be saved for items. The saved value will then be displayed as the initial feedback. Every time new feedback is submitted, the average value will be recalculated automatically.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free1</td>
            <td>The content of the free text field 1. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free2</td>
            <td>The content of the free text field 2. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free3</td>
            <td>The content of the free text field 3. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free4</td>
            <td>The content of the free text field 4. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free5</td>
            <td>The content of the free text field 5. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free6</td>
            <td>The content of the free text field 6. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free7</td>
            <td>The content of the free text field 7. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free8</td>
            <td>The content of the free text field 8. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free9</td>
            <td>The content of the free text field 9. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free10</td>
            <td>The content of the free text field 10. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free11</td>
            <td>The content of the free text field 11. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free12</td>
            <td>The content of the free text field 12. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free13</td>
            <td>The content of the free text field 13. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free14</td>
            <td>The content of the free text field 14. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free15</td>
            <td>The content of the free text field 15. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free16</td>
            <td>The content of the free text field 16. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free17</td>
            <td>The content of the free text field 17. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free18</td>
            <td>The content of the free text field 18. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free19</td>
            <td>The content of the free text field 19. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>free20</td>
            <td>The content of the free text field 20. This can be displayed in the online store or on eBay.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>texts</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemText<a name="item_models_itemtext"></a>

The item text model

#### Namespace

Plenty\Modules\Item\Item\Models


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
            <td>lang</td>
            <td>The language of the item text.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name1</td>
            <td>Default name of the item displayed in the online store and used for markets. The maximum length is 240 characters. The item name is also used for structuring the item URL.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td>Alternative item name that can be used e.g. for markets. The maximum length is 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td>Alternative item name that can be used e.g. for markets. The maximum length is 240 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td>The preview text of the item. This short description text can be displayed as a teaser in item lists.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td>The meta description of the item. This description is analysed by search engines and displayed in search results. This text should be treated as an advertising text to maximise click-through from search engine result pages. Current recommended limit is 156 characters.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The detailed description of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>technicalData</td>
            <td>Technical data of the item.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>keywords</td>
            <td>HTML meta keywords to tag the item for search engines. More than one keyword can be separated by commas.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlPath</td>
            <td>he item's URL path in the online store. By default, the URL path consists of the categories and the item name. The path is assigned automatically when the item is created and is displayed as part of the URL when the item is selected in the online store.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# ItemImage<a name="item_itemimage"></a>
    
## Models<a name="item_itemimage_models"></a>
### ItemImageAvailability<a name="item_models_itemimageavailability"></a>

ItemImageAvailability

#### Namespace

Plenty\Modules\Item\ItemImage\Models


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
            <td>imageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemImageName<a name="item_models_itemimagename"></a>

ItemImageName

#### Namespace

Plenty\Modules\Item\ItemImage\Models


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
            <td>imageId</td>
            <td>The image id of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The lang of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the image</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>alternate</td>
            <td>The alternate name of the image</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ItemImageUpload<a name="item_models_itemimageupload"></a>

ItemImage

#### Namespace

Plenty\Modules\Item\ItemImage\Models


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
            <td>autoincrement</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>created</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updated</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uploadImageData</td>
            <td>base64 encoded image data</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uploadUrl</td>
            <td>the url to load the image from</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uploadFileName</td>
            <td>filename for new image</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Manufacturer<a name="item_manufacturer"></a>
    
## Contracts<a name="item_manufacturer_contracts"></a>
### ManufacturerCommissionRepositoryContract<a name="item_contracts_manufacturercommissionrepositorycontract"></a>

Repository for ManufacturerCommission

#### Namespace

Plenty\Modules\Item\Manufacturer\Contracts



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_manufacturercommission">ManufacturerCommission</a>
</pre>
    
Find one ManufacturerCommission by given Id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_manufacturercommission">ManufacturerCommission</a>
</pre>
    
Creates new ManufacturerCommission
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_manufacturercommission">ManufacturerCommission</a>
</pre>
    
Updates existing ManufacturerCommission
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>
    
Delete an ManufacturerCommission by givenId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByManufacturerId</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Find ManufacturerCommissions by given ManufacturerId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>



### ManufacturerRepositoryContract<a name="item_contracts_manufacturerrepositorycontract"></a>

Repository for item manufacturers

#### Namespace

Plenty\Modules\Item\Manufacturer\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_manufacturer">Manufacturer</a>
</pre>
    
store a new manufacturer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="item#item_models_manufacturer">Manufacturer</a>
</pre>
    
Update an existing manufacturer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    
Delete a manufacturer by the manufacturer id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $manufacturerId):<a href="item#item_models_manufacturer">Manufacturer</a>
</pre>
    
Find an existing Manufacturer
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$manufacturerId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $params = [], <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>
    
Search manufacturers by Filter
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_manufacturer_models"></a>
### Manufacturer<a name="item_models_manufacturer"></a>

The item manufacturer model

#### Namespace

Plenty\Modules\Item\Manufacturer\Models


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
            <td>The name of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>logo</td>
            <td>The logo of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>url</td>
            <td>The url of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pixmaniaBrandId</td>
            <td>The pixmania brand id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannBrandId</td>
            <td>The neckermann brand id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalName</td>
            <td>The external name of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannAtEpBrandId</td>
            <td>The neckermann at ep brand id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>neckermannAtCdBrandId</td>
            <td>The neckermann at cd brand id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>street</td>
            <td>The street of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>houseNo</td>
            <td>The house number of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>postcode</td>
            <td>The postal code of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>town</td>
            <td>The town of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The country id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>phoneNumber</td>
            <td>The phone number of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>faxNumber</td>
            <td>The fax number of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>email</td>
            <td>The email of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>laRedouteBrandId</td>
            <td>The la redoute brand id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>manufacturerComment</td>
            <td>The comment of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td>The last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>commissions</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### ManufacturerCommission<a name="item_models_manufacturercommission"></a>

The item manufacturer commission model

#### Namespace

Plenty\Modules\Item\Manufacturer\Models


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
            <td>The id of the commission</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>manufacturerId</td>
            <td>The id of the manufacturer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>clientId</td>
            <td>The id of the client</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>referrerId</td>
            <td>The id of the referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>commission</td>
            <td>The value of the commission</td>
        </tr><tr>
            <td><a href="item#item_models_manufacturer">Manufacturer</a>
</td>
            <td>manufacturer</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Property<a name="item_property"></a>
    
## Contracts<a name="item_property_contracts"></a>
### PropertyItemNameRepositoryContract<a name="item_contracts_propertyitemnamerepositorycontract"></a>

Repository for property item name

#### Namespace

Plenty\Modules\Item\Property\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyItemId):<a href="item#item_models_propertyitemname">PropertyItemName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyitemname">PropertyItemName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyitemname">PropertyItemName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByPropertyItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId):<a href="item#item_models_propertyitemname">PropertyItemName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
</table>



### PropertyItemRepositoryContract<a name="item_contracts_propertyitemrepositorycontract"></a>

Repository for property item

#### Namespace

Plenty\Modules\Item\Property\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_propertyitem">PropertyItem</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_propertyitem">PropertyItem</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_propertyitem">PropertyItem</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>



### PropertyMarketComponentRepositoryContract<a name="item_contracts_propertymarketcomponentrepositorycontract"></a>

Repository for property market component

#### Namespace

Plenty\Modules\Item\Property\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyItemId):<a href="item#item_models_propertymarketcomponent">PropertyMarketComponent</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/float">float</a> $marketReference):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketReference</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/float">float</a> $marketReference):<a href="item#item_models_propertymarketcomponent">PropertyMarketComponent</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketReference</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/float">float</a> $marketReference):<a href="item#item_models_propertymarketcomponent">PropertyMarketComponent</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$marketReference</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByPropertyItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId):<a href="item#item_models_propertymarketcomponent">PropertyMarketComponent</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPropertyMarketComponents</strong>(<a target="_blank" href="http://php.net/float">float</a> $referrerId, <a target="_blank" href="http://php.net/int">int</a> $componentId = null):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/float">float</a></td>
        <td>$referrerId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$componentId</td>
        <td></td>
    </tr>
</table>



### PropertySelectionRepositoryContract<a name="item_contracts_propertyselectionrepositorycontract"></a>

Repository for property selection

#### Namespace

Plenty\Modules\Item\Property\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyItemId):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByPropertyItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyItemId):<a href="item#item_models_propertyselection">PropertySelection</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyItemId</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_property_models"></a>
### PropertyItem<a name="item_models_propertyitem"></a>

The PropertyItem including PropertyItemName and PropertyMarketComponent

#### Namespace

Plenty\Modules\Item\Property\Models


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
            <td>The id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>unit</td>
            <td>The unit of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyGroupId</td>
            <td>The property group id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>imageName</td>
            <td>The image name of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendName</td>
            <td>The backend name of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueType</td>
            <td>The value type of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>searchable</td>
            <td>Indicates if the property item is searchable</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>orderProperty</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>showItem</td>
            <td>Indicates if the property item is shown</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>showItemList</td>
            <td>Indicates if the property item list is shown</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayCheckout</td>
            <td>Indicates if the checkout is displayed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayPdf</td>
            <td>Indicates if the pdf is displayed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>backendNote</td>
            <td>The backend note of the propety item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>surcharge</td>
            <td>The surcharge of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayAsAdditionalCosts</td>
            <td>Indicates if the property item is displayed as additional costs</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketComponents</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### PropertyItemName<a name="item_models_propertyitemname"></a>

The PropertyItemName including PropertyItem

#### Namespace

Plenty\Modules\Item\Property\Models


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
            <td>propertyItemId</td>
            <td>The id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the property item</td>
        </tr><tr>
            <td><a href="item#item_models_propertyitem">PropertyItem</a>
</td>
            <td>property</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### PropertyMarketComponent<a name="item_models_propertymarketcomponent"></a>

The PropertyMarketComponent including PropertyItem

#### Namespace

Plenty\Modules\Item\Property\Models


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
            <td>propertyItemId</td>
            <td>The id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>componentId</td>
            <td>The id of the component</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketReference</td>
            <td>The market reference of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalComponent</td>
            <td>The external component of the property</td>
        </tr><tr>
            <td><a href="item#item_models_propertyitem">PropertyItem</a>
</td>
            <td>property</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### PropertySelection<a name="item_models_propertyselection"></a>

The PropertySelection including PropertyItem

#### Namespace

Plenty\Modules\Item\Property\Models


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
            <td>The id of the property selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyItemId</td>
            <td>The id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The lang of the property selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the property selection</td>
        </tr><tr>
            <td><a href="item#item_models_propertyitem">PropertyItem</a>
</td>
            <td>property</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# SalesPrice<a name="item_salesprice"></a>
    
## Contracts<a name="item_salesprice_contracts"></a>
### SalesPriceRepositoryContract<a name="item_contracts_salespricerepositorycontract"></a>

sales price

#### Namespace

Plenty\Modules\Item\SalesPrice\Contracts



#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>
    
Show an VariationSalesPrice by given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>
    
Create new VariationSalesPrice
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>
    
Update an existing VariationSalesPrice
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Delete an VariationSalesPrice by given id. If at least one relation exists, throws an exception.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId):<a href="item#item_models_salesprice">SalesPrice</a>
</pre>
    
Get list of SalesPrices from type
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>
    
Get list of SalesPrices
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_salesprice_models"></a>
### SalesPrice<a name="item_models_salesprice"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>The id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>minimumOrderQuantity</td>
            <td>The minimum order quantity of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isCustomerPrice</td>
            <td>Indicates if the sales price is a customer price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isDisplayedByDefault</td>
            <td>Indicates if the sales price is displayed by default</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isLiveConversion</td>
            <td>Indicates if the sales price is live converted</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>name</td>
            <td>names</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>account</td>
            <td>accounts</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>country</td>
            <td>countries</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>currency</td>
            <td>currencies</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>customerClass</td>
            <td>customerClasses</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>referrer</td>
            <td>referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>onlineStore</td>
            <td>onlineStore</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceAccount<a name="item_models_salespriceaccount"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountType</td>
            <td>The account type of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountId</td>
            <td>The account id of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceCountry<a name="item_models_salespricecountry"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The country id of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceCurrency<a name="item_models_salespricecurrency"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currency</td>
            <td>The currency of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceCustomerClass<a name="item_models_salespricecustomerclass"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerClassId</td>
            <td>The customer class id of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceName<a name="item_models_salespricename"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The lang of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>nameInternal</td>
            <td>The internal name of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>nameExternal</td>
            <td>The external name of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceOnlineStore<a name="item_models_salespriceonlinestore"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The plenty id of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### SalesPriceReferrer<a name="item_models_salespricereferrer"></a>



#### Namespace

Plenty\Modules\Item\SalesPrice\Models


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
            <td>priceId</td>
            <td>The price id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>referrerId</td>
            <td>The referrer id of the sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# ShippingSupport<a name="item_shippingsupport"></a>
    
## Contracts<a name="item_shippingsupport_contracts"></a>
### ShippingSupportRepositoryContract<a name="item_contracts_shippingsupportrepositorycontract"></a>

Repository for ShippingSupport

#### Namespace

Plenty\Modules\Item\ShippingSupport\Contracts



#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_shippingsupport">ShippingSupport</a>
</pre>
    
Find one ShippingSupport by Id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_shippingsupport">ShippingSupport</a>
</pre>
    
Adds shipping support to article
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Remove shipping support to article
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_shippingsupport_models"></a>
### ShippingSupport<a name="item_models_shippingsupport"></a>

The shipping support model

#### Namespace

Plenty\Modules\Item\ShippingSupport\Models


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
            <td>The id of the shipping support</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The id of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>profileId</td>
            <td>The profile id of the shipping support</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Unit<a name="item_unit"></a>
    
## Contracts<a name="item_unit_contracts"></a>
### UnitNameRepositoryContract<a name="item_contracts_unitnamerepositorycontract"></a>

Repository for Unit Name

#### Namespace

Plenty\Modules\Item\Unit\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $unitId):<a href="item#item_models_unitname">UnitName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $unitId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $unitId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_unitname">UnitName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $unitId, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="item#item_models_unitname">UnitName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByUnitId</strong>(<a target="_blank" href="http://php.net/int">int</a> $unitId):<a href="item#item_models_unitname">UnitName</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$unitId</td>
        <td></td>
    </tr>
</table>



### UnitRepositoryContract<a name="item_contracts_unitrepositorycontract"></a>

Repository for Unit

#### Namespace

Plenty\Modules\Item\Unit\Contracts



#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_unit">Unit</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_unit">Unit</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="item#item_models_unit">Unit</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = [], <a target="_blank" href="http://php.net/int">int</a> $perPage = 50, <a target="_blank" href="http://php.net/int">int</a> $page = 1):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_unit_models"></a>
### Unit<a name="item_models_unit"></a>

The unit model including unit name

#### Namespace

Plenty\Modules\Item\Unit\Models


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
            <td>The id of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>unitOfMeasurement</td>
            <td>The unit of measurement of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>DecimalPlacesAllowed</td>
            <td>Declares if decimal places are allowed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The last updated date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>langs</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### UnitName<a name="item_models_unitname"></a>

The unit name model including the unit

#### Namespace

Plenty\Modules\Item\Unit\Models


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
            <td>unitId</td>
            <td>The id of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the unit</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the unit</td>
        </tr><tr>
            <td><a href="item#item_models_unit">Unit</a>
</td>
            <td>unit</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# Variation<a name="item_variation"></a>
    
## Contracts<a name="item_variation_contracts"></a>
### VariationRepositoryContract<a name="item_contracts_variationrepositorycontract"></a>

Repository for item basket

#### Namespace

Plenty\Modules\Item\Variation\Contracts



#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $with, <a target="_blank" href="http://php.net/string">string</a> $lang):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createPrimary</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variation">Variation</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_variation_models"></a>
### Variation<a name="item_models_variation"></a>

Variation

#### Namespace

Plenty\Modules\Item\Variation\Models


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
            <td>isActive</td>
            <td>Checks if the variation is active</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueSetId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>autoStockInvisible</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>autoStockNoStockIcon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>autoStockPositiveStockIcon</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>autoStockVisible</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>automaticClientVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>availability</td>
            <td>Checks the availability of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>availableUntil</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td>The created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customNumber</td>
            <td>The custom number of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>customsPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>estimatedAvailability</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>externalId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge1</td>
            <td>The extra shipping charge 1 of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>extraShippingCharge2</td>
            <td>The extra shipping charge 2 of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>heightMm</td>
            <td>The height in millimeter of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>intervalOrderQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td>The last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lengthMm</td>
            <td>The length in millimeter of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>limitOrderByStockSelect</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainWarehouse</td>
            <td>The main warehouse of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maximumOrderQuantity</td>
            <td>The minimum order quantity of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minimumOrderQuantity</td>
            <td>The maximum order quantity of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>model</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>operatingCostsPercent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>packingUnitType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>packingUnits</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentItemVariationQuantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>picking</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priceCalculationSetId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isMain</td>
            <td>Checks if the variation is a main variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mainVariationId</td>
            <td>The id of the main variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td>The purchase price of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relatedLastUpdateTimestamp</td>
            <td>The related last update date timestamp of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>releaseDate</td>
            <td>The release date of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>storageCosts</td>
            <td>The storage costs of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>transportationCosts</td>
            <td>The transportation costs of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitCombinationId</td>
            <td>The unit combination id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>unitLoadDevice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>unitsContained</td>
            <td>The amount of units contained for this variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationName</td>
            <td>The variation name of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>vatId</td>
            <td>The id of the tax rate of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightG</td>
            <td>The weight in grams of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>weightNetG</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>widthMm</td>
            <td>The width in millimeter of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationBarcodes</td>
            <td>barcodes</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSalesPrices</td>
            <td>salesPrices</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketItemNumbers</td>
            <td>marketItemNumbers</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationCategories</td>
            <td>Categories</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationClients</td>
            <td>Clients</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationMarkets</td>
            <td>Markets</td>
        </tr><tr>
            <td><a href="item#item_models_variationdefaultcategory">VariationDefaultCategory</a>
</td>
            <td>variationDefaultCategory</td>
            <td>DefaultCategory</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationSuppliers</td>
            <td>Suppliers</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>variationWarehouses</td>
            <td>Warehouses</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The item id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>clientVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>salesPriceVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>supplierVariationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseVariationId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationBarcode<a name="item_variationbarcode"></a>
    
## Models<a name="item_variationbarcode_models"></a>
### VariationBarcode<a name="item_models_variationbarcode"></a>

Variation Barcode

#### Namespace

Plenty\Modules\Item\VariationBarcode\Models


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
            <td>code</td>
            <td>The code of the variation's barcode. The combination of code and barcode ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>barcodeId</td>
            <td>The unique ID of the barcode linked to the variation. The combination of code and barcode ID must be unique.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The unique ID of the variation. The ID must be specified.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the code for the variation was created.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationCategory<a name="item_variationcategory"></a>
    
## Models<a name="item_variationcategory_models"></a>
### VariationCategory<a name="item_models_variationcategory"></a>

Variation Category

#### Namespace

Plenty\Modules\Item\VariationCategory\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryId</td>
            <td>The id of the category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the variation category</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isNeckermannPrimary</td>
            <td>Indicates if the variation category is ...</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationClient<a name="item_variationclient"></a>
    
## Models<a name="item_variationclient_models"></a>
### VariationClient<a name="item_models_variationclient"></a>

Variation Client

#### Namespace

Plenty\Modules\Item\VariationClient\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The id of the variation client</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The created at date timestamp</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationDefaultCategory<a name="item_variationdefaultcategory"></a>
    
## Models<a name="item_variationdefaultcategory_models"></a>
### VariationDefaultCategory<a name="item_models_variationdefaultcategory"></a>

Variation Default Category

#### Namespace

Plenty\Modules\Item\VariationDefaultCategory\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>branchId</td>
            <td>The id of the category branch</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The id of the client</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>manually</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationDescription<a name="item_variationdescription"></a>
    
## Models<a name="item_variationdescription_models"></a>
### VariationDescription<a name="item_models_variationdescription"></a>

Variation Default Category

#### Namespace

Plenty\Modules\Item\VariationDescription\Models


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
            <td>The ID of the description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The ID of the item the description belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The default name of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name2</td>
            <td>Alternative item name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name3</td>
            <td>Alternative item name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>previewDescription</td>
            <td>The preview description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaDescription</td>
            <td>The description for search engines</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The long description of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>technicalData</td>
            <td>The technical data of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlPath</td>
            <td>The URL of the item in the online store</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>metaKeywords</td>
            <td>Meta keywords for search engines</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationImage<a name="item_variationimage"></a>
    
## Models<a name="item_variationimage_models"></a>
### VariationImage<a name="item_models_variationimage"></a>



#### Namespace

Plenty\Modules\Item\VariationImage\Models


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
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>imageId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationMarket<a name="item_variationmarket"></a>
    
## Models<a name="item_variationmarket_models"></a>
### VariationMarket<a name="item_models_variationmarket"></a>

Variation Market

#### Namespace

Plenty\Modules\Item\VariationMarket\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>marketId</td>
            <td>The id of the market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The created at date timestamp</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationMarketIdentNumber<a name="item_variationmarketidentnumber"></a>
    
## Models<a name="item_variationmarketidentnumber_models"></a>
### VariationMarketIdentNumber<a name="item_models_variationmarketidentnumber"></a>

Variation Market Ident Number

#### Namespace

Plenty\Modules\Item\VariationMarketIdentNumber\Models


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
            <td>The id of the variation market ident number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>countryId</td>
            <td>The country id of the variation market ident number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the variation market ident number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the variation market ident number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the variation market ident number</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationProperty<a name="item_variationproperty"></a>
    
## Models<a name="item_variationproperty_models"></a>
### VariationProperty<a name="item_models_variationproperty"></a>

The VariationPropertyValue

#### Namespace

Plenty\Modules\Item\VariationProperty\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyItemId</td>
            <td>The id of the property item</td>
        </tr><tr>
            <td><a href="item#item_models_propertyitem">PropertyItem</a>
</td>
            <td>propertyItem</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationPropertyValue<a name="item_models_variationpropertyvalue"></a>

The VariationPropertyValue

#### Namespace

Plenty\Modules\Item\VariationProperty\Models


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
            <td>The id of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyItemId</td>
            <td>The id of the property item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertySelectionId</td>
            <td>The id of the property selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>valueInt</td>
            <td>The int value of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>valueFloat</td>
            <td>The float value of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>valueFile</td>
            <td>The file value of the variation property value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>surcharge</td>
            <td>The surcharge of the variation property value</td>
        </tr><tr>
            <td><a href="item#item_models_propertyitem">PropertyItem</a>
</td>
            <td>propertyItem</td>
            <td></td>
        </tr><tr>
            <td><a href="item#item_models_propertyselection">PropertySelection</a>
</td>
            <td>propertySelection</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationSalesPrice<a name="item_variationsalesprice"></a>
    
## Contracts<a name="item_variationsalesprice_contracts"></a>
### VariationSalesPriceRepositoryContract<a name="item_contracts_variationsalespricerepositorycontract"></a>

Repository for VariationSalesPrice

#### Namespace

Plenty\Modules\Item\VariationSalesPrice\Contracts



#### Methods

<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>
    
Show an VariationSalesPrice by given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>
    
Create new VariationSalesPrice
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>
    
Update an existing VariationSalesPrice
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $salesPriceId, <a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>
    
Delete an VariationSalesPrice by given id. If at least one relation exists, throws an exception.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$salesPriceId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>
    
Find an existing VariationSalesPrice by given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByVariationIdWithInheritance</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a href="item#item_models_variationsalesprice">VariationSalesPrice</a>
</pre>
    
Find an existing VariationSalesPrice by given id.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_variationsalesprice_models"></a>
### VariationSalesPrice<a name="item_models_variationsalesprice"></a>

VariationSalesPrice

#### Namespace

Plenty\Modules\Item\VariationSalesPrice\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>salesPriceId</td>
            <td>The id of the sales price</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>price</td>
            <td>The price of the variation sales price</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationSku<a name="item_variationsku"></a>
    
## Contracts<a name="item_variationsku_contracts"></a>
### VariationSkuRepositoryContract<a name="item_contracts_variationskurepositorycontract"></a>

Repository for VariationSku

#### Namespace

Plenty\Modules\Item\VariationSku\Contracts



#### Methods

<pre>public <strong>generateSku</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $marketId, <a target="_blank" href="http://php.net/int">int</a> $accountId, $sku = null, <a target="_blank" href="http://php.net/bool">bool</a> $setLastExportedTimestamp = true):<a target="_blank" href="http://php.net/string">string</a></pre>
    
Generate or update Sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$marketId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$accountId</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$sku</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$setLastExportedTimestamp</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationsku">VariationSku</a>
</pre>
    
Create sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $skuId):<a href="item#item_models_variationsku">VariationSku</a>
</pre>
    
Update sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$skuId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/int">int</a> $skuId):<a href="miscellaneous#miscellaneous_models_deleteresponse">DeleteResponse</a>
</pre>
    
Delete sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$skuId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/int">int</a> $skuId):<a href="item#item_models_variationsku">VariationSku</a>
</pre>
    
Show sku
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$skuId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>search</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Search sku´s
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Find sku´s by variationId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_variationsku_models"></a>
### VariationSku<a name="item_models_variationsku"></a>

The variationSku model

#### Namespace

Plenty\Modules\Item\VariationSku\Models


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
            <td>The row id of the table plenty_item_variation_market_status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The id of the variation.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>marketId</td>
            <td>The id of the marketplace.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>accountId</td>
            <td>The id of the marketplace account.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>initialSku</td>
            <td>The initial SKU of the variation. The initial SKU can not be modified even if you make changes to the variation SKU. It is possible, however, to reset the variation SKU to the initial SKU.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationSku</td>
            <td>The SKU of the variation. The SKU is adjustable but may not exist twice for the combination maketId and acoountId.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>active</td>
            <td>Flag that indicates if the item is ready for export (currently not in use).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdTimestamp</td>
            <td>The time the SKU was created (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastExportTimestamp</td>
            <td>The time the variation was last exported (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deletedTimestamp</td>
            <td>The time the variation was deleted (YYYY-MM-DD HH:MM:SS).</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>status</td>
            <td>The status of the variation after the export. Possible entries are INACTIVE, SEND and ACTIVE.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>additionalInformation</td>
            <td>The field that contains additional information.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationStock<a name="item_variationstock"></a>
    
## Contracts<a name="item_variationstock_contracts"></a>
### VariationStockRepositoryContract<a name="item_contracts_variationstockrepositorycontract"></a>



#### Namespace

Plenty\Modules\Item\VariationStock\Contracts



#### Methods

<pre>public <strong>searchByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $rowCount = 50, <a target="_blank" href="http://php.net/int">int</a> $offset):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Find Stock by given Variation id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowCount</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>searchStorageLocationsByVariationId</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/array">array</a> $params):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Find all storage locations by given warehouse id
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>intake</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationstock">VariationStock</a>
</pre>
    
Stock intake
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>correction</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="item#item_models_variationstock">VariationStock</a>
</pre>
    
Stock Correction
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>movement</strong>(<a target="_blank" href="http://php.net/int">int</a> $variationId, <a target="_blank" href="http://php.net/int">int</a> $rowCount = 50, <a target="_blank" href="http://php.net/int">int</a> $offset):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$variationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowCount</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$offset</td>
        <td></td>
    </tr>
</table>


## Models<a name="item_variationstock_models"></a>
### VariationStock<a name="item_models_variationstock"></a>



#### Namespace

Plenty\Modules\Item\VariationStock\Models


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
            <td>itemName</td>
            <td>The item name of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flag1</td>
            <td>The flag 1 of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>flag2</td>
            <td>The flag 2 of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isBundle</td>
            <td>Checks if the variation is a bundle</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>attributeSelection</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>customNumber</td>
            <td>The custom number of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>barcode</td>
            <td>The barcode of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>availability</td>
            <td>Checks the availability of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedListing</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedBundles</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>valueOfGoods</td>
            <td>The value of the goods in the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>purchasePrice</td>
            <td>The purchase price of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The id of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The id of the item</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueSetId</td>
            <td>The attribute value set id of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>physicalStock</td>
            <td>The physical stock of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reservedStock</td>
            <td>The reserved stock of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>netStock</td>
            <td>The actual available stock of the variation stock</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reordered</td>
            <td>The reordered</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>reorderDelta</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reorderLevel</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### VariationStockMovement<a name="item_models_variationstockmovement"></a>



#### Namespace

Plenty\Modules\Item\VariationStock\Models


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
            <td>sourceString</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>reasonString</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>attributeSelection</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>warehouseName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>variationNumber</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>processRowId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeValueSet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantity</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reason</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>entryDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sourceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>processRowType</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>purchasePrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>errorCode</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationSupplier<a name="item_variationsupplier"></a>
    
## Models<a name="item_variationsupplier_models"></a>
### VariationSupplier<a name="item_models_variationsupplier"></a>

Variation Supplier

#### Namespace

Plenty\Modules\Item\VariationSupplier\Models


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
            <td>The id of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>supplierId</td>
            <td>The id of the supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>purchasePrice</td>
            <td>The purchase price of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minimumOrderValue</td>
            <td>The minimum order value of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemNumber</td>
            <td>The item number of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastPriceQuery</td>
            <td>The last price of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deliveryTimeInDays</td>
            <td>The delivery time in days of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>discount</td>
            <td>The discount of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>discountable</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/double">double</a></td>
            <td>packagingUnit</td>
            <td>The packaging unit of the variation supplier</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td>The last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The created at date timestamp</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
# VariationWarehouse<a name="item_variationwarehouse"></a>
    
## Models<a name="item_variationwarehouse_models"></a>
### VariationWarehouse<a name="item_models_variationwarehouse"></a>

Variation Warehouse

#### Namespace

Plenty\Modules\Item\VariationWarehouse\Models


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
            <td>variationId</td>
            <td>The id of the variation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseId</td>
            <td>The id of the warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>warehouseZoneId</td>
            <td>The id of the warehouse zone</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storageLocationType</td>
            <td>The storage location type of the variation warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reorderLevel</td>
            <td>The reorder level of the variation warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maximumStock</td>
            <td>The maximum stock of the variation warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockTurnoverInDays</td>
            <td>The stock turnover in days of the variation warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>storageLocation</td>
            <td>The storage location of the variation warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>stockBuffer</td>
            <td>The stock buffer of the variation warehouse</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateTimestamp</td>
            <td>The last update date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The created at date timestamp</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
