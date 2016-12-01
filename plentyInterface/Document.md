

# Document<a name="document_document"></a>
    
## Models<a name="document_document_models"></a>
### Document<a name="document_models_document"></a>

Document


#### Namespace

`Plenty\Modules\Document\Models`


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
            <td>The ID of the document.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the document.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>number</td>
            <td>The document number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>numberWithPrefix</td>
            <td>Number with prefix</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>directoryId</td>
            <td>The directory id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td>The path</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The user id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>source</td>
            <td>The source</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayDate</td>
            <td>The date displayed on the document</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>created at timestamp</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>updated at timestamp</td>
        </tr><tr>
            <td><a href="document#document_models_documentdirectory">DocumentDirectory</a>
</td>
            <td>directory</td>
            <td>The associated directory</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</td>
            <td>contacts</td>
            <td>Collection of associated contacts</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</td>
            <td>orders</td>
            <td>Collection of associated orders</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</td>
            <td>webstores</td>
            <td>Collection of associated webstores</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</td>
            <td>categories</td>
            <td>Collection of associated categories</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
returns this model as an array
    

### DocumentDirectory<a name="document_models_documentdirectory"></a>

The document directory model


#### Namespace

`Plenty\Modules\Document\Models`


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
            <td>The ID of the directory</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayType</td>
            <td>The display type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The directory name</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
returns this model as an array
    

### DocumentReference<a name="document_models_documentreference"></a>

The document reference model


#### Namespace

`Plenty\Modules\Document\Models`


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
            <td>documentId</td>
            <td>The ID of the document</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The reference type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The reference value (e.g. the id of another model)</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
returns this model as an array
    
