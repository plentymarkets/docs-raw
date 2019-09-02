

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
        <td>This field is deprecated and will be removed soon</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$writeCapacityUnits</td>
        <td>This field is deprecated and will be removed soon</td>
    </tr>
</table>


<pre>public <strong>updateTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelClassName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelClassName</td>
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

    

    

### JoinClauseQuery<a name="plugin_contracts_joinclausequery"></a>

database join query


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`





#### Methods

<pre>public <strong>on</strong>(<a target="_blank" href="http://php.net/string">string</a> $firstModelName, $first, <a target="_blank" href="http://php.net/string">string</a> $operator = null, <a target="_blank" href="http://php.net/string">string</a> $secondModelName = null, <a target="_blank" href="http://php.net/string">string</a> $second = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$firstModelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$first</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$secondModelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$second</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>where</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelName, $column, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a basic where clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$column</td>
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
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhere</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelName, $column, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$column</td>
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


<pre>public <strong>whereNull</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelName, $column, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $not = false):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where null&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$column</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$not</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhereNull</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelName, $column):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where null&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$column</td>
        <td></td>
    </tr>
</table>



### Query<a name="plugin_contracts_query"></a>

database query


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`





#### Methods

<pre>public <strong>select</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a basic select clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>where</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a basic where clause to the query.
    
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


<pre>public <strong>whereIn</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $not = false):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where in&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$not</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhereIn</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/array">array</a> $values):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where in&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhere</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where&quot; clause to the query.
    
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


<pre>public <strong>whereNull</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $not = false):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where null&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$not</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhereNull</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where null&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereBetween</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $not = false):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a where between statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$not</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereNotBetween</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a where not between statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereDate</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $operator, $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where date&quot; statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
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
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereMonth</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $operator, $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where month&quot; statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
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
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereDay</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $operator, $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where day&quot; statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
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
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereYear</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $operator, $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where year&quot; statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
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
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereTime</strong>(<a target="_blank" href="http://php.net/string">string</a> $column, <a target="_blank" href="http://php.net/string">string</a> $operator, <a target="_blank" href="http://php.net/int">int</a> $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where time&quot; statement to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$column</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>having</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, <a target="_blank" href="http://php.net/string">string</a> $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;having&quot; clause to the query.
    
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
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orHaving</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, <a target="_blank" href="http://php.net/string">string</a> $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;or having&quot; clause to the query.
    
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
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orderBy</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $direction = &quot;asc&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;order by&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$direction</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>forPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $perPage = 15):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Set the limit and offset for a given page.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$perPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>count</strong>(<a target="_blank" href="http://php.net/string">string</a> $columns = &quot;*&quot;):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Retrieve the &quot;count&quot; result of the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>limit</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Set the &quot;limit&quot; value of the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>offset</strong>(<a target="_blank" href="http://php.net/int">int</a> $value):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Set the &quot;offset&quot; value of the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCountForPagination</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the count of the total records for the paginator.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>delete</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    

### CriteriaQuery<a name="plugin_contracts_criteriaquery"></a>

database query


#### Namespace

`Plenty\Modules\Plugin\DataBase\Contracts`





#### Methods

<pre>public <strong>where</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a basic where clause to the query.
    
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


<pre>public <strong>whereIn</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/array">array</a> $values, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $not = false):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where in&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$not</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhereIn</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/array">array</a> $values):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where in&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$values</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhere</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, $value = null):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add an &quot;or where&quot; clause to the query.
    
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


