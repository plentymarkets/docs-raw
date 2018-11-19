

# History<a name="data_history"></a>
    
## Models<a name="data_history_models"></a>
### DataHistory<a name="data_models_datahistory"></a>

The data history model


#### Namespace

`Plenty\Modules\Data\History\Models`




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
            <td>referenceType</td>
            <td>The data type that changed (for example 'contact')</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referenceId</td>
            <td>The id of data that changed</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The id of the user that invoked the change</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>userName</td>
            <td>The name of the user that invoked the change</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>reference</td>
            <td>The reference of the data</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>uuid</td>
            <td>The unique identifier of the data history item</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</td>
            <td>dataChangeList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ttl</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
