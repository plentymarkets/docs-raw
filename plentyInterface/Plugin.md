

# DataBase<a name="plugin_database"></a>
    
## Contracts<a name="plugin_database_contracts"></a>
### DataBase<a name="plugin_contracts_database"></a>

Database contract


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`



#### Methods

<pre>public <strong>save</strong>(<a href="plugin#plugin_contracts_model">Model</a>
 $model):<a href="plugin#plugin_contracts_model">Model</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="plugin#plugin_contracts_model">Model</a>
</td>
        <td>$model</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName, $primaryKeyFieldValue):<a href="plugin#plugin_contracts_model">Model</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$primaryKeyFieldValue</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>query</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName):<a href="plugin#plugin_contracts_query">Query</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a href="plugin#plugin_contracts_model">Model</a>
 $model):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="plugin#plugin_contracts_model">Model</a>
</td>
        <td>$model</td>
        <td></td>
    </tr>
</table>



### Migrate<a name="plugin_contracts_migrate"></a>

Migrate models


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`



#### Methods

<pre>public <strong>createTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 10, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 20):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$readCapacityUnits</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$writeCapacityUnits</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
        <td></td>
    </tr>
</table>



### Model<a name="plugin_contracts_model"></a>

Database model


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`


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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>primaryKeyFieldName</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>primaryKeyFieldType</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>autoIncrementPrimaryKey</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>textFields</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>getTableName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### Query<a name="plugin_contracts_query"></a>

database query


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`



#### Methods

<pre>public <strong>where</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhere</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# DynamoDb<a name="plugin_dynamodb"></a>
    
## Contracts<a name="plugin_dynamodb_contracts"></a>
### DynamoDbRepositoryContract<a name="plugin_contracts_dynamodbrepositorycontract"></a>

AWS DynamoDb Repository


#### Namespace

`Plenty\Modules\Plugin\DynamoDb\Contracts`



#### Methods

<pre>public <strong>createTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $attributeDefinitions, <a target="_blank" href="http://php.net/array">array</a> $keySchema, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 3, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 2):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>

    
Create a table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$attributeDefinitions</td>
        <td>http://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_AttributeValue.html</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$keySchema</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$readCapacityUnits</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$writeCapacityUnits</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 3, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 2):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>

    
Update a table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$readCapacityUnits</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$writeCapacityUnits</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>putItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $item):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>

    
Add item to table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$item</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/boolean">boolean</a> $consistentRead, <a target="_blank" href="http://php.net/array">array</a> $key):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Retrieving items
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$consistentRead</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete an item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$key</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>

    
Deleting a table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>scan</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/string">string</a> $returnFields = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $expressionAttributeValues = [], <a target="_blank" href="http://php.net/string">string</a> $filterExpression = &quot;&quot;, <a target="_blank" href="http://php.net/int">int</a> $limit):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
A scan operation scans the entire table. You can specify filters to apply to the results to refine the values returned to you, after the complete scan. Amazon DynamoDB puts a 1MB limit on the scan (the limit applies before the results are filtered).
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$returnFields</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$expressionAttributeValues</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filterExpression</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$limit</td>
        <td>is taken into account when value greater than 0</td>
    </tr>
</table>


# Libs<a name="plugin_libs"></a>
    
## Contracts<a name="plugin_libs_contracts"></a>
### LibraryCallContract<a name="plugin_contracts_librarycallcontract"></a>

library call


#### Namespace

`Plenty\Modules\Plugin\Libs\Contracts`



#### Methods

<pre>public <strong>call</strong>(<a target="_blank" href="http://php.net/string">string</a> $libCall, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$libCall</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
</table>


# Storage<a name="plugin_storage"></a>
    
## Contracts<a name="plugin_storage_contracts"></a>
### StorageRepositoryContract<a name="plugin_contracts_storagerepositorycontract"></a>

Storage Repository


#### Namespace

`Plenty\Modules\Plugin\Storage\Contracts`



#### Methods

<pre>public <strong>uploadFile</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/string">string</a> $pathToFile, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false, <a target="_blank" href="http://php.net/array">array</a> $metaData = []):<a href="cloud#cloud_models_storageobject">StorageObject</a>
</pre>

    
Upload an object by streaming the contents of a file $pathToFile should be absolute path to a file on disk
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>e.g. myDir/x/y/z/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pathToFile</td>
        <td>absolute path to a file on disk</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$metaData</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>uploadObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/string">string</a> $body, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false, <a target="_blank" href="http://php.net/array">array</a> $metaData = []):<a href="cloud#cloud_models_storageobject">StorageObject</a>
</pre>

    
Create an object with content in $body
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>e.g. myDir/x/y/z/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$body</td>
        <td>file content</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$metaData</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false):<a href="cloud#cloud_models_storageobject">StorageObject</a>
</pre>

    
Get an object
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>e.g. myDir/x/y/z/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getObjectUrl</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false, <a target="_blank" href="http://php.net/int">int</a> $minutesToExpire = 5):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Returns the URL to an object identified by its bucket and key. The URL will be signed and set to expire at the provided time.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>e.g. myDir/x/y/z/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$minutesToExpire</td>
        <td>Minutes between 1 and 15</td>
    </tr>
</table>


<pre>public <strong>getObjectAsTemporaryFileResource</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get local file resource of an object. Use this if it is really necessary! Using getObject is the normal and effective way.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>e.g. myDir/x/y/z/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/boolean">boolean</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>doesObjectExist</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks if object exists
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>e.g. myDir/x/y/z/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>

    
Executes the DeleteObject operation.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td>myDir/HelloWorld.txt</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listObjects</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $prefix = &quot;&quot;, <a target="_blank" href="http://php.net/int">int</a> $limit, <a target="_blank" href="http://php.net/string">string</a> $startKey = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $continuationToken = &quot;&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false, <a target="_blank" href="http://php.net/bool">bool</a> $resultKeyWithoutPrefix = true):<a href="cloud#cloud_models_storageobjectlist">StorageObjectList</a>
</pre>

    
Returns some or all (up to 1000) objects
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td>name of your plugin</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$prefix</td>
        <td>Limits the response to keys that begin with the specified prefix.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$limit</td>
        <td>The total number of items to return.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$startKey</td>
        <td>is where you want to start listing from. $startKey can be any key in the bucket.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$continuationToken</td>
        <td>indicates that the list is being continued on this bucket with a token.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$resultKeyWithoutPrefix</td>
        <td></td>
    </tr>
</table>


