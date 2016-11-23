

# DynamoDb<a name="cloud_dynamodb"></a>
    
## Contracts<a name="cloud_dynamodb_contracts"></a>
### DynamoDbRepositoryContract<a name="cloud_contracts_dynamodbrepositorycontract"></a>

Used for interaction with DynamoDB

#### Namespace

`Plenty\Modules\Cloud\DynamoDb\Contracts`



#### Methods

<pre>public <strong>createTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $attributeDefinitions, <a target="_blank" href="http://php.net/array">array</a> $keySchema, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 3, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 2):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Create a table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td>The name of the table to create</td>
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


<pre>public <strong>updateTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 3, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 2):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Update a table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>putItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $item):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Add item to table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>getItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/boolean">boolean</a> $consistentRead, <a target="_blank" href="http://php.net/array">array</a> $key):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Retrieving items
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>deleteItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $key):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Delete an item
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


<pre>public <strong>deleteTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Deleting a table
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>scan</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/string">string</a> $returnFields = &quot;&quot;, <a target="_blank" href="http://php.net/array">array</a> $expressionAttributeValues = [], <a target="_blank" href="http://php.net/string">string</a> $filterExpression = &quot;&quot;, <a target="_blank" href="http://php.net/int">int</a> $limit):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    
A scan operation scans the entire table. You can specify filters to apply to the results to refine the values
returned to you, after the complete scan. Amazon DynamoDB puts a 1MB limit on the scan (the limit applies before
the results are filtered).
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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


# Storage<a name="cloud_storage"></a>
    
## Contracts<a name="cloud_storage_contracts"></a>
### StorageRepositoryContract<a name="cloud_contracts_storagerepositorycontract"></a>

Store files on amazon S3

#### Namespace

`Plenty\Modules\Cloud\Storage\Contracts`



#### Methods

<pre>public <strong>uploadFile</strong>(<a target="_blank" href="http://php.net/string">string</a> $bucket, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/string">string</a> $pathToFile, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false, <a target="_blank" href="http://php.net/array">array</a> $metaData = []):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Upload an object by streaming the contents of a file $pathToFile should be absolute path to a file on disk
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$bucket</td>
        <td>e.g. plentymarkets-documents | plentymarkets-items | plentymarkets-plugins</td>
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


<pre>public <strong>uploadObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $bucket, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/string">string</a> $body, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false, <a target="_blank" href="http://php.net/array">array</a> $metaData = []):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Create an object with content in $body
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$bucket</td>
        <td>e.g. plentymarkets-documents | plentymarkets-items | plentymarkets-plugins</td>
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


<pre>public <strong>getObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $bucket, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false):<a target="_blank" href="http://php.net/array">array</a></pre>
    
Get an object from FS
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$bucket</td>
        <td>e.g. plentymarkets-documents | plentymarkets-items | plentymarkets-plugins</td>
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


<pre>public <strong>getObjectAsTemporaryFileResource</strong>(<a target="_blank" href="http://php.net/string">string</a> $bucket, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/boolean">boolean</a> $publicVisible = false):<a target="_blank" href="http://php.net/string">string</a></pre>
    
Get local file resource of an object. Use this if it is really necessary! Using getObject is the normal and effective way.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$bucket</td>
        <td>e.g. plentymarkets-documents | plentymarkets-items | plentymarkets-plugins</td>
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


<pre>public <strong>doesObjectExist</strong>(<a target="_blank" href="http://php.net/string">string</a> $bucket, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Checks if object exists
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$bucket</td>
        <td>e.g. plentymarkets-documents | plentymarkets-items | plentymarkets-plugins</td>
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


<pre>public <strong>deleteObjects</strong>(<a target="_blank" href="http://php.net/string">string</a> $bucket, <a target="_blank" href="http://php.net/array">array</a> $keyList, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a target="_blank" href="http://php.net/boolean">boolean</a></pre>
    
Executes the DeleteObjects operation. You may specify up to 1000 keys.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$bucket</td>
        <td>e.g. plentymarkets-documents | plentymarkets-items | plentymarkets-plugins</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$keyList</td>
        <td>[[Key => myDir/HelloWorld.txt], ...]</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
</table>


