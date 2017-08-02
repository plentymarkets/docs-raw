

# Document<a name="document_document"></a>
    
## Contracts<a name="document_document_contracts"></a>
### DocumentRepositoryContract<a name="document_contracts_documentrepositorycontract"></a>

Download and list order documents as well as download, list, upload and delete category documents.


#### Namespace

`Plenty\Modules\Document\Contracts`



#### Methods

<pre>public <strong>getDocumentPath</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get the path to a document
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the document</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $id, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="document#document_models_document">Document</a>
</pre>

    
Get a document
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td>The ID of the document</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to be loaded</td>
    </tr>
</table>


<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
List documents
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of orders to be displayed per page. The default number of orders per page is 50.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The columns to be loaded</td>
    </tr>
</table>


<pre>public <strong>uploadOrderDocuments</strong>(<a target="_blank" href="http://php.net/int">int</a> $orderId, <a target="_blank" href="http://php.net/string">string</a> $type, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Upload order documents
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$orderId</td>
        <td>The ID of the order</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$type</td>
        <td>The document type. Only 'invoice_external' is supported.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>uploadCategoryDocuments</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Upload category documents
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The ID of the category</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteCategoryDocument</strong>(<a target="_blank" href="http://php.net/int">int</a> $categoryId, <a target="_blank" href="http://php.net/int">int</a> $documentId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Delete a category document.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$categoryId</td>
        <td>The ID of the category</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$documentId</td>
        <td>The ID of the document</td>
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
            <td>The ID of the document</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the document</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>number</td>
            <td>The document number</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>numberWithPrefix</td>
            <td>The document number with prefix</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>path</td>
            <td>The path to the document</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>source</td>
            <td>The source where the document was generated. Possible sources are 'klarna', 'soap', 'admin', 'hitmeister', 'paypal' and 'rest'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayDate</td>
            <td>The date displayed on the document</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The time the document was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The time the document was last updated</td>
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

    
Returns this model as an array.
    

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

    
Returns this model as an array.
    
