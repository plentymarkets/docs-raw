

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


<pre>public <strong>query</strong>(<a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $queryParams):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$tableName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$queryParams</td>
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
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>getTableName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>
    

    
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


