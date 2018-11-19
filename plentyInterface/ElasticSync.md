

# Models<a name="elasticsync_models"></a>
    
## Sync<a name="elasticsync_models_sync"></a>
### SyncLog<a name="elasticsync_sync_synclog"></a>

The synclog model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Sync`




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
            <td>The ID of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>syncId</td>
            <td>The syncId of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>syncHash</td>
            <td>The syncHash of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>jobHash</td>
            <td>The jobHash of the synclog</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>hashDate</td>
            <td>The hashDate of the synclog</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the synclog was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the synclog was last updated</td>
        </tr><tr>
            <td><a href="elasticsync#elasticsync_sync_synclog">SyncLog</a>
</td>
            <td>syncLog</td>
            <td>The sync log from ElasticSync.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Mapping<a name="elasticsync_sync_mapping"></a>

The mapping model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Sync`




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
            <td>The ID of the mapping</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>data</td>
            <td>The data of the mapping</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the mapping was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the mapping was last updated</td>
        </tr><tr>
            <td><a href="elasticsync#elasticsync_sync_mapping">Mapping</a>
</td>
            <td>mapping</td>
            <td>The mapping from ElasticSync.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Sync<a name="elasticsync_sync_sync"></a>

The sync model.


#### Namespace

`Plenty\Modules\ElasticSync\Models\Sync`




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
            <td>The ID of the sync</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>data</td>
            <td>The data of the sync</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the sync was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the sync was last updated</td>
        </tr><tr>
            <td><a href="elasticsync#elasticsync_sync_sync">Sync</a>
</td>
            <td>sync</td>
            <td>The sync from ElasticSync.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