<pre>public <strong>whereNull</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;, <a target="_blank" href="http://php.net/bool">bool</a> $not = false):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;where null&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$not</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orWhereNull</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Add an &quot;or where null&quot; clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fieldName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>having</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, <a target="_blank" href="http://php.net/string">string</a> $value = null, <a target="_blank" href="http://php.net/string">string</a> $boolean = &quot;and&quot;):<a href="plugin#plugin_database_contracts">Contracts</a>
</pre>

    
Add a &quot;having&quot; clause to the query.
    
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
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boolean</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>orHaving</strong>(<a target="_blank" href="http://php.net/string">string</a> $fieldName, <a target="_blank" href="http://php.net/string">string</a> $operator = null, <a target="_blank" href="http://php.net/string">string</a> $value = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Add a &quot;or having&quot; clause to the query.
    
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
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>whereHas</strong>(<a target="_blank" href="http://php.net/string">string</a> $modelName, $callback = null, <a target="_blank" href="http://php.net/string">string</a> $operator = &quot;&gt;=&quot;, <a target="_blank" href="http://php.net/int">int</a> $count = 1):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$modelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$callback</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$operator</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$count</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>join</strong>(<a target="_blank" href="http://php.net/string">string</a> $firstModelName, $callback, <a target="_blank" href="http://php.net/string">string</a> $as = &quot;&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Add a join clause to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$firstModelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$callback</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$as</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>leftJoin</strong>(<a target="_blank" href="http://php.net/string">string</a> $firstModelName, $callback):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Add a left join to the query.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$firstModelName</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$callback</td>
        <td></td>
    </tr>
</table>


## Annotations<a name="plugin_database_annotations"></a>
### Relation<a name="plugin_annotations_relation"></a>




#### Namespace

`Plenty\Modules\Plugin\DataBase\Annotations`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Index<a name="plugin_annotations_index"></a>




#### Namespace

`Plenty\Modules\Plugin\DataBase\Annotations`





#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# PluginSet<a name="plugin_pluginset"></a>
    
## Contracts<a name="plugin_pluginset_contracts"></a>
### PluginSetRepositoryContract<a name="plugin_contracts_pluginsetrepositorycontract"></a>

list, create, update or delete plugin sets


#### Namespace

`Plenty\Modules\Plugin\PluginSet\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="plugin#plugin_models_pluginset">PluginSet</a>
</pre>

    
Create a plugin set. The data array has to contain a &#039;name&#039; field. Throws a &#039;TooManyPluginSetsException&#039; if the maximum number of sets is exceeded.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data for the newly created plugin set. Only the 'name' field is required: ['name' => 'MyNewPluginSet'].</td>
    </tr>
</table>


<pre>public <strong>copy</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="plugin#plugin_models_pluginset">PluginSet</a>
</pre>

    
Copy a plugin set. All set entries from the source set will be copied into the new set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Has to contain the Id of the plugin set to copy from and the name for the new set: ['copyPluginSetId' => 12, 'name' =>
'NewSetWithCopiedEntries'].</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Update a set. Only the &#039;name&#039; field can be updated.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>Id of the plugin set to update</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Update data must only contain a 'name' field: ['name' => 'NewNameForMySet']</td>
    </tr>
</table>


<pre>public <strong>delete</strong>($what):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Delete a set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$what</td>
        <td>The PluginSet object to delete or a PluginSet-Id</td>
    </tr>
</table>


<pre>public <strong>get</strong>($pluginSetOrId):<a href="plugin#plugin_models_pluginset">PluginSet</a>
</pre>

    
Get a plugin set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$pluginSetOrId</td>
        <td>The Id of the plugin set to retrieve from the database. If a PluginSet object is passed instead of an integer, the
object is returned without change.</td>
    </tr>
</table>


<pre>public <strong>list</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List all plugin sets.
    
<pre>public <strong>listSetEntries</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List all set entries of a plugin set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The Id of the plugin set to list the entries from.</td>
    </tr>
</table>


<pre>public <strong>listWebstores</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List all webstores a plugin set is related to.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The Id of the set in question</td>
    </tr>
</table>


<pre>public <strong>listLayoutContainers</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
List all LayoutContainers for a plugin set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The Id of the plugin set in question</td>
    </tr>
</table>


<pre>public <strong>getOrCreatePluginSetEntry</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/bool">bool</a> $withTrashed = false):<a href="plugin#plugin_models_pluginsetentry">PluginSetEntry</a>
</pre>

    
Get the PluginSetEntry object containing a specific plugin for a set. If a PluginSetEntry does not exist, it will be created.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The Id of the plugin set in question</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td>The Id of the plugin in question</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$withTrashed</td>
        <td>If true, deleted PluginSetEntires will be included. Default is false.</td>
    </tr>
</table>


<pre>public <strong>changePluginActiveStatusForSet</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/bool">bool</a> $active):<a href="plugin#plugin_models_plugin">Plugin</a>
</pre>

    
Activates / deactivates a plugin for a set by trashing or restoring the respective set entry.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>The id of the plugin set in question</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td>The id of the plugin in question</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$active</td>
        <td>true if the plugin should be activated for the set, false if it should be deactivated.</td>
    </tr>
</table>


<pre>public <strong>removePluginFromSet</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $pluginId):<a href="plugin#plugin_models_plugin">Plugin</a>
</pre>

    
Remove a plugin from a set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td>The Id of the plugin set in question</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td>The Id of the plugin that should be removed from the set.</td>
    </tr>
</table>


<pre>public <strong>createPreviewHash</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Create a preview hash for a plugin set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td>The plugin set in question</td>
    </tr>
</table>


<pre>public <strong>getPreviewPluginSetId</strong>(<a target="_blank" href="http://php.net/string">string</a> $previewHash):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Extract a plugin set id from a preview hash.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$previewHash</td>
        <td>The preview has to extract the plugin set id from</td>
    </tr>
</table>


<pre>public <strong>installGitPlugin</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/array">array</a> $requestData):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Install a git-plugin into a set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td>The Id of the plugin set to install the plugin into</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td>The Id of the (git-) plugin that should be installed into the set</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$requestData</td>
        <td>Must contain a 'branch' field that specifies the branch that should be installed: ['branch' => 'stable']</td>
    </tr>
</table>


<pre>public <strong>setPosition</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/array">array</a> $requestData):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Change the position of a plugin in a set
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td>The id of the plugin set in question</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td>The id of the plugin of which the position should be changed</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$requestData</td>
        <td>Must contain a 'position' field with an integer specifying the new position: ['position' => 99]</td>
    </tr>
</table>


<pre>public <strong>getSyncState</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Get the sync state, to determine if Plugins have been (de-)activated since last build.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>The id of the PluginSet</td>
    </tr>
</table>


<pre>public <strong>getPluginSetHash</strong>($pluginSetOrId):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$pluginSetOrId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPluginSetIdFromHash</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginSetHash):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginSetHash</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getCurrentPluginSetId</strong>():<a target="_blank" href="http://php.net/int">int</a></pre>

    
Get the PluginSetID of the currently running plugin.
    

### PluginSetEntryRepositoryContract<a name="plugin_contracts_pluginsetentryrepositorycontract"></a>

get, create, update or delete plugin set entries


#### Namespace

`Plenty\Modules\Plugin\PluginSet\Contracts`





#### Methods

<pre>public <strong>get</strong>($idOrInstance):<a href="plugin#plugin_models_pluginsetentry">PluginSetEntry</a>
</pre>

    
Get a PluginSetEntry.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$idOrInstance</td>
        <td>The Id of the PluginSetEntry to retrieve or the PluginSetEntry object itself.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="plugin#plugin_models_pluginsetentry">PluginSetEntry</a>
</pre>

    
Create a set entry.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Must contain a 'pluginId' field and a 'pluginSetId' field to specify which plugin should be associated with which plugin set in the
newly created set entry: ['pluginId' => 5, 'pluginSetId' => 3]</td>
    </tr>
</table>


<pre>public <strong>copyToPluginSet</strong>($pluginSetEntryOrId, $pluginSetOrId, <a target="_blank" href="http://php.net/bool">bool</a> $copyConfigurations):<a href="plugin#plugin_models_pluginsetentry">PluginSetEntry</a>
</pre>

    
Copy a PluginSetEntry to a PluginSet
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$pluginSetEntryOrId</td>
        <td>The id of the PluginSetEntry that should be copied, or the PluginSetEntry object itself</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$pluginSetOrId</td>
        <td>The id of the PluginSet the entry should be copied to, or the PluginSet object itself</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$copyConfigurations</td>
        <td>true if the configurations related to the set entry should also be copied, false if not</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Update a PluginSetEntry. Associate a set entry with a new set, a new plugin, or both.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The id of the set entry to update</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Must contain EITHER a 'pluginId' field OR a 'pluginSetId' field OR both.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>($what):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Delete a PluginSetEntry
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$what</td>
        <td>The PluginSetEntry object to delete or a PluginSetEntry-Id</td>
    </tr>
</table>


## Models<a name="plugin_pluginset_models"></a>
### PluginSet<a name="plugin_models_pluginset"></a>

Eloquent model representing a PluginSet.


#### Namespace

`Plenty\Modules\Plugin\PluginSet\Models`




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
            <td>hash</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentPluginSetId</td>
            <td></td>
        </tr><tr>
            <td><a href="plugin#plugin_models_pluginset">PluginSet</a>
</td>
            <td>parentPluginSet</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>pluginSetEntries</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>pluginSetEntriesWithTrashed</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>layoutContainers</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>webstores</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PluginSetEntry<a name="plugin_models_pluginsetentry"></a>

Eloquent model representing a PluginSetEntry.


#### Namespace

`Plenty\Modules\Plugin\PluginSet\Models`




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
            <td>pluginId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pluginSetId</td>
            <td></td>
        </tr><tr>
            <td><a href="plugin#plugin_models_plugin">Plugin</a>
</td>
            <td>plugin</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>branchName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>commit</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
# Plugin<a name="plugin_plugin"></a>
    
## Contracts<a name="plugin_plugin_contracts"></a>
### PluginRepositoryContract<a name="plugin_contracts_pluginrepositorycontract"></a>

Search plugins according to parameters


#### Namespace

`Plenty\Modules\Plugin\Contracts`





#### Methods

<pre>public <strong>searchPlugins</strong>(<a target="_blank" href="http://php.net/array">array</a> $params = [], <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = \Plenty\Modules\Plugin\Models\Plugin::DEFAULT_ITEMS_PER_PAGE):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Search plugins using filters. Example: searchPlugins([&#039;name&#039; =&gt; &#039;PluginIWantToFind&#039;])
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPluginSets</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isActiveInPluginSet</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isActiveInPluginSetByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isActiveInWebstore</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/int">int</a> $webstoreId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isActiveInWebstoreByPluginName</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/int">int</a> $webstoreId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>decoratePlugin</strong>(<a href="plugin#plugin_models_plugin">Plugin</a>
 $plugin, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId = null):<a href="plugin#plugin_models_plugin">Plugin</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="plugin#plugin_models_plugin">Plugin</a>
</td>
        <td>$plugin</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>



### PluginLayoutContainerRepositoryContract<a name="plugin_contracts_pluginlayoutcontainerrepositorycontract"></a>

Plugin layout container


#### Namespace

`Plenty\Modules\Plugin\Contracts`





#### Methods

<pre>public <strong>all</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateAll</strong>(<a target="_blank" href="http://php.net/array">array</a> $dataList, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$dataList</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getActiveLinkedLayoutContainers</strong>(<a target="_blank" href="http://php.net/array">array</a> $activeContainerKeysList, <a target="_blank" href="http://php.net/array">array</a> $activeDataProviderKeysList, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$activeContainerKeysList</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$activeDataProviderKeysList</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getActiveLinkedLayoutContainersByPluginSetId</strong>(<a target="_blank" href="http://php.net/array">array</a> $activeContainerKeysList, <a target="_blank" href="http://php.net/array">array</a> $activeDataProviderKeysList, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$activeContainerKeysList</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$activeDataProviderKeysList</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addNew</strong>(<a target="_blank" href="http://php.net/array">array</a> $dataList, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$dataList</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/string">string</a> $containerKey, <a target="_blank" href="http://php.net/string">string</a> $dataProviderKey, <a target="_blank" href="http://php.net/int">int</a> $containerPluginId = null, <a target="_blank" href="http://php.net/int">int</a> $dataProviderPluginId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$containerKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$dataProviderKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$containerPluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$dataProviderPluginId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>removeOne</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/string">string</a> $containerKey, <a target="_blank" href="http://php.net/string">string</a> $dataProviderKey, <a target="_blank" href="http://php.net/int">int</a> $containerPluginId = null, <a target="_blank" href="http://php.net/int">int</a> $dataProviderPluginId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$containerKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$dataProviderKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$containerPluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$dataProviderPluginId</td>
        <td></td>
    </tr>
</table>



### ConfigurationRepositoryContract<a name="plugin_contracts_configurationrepositorycontract"></a>

Save config values for plugins


#### Namespace

`Plenty\Modules\Plugin\Contracts`





#### Methods

<pre>public <strong>saveConfiguration</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/array">array</a> $configMap, <a target="_blank" href="http://php.net/int">int</a> $setId = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$configMap</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>copyToPluginSetEntry</strong>($configurationOrId, $pluginSetEntryOrId):<a target="_blank" href="http://php.net/int">int</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$configurationOrId</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$pluginSetEntryOrId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getConfigurationFile</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginId, <a target="_blank" href="http://php.net/int">int</a> $setId):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>export</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/int">int</a> $pluginId = null, <a target="_blank" href="http://php.net/bool">bool</a> $active = null):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$active</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>import</strong>(<a target="_blank" href="http://php.net/int">int</a> $setId, <a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $pluginId = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$setId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginId</td>
        <td></td>
    </tr>
</table>


## Models<a name="plugin_plugin_models"></a>
### Plugin<a name="plugin_models_plugin"></a>

Eloquent model representing a Plugin.


#### Namespace

`Plenty\Modules\Plugin\Models`




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
            <td>The ID of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the plugin. The position is used to determine the plugin
order.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>activeStage</td>
            <td>Shows whether the plugin is active in Stage. Inactive plugins will not
be provisioned in Stage.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>activeProductive</td>
            <td>Shows whether the plugin is active in Productive. Inactive plugins will
not be provisioned in Productive.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>created_at</td>
            <td>The date that the plugin was created.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updated_at</td>
            <td>The date that the plugin was updated last.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>inStage</td>
            <td>Shows whether the plugin is provisioned in Stage.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>inProductive</td>
            <td>Shows whether the plugin is provisioned in Productive.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isConnectedWithGit</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>updateInformation</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the plugin. The following plugin types are available:
<ul>
    <li>Template</li>
    <li>Export</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>installed</td>
            <td>Whether or not the plugin is installed. This will be false for plugins
that have been purchased from the marketplace but have not yet been installed in any set.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>version</td>
            <td>The version of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>versionStage</td>
            <td>The version of the plugin in stage</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>versionProductive</td>
            <td>The version of the plugin in productive</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketplaceVariations</td>
            <td>A list of available marketplace versions</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description text of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>namespace</td>
            <td>The namespace of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>dependencies</td>
            <td>A list of plugins with dependencies to the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>author</td>
            <td>The name of the plugin author</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>price</td>
            <td>The price of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>keywords</td>
            <td>A list of plugin keywords</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>require</td>
            <td>A list of plugins that are required by the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>notInstalledRequirements</td>
            <td>A list of required plugins that are not installed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>notActiveStageRequirements</td>
            <td>A list of required plugins that are not active in stage</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>notActiveProductiveRequirements</td>
            <td>A list of required plugins that are not active in productive</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>serviceProvider</td>
            <td>The class name of the service provider</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>runOnBuild</td>
            <td>The list of classes to execute once on plugin build</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>checkOnBuild</td>
            <td>The list of classes to execute on every plugin build</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pluginPath</td>
            <td>The plugin path</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>authorIcon</td>
            <td>The author icon</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pluginIcon</td>
            <td>The plugin icon</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>license</td>
            <td>The plugin license</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>shortDescription</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isClosedSource</td>
            <td>is closed source</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>inboxPath</td>
            <td>path in the inbox (closed source, open source)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>marketplaceName</td>
            <td>The plugin name displayed in marketplace</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>source</td>
            <td>Whether this plugin was installed from marketplace, git or local</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>javaScriptFiles</td>
            <td>A list of included javascript files</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>containers</td>
            <td>A list of provided containers with name and description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>dataProviders</td>
            <td>A list of data providers with name and description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>categories</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>webhookUrl</td>
            <td>webhookUrl</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isExternalTool</td>
            <td>is external tool</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>directDownloadLinks</td>
            <td>A list of urls for the external tool</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>forwardLink</td>
            <td>A forward link to the external tool developers page</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>branch</td>
            <td>The branch to checkout for this particular Plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>commit</td>
            <td>The commit to checkout for this particular Plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>subscriptionInformation</td>
            <td>A list if subscription informations</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>offerTrial</td>
            <td>Determines if the plugin offers a trial period for plentyMarketplace</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>offerFreemium</td>
            <td>Determines if the plugin offers freemium functionality</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>configurations</td>
            <td>A list of plugin configuration items</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>webstores</td>
            <td>A list of clients (stores) activated for the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>linkedDataProviders</td>
            <td>A list of dataProviders linked with a container of this plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>linkedContainers</td>
            <td>A list of containers linked with a data provider of this plugin</td>
        </tr><tr>
            <td><a href="plugin#plugin_models_git">Git</a>
</td>
            <td>repository</td>
            <td></td>
        </tr><tr>
            <td><a href="plugin#plugin_models_installedplugins">InstalledPlugins</a>
</td>
            <td>installedPlugins</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>pluginSetIds</td>
            <td>Array of PluginSet Ids where this plugin is contained.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>pluginSetEntries</td>
            <td>A list of PluginSetEntries this plugin is linked to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>pluginSetEntriesWithTrashed</td>
            <td>A list of PluginSetEntries this plugin is linked to, including
trashed
          entries</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### InstalledPlugins<a name="plugin_models_installedplugins"></a>

Model representing an installed Plugin


#### Namespace

`Plenty\Modules\Plugin\Models`




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
            <td>The ID of the installed plugin instance</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationId</td>
            <td>The variationId of the installed version</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td>The id of the installed plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>removed</td>
            <td>Whether this version of the plugin has been removed by the customer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lastUpdateChecksum</td>
            <td>checksum of last installed plugin code</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="plugin_plugin_events"></a>
### PluginSendMail<a name="plugin_events_pluginsendmail"></a>

PluginSendMail


#### Namespace

`Plenty\Modules\Plugin\Events`





#### Methods

<pre>public <strong>getTemplate</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getContactEmail</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getCallFunction</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### AfterBuildPlugins<a name="plugin_events_afterbuildplugins"></a>

Event after plugin build has finished


#### Namespace

`Plenty\Modules\Plugin\Events`





#### Methods

<pre>public <strong>getPluginSet</strong>():<a href="plugin#plugin_models_pluginset">PluginSet</a>
</pre>

    
Get the plugin set which have been built
    
<pre>public <strong>sourceHasChanged</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Check if php files of a plugin have been changed
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>resourcesHasChanged</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Check if resource files of a plugin have been changed
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td></td>
    </tr>
</table>



### LoadSitemapPattern<a name="plugin_events_loadsitemappattern"></a>

LoadSitemapPatternEvent


#### Namespace

`Plenty\Modules\Plugin\Events`




## Services<a name="plugin_plugin_services"></a>
### PluginSeoSitemapService<a name="plugin_services_pluginseositemapservice"></a>

The PluginSeoSitemapService collect the sitemap patterns.


#### Namespace

`Plenty\Modules\Plugin\Services`





#### Methods

<pre>public <strong>loadPatterns</strong>(<a target="_blank" href="http://php.net/string">string</a> $url):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$url</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getPatterns</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>setItemPattern</strong>(<a target="_blank" href="http://php.net/array">array</a> $pattern):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$pattern</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setBlogPattern</strong>(<a target="_blank" href="http://php.net/array">array</a> $pattern):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$pattern</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setContentCategoryPattern</strong>(<a target="_blank" href="http://php.net/array">array</a> $pattern):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$pattern</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setItemCategoryPattern</strong>(<a target="_blank" href="http://php.net/array">array</a> $pattern):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$pattern</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getItemPattern</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getBlogPattern</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getItemCategoryPattern</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getContentCategoryPattern</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### PluginSendMailService<a name="plugin_services_pluginsendmailservice"></a>

The PluginSendMailService send mails in plugins


#### Namespace

`Plenty\Modules\Plugin\Services`





#### Methods

<pre>public <strong>sendMail</strong>(<a target="_blank" href="http://php.net/string">string</a> $url, <a target="_blank" href="http://php.net/string">string</a> $template = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $email = &quot;&quot;, <a target="_blank" href="http://php.net/string">string</a> $callFunction = &quot;&quot;):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$url</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$template</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$email</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$callFunction</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getStatus</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setStatus</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $status):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$status</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>isInitialized</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>setInitialized</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $initialized):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$initialized</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getEmailPlaceholder</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>addEmailPlaceholder</strong>(<a target="_blank" href="http://php.net/string">string</a> $placeholder, <a target="_blank" href="http://php.net/string">string</a> $value):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$placeholder</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$value</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setEmailPlaceholder</strong>(<a target="_blank" href="http://php.net/array">array</a> $emailPlaceholder):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$emailPlaceholder</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getEmailPlaceholderKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/string">string</a> $default = &quot;&quot;):<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$key</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$default</td>
        <td></td>
    </tr>
</table>


# DynamoDb<a name="plugin_dynamodb"></a>
    
## Contracts<a name="plugin_dynamodb_contracts"></a>
### DynamoDbRepositoryContract<a name="plugin_contracts_dynamodbrepositorycontract"></a>

AWS DynamoDb Repository (Deprecated)

<div class="panel panel-warning">
    <div class="panel-heading">
        <h3 class="panel-title">
            <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
            Deprecated! <small>(since 2017-06-30)</small>        </h3>
    </div>
    <div class="panel-body">
        Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
    </div>
</div>

#### Namespace

`Plenty\Modules\Plugin\DynamoDb\Contracts`





#### Methods

<pre>public <strong>createTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $attributeDefinitions, <a target="_blank" href="http://php.net/array">array</a> $keySchema, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 3, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 2):<a target="_blank" href="http://php.net/bool">bool</a></pre>

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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


<pre>public <strong>updateTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/int">int</a> $readCapacityUnits = 3, <a target="_blank" href="http://php.net/int">int</a> $writeCapacityUnits = 2):<a target="_blank" href="http://php.net/bool">bool</a></pre>

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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


<pre>public <strong>putItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/array">array</a> $item):<a target="_blank" href="http://php.net/bool">bool</a></pre>

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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


<pre>public <strong>getItem</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName, <a target="_blank" href="http://php.net/bool">bool</a> $consistentRead, <a target="_blank" href="http://php.net/array">array</a> $key):<a target="_blank" href="http://php.net/array">array</a></pre>

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
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

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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


<pre>public <strong>deleteTable</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $tableName):<a target="_blank" href="http://php.net/bool">bool</a></pre>

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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

<div class="panel panel-warning">
        <div class="panel-heading">
            <h3 class="panel-title">
                <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
                Deprecated! <small>(since 2017-06-30)</small>            </h3>
        </div>
        <div class="panel-body">
            Please use Plenty\Modules\Plugin\DataBase\Contracts\DataBase instead
        </div>
    </div>
    
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


# Storage<a name="plugin_storage"></a>
    
## Contracts<a name="plugin_storage_contracts"></a>
### StorageRepositoryContract<a name="plugin_contracts_storagerepositorycontract"></a>

Storage Repository


#### Namespace

`Plenty\Modules\Plugin\Storage\Contracts`





#### Methods

<pre>public <strong>uploadObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/string">string</a> $body, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false, <a target="_blank" href="http://php.net/array">array</a> $metaData = []):<a href="cloud#cloud_models_storageobject">StorageObject</a>
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
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$publicVisible</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$metaData</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a href="cloud#cloud_models_storageobject">StorageObject</a>
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
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
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


<pre>public <strong>getObjectAsTemporaryFileResource</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a target="_blank" href="http://php.net/string">string</a></pre>

    
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
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
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


<pre>public <strong>deleteObject</strong>(<a target="_blank" href="http://php.net/string">string</a> $pluginName, <a target="_blank" href="http://php.net/string">string</a> $key, <a target="_blank" href="http://php.net/bool">bool</a> $publicVisible = false):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
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


<pre>public <strong>getPluginZip</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/string">string</a> $pluginName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get all objects of a plugin as zip file
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$pluginName</td>
        <td></td>
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


# VersionControl<a name="plugin_versioncontrol"></a>
    
## Models<a name="plugin_versioncontrol_models"></a>
### Git<a name="plugin_models_git"></a>

Model holding plugin data concerning Git version control.


#### Namespace

`Plenty\Modules\Plugin\VersionControl\Models`




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
            <td>git id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pluginId</td>
            <td>plugin id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>username</td>
            <td>username for remote account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>password</td>
            <td>password for remote account</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>remoteUrl</td>
            <td>url for remote repository</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>branch</td>
            <td>actual selected branch</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>autoFetch</td>
            <td>automatically fetch from remote repository</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>webhookToken</td>
            <td>token needed for development</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>created timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>last update timestamp</td>
        </tr><tr>
            <td><a href="plugin#plugin_models_plugin">Plugin</a>
</td>
            <td>plugin</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
