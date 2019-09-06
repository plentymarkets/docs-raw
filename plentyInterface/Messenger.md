

# Messenger<a name="messenger_messenger"></a>
    
## Contracts<a name="messenger_messenger_contracts"></a>
### MessengerRepositoryContract<a name="messenger_contracts_messengerrepositorycontract"></a>

The contract defines methods to add and show/list messages.


#### Namespace

`Plenty\Modules\Messenger\Contracts`





#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="messenger#messenger_models_message">Message</a>
</pre>

    
Create a new Message.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>show</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Show a message with all its successors.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td>The UUID5 of the Message.</td>
    </tr>
</table>


<pre>public <strong>list</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid = null, <a target="_blank" href="http://php.net/bool">bool</a> $successors = true, <a target="_blank" href="http://php.net/int">int</a> $amount = self::DEFAULT_MESSAGES_AMOUNT):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List messages.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td>The reference UUID5 of the message to start from (excluding).
If not set, the uuid of the newest message will be used.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$successors</td>
        <td>If set to FALSE, the messages older than the referenced message will be returned.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$amount</td>
        <td>The amount of messages to list (defaults to 50)</td>
    </tr>
</table>


<pre>public <strong>getMessages</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = self::DEFAULT_PAGE_OF_MESSAGES, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = self::DEFAULT_ITEMS_PER_PAGE_OF_MESSAGES):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get messages.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The number of the retured page of messages, default is 1 (the first)</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The amount of messages to list (defaults to 50)</td>
    </tr>
</table>


<pre>public <strong>updateReadBy</strong>(<a target="_blank" href="http://php.net/int">int</a> $readBy, <a target="_blank" href="http://php.net/string">string</a> $uuid):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update ReadBy Array of message
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$readBy</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateVisibility</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/string">string</a> $uuid):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update the visibility of the message.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The message with the data to be updates</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td>The uuid of the messages.</td>
    </tr>
</table>


<pre>public <strong>setDone</strong>(<a target="_blank" href="http://php.net/string">string</a> $doneAt = null, <a target="_blank" href="http://php.net/string">string</a> $uuid):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Set the doneAt date in the message.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$doneAt</td>
        <td>The doneAt date as ISO date string</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td>The uuid of the message.</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Deletes a message stream by uuid.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getAttachment</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid, <a target="_blank" href="http://php.net/string">string</a> $filename):<a href="messenger#messenger_models_attachment">Attachment</a>
</pre>

    
Get a message attachment.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td>The message uuid</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$filename</td>
        <td>The filename of the attachment.</td>
    </tr>
</table>


<pre>public <strong>updateMetaData</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid, <a target="_blank" href="http://php.net/array">array</a> $metaData):<a href="messenger#messenger_models_message">Message</a>
</pre>

    
Update meta data from message
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$metaData</td>
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
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="messenger_messenger_models"></a>
### MessageMetaData<a name="messenger_models_messagemetadata"></a>

The messenger MessageMetaData model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>readBy</td>
            <td>array of users</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### MessageLinkedTo<a name="messenger_models_messagelinkedto"></a>

The messenger MessageLinkedTo model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td>type</td>
            <td>The type of the link (one of {@link MessageTypesService::LINKED_TO_TYPE_MESSAGE},
{@link MessageTypesService::LINKED_TO_TYPE_ORDER}, {@link MessageTypesService::LINKED_TO_TYPE_CONTACT}
and {@link MessageTypesService::LINKED_TO_TYPE_PAYMENT})</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>value</td>
            <td>The value of the link. For type {@link MessageTypesService::LINKED_TO_TYPE_MESSAGE} it is a string (uuid5)
and an integer otherwise.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>typeId</td>
            <td>This can be the id of a sub type (e.g. the order subTypeId). (optional)</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### MessageReferrer<a name="messenger_models_messagereferrer"></a>

The messenger MessageReferrer model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td>type</td>
            <td>The type of the from instance (one of {@link MessageTypesService::REFERRER_TYPE_SYSTEM},
{@link MessageTypesService::REFERRER_TYPE_BACKEND}, {@link MessageTypesService::REFERRER_TYPE_REST}
and {@link MessageTypesService::REFERRER_TYPE_PLUGIN})</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>value</td>
            <td>The value of the instance. It is an integer (the user id) for type
{@link MessageTypesService::REFERRER_TYPE_SYSTEM}, {@link MessageTypesService::REFERRER_TYPE_BACKEND}
and {@link MessageTypesService::REFERRER_TYPE_REST} and a string (the plugin name) for type
{@link MessageTypesService::REFERRER_TYPE_PLUGIN}.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>An optional name for the instance. For type {@link MessageTypesService::REFERRER_TYPE_PLUGIN} it is
the plugin namespace, the user name otherwise.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### MessageFrom<a name="messenger_models_messagefrom"></a>

The messenger MessageFrom model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td>type</td>
            <td>The type of the from instance (one of {@link MessageTypesService::FROM_TYPE_USER},
{@link MessageTypesService::FROM_TYPE_CONTACT} and {@link MessageTypesService::FROM_TYPE_EMAIL})</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>value</td>
            <td>The value of the instance. For type {@link MessageTypesService::FROM_TYPE_EMAIL} it is a string (the email)
and the id of the user or the contact otherwise.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>An optional name for the instance, e.g. the real name for type {@link MessageTypesService::FROM_TYPE_EMAIL}</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Attachment<a name="messenger_models_attachment"></a>

The messenger Attachment model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td>The file name of the attachment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>message</td>
            <td>The uuid of the message the attachment belongs to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>size</td>
            <td>The size of the attachment in bytes.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contentType</td>
            <td>The content type fo the attachment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>content</td>
            <td>The content of the attachment.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Message<a name="messenger_models_message"></a>

The messenger Message model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td>uuid</td>
            <td>The UUID5 identifier of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td>The plenty ID hash</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>parentUuid</td>
            <td>The uuid5 of the parent message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>linkedTo</td>
            <td>An array with MessageLinkedTo instances.</td>
        </tr><tr>
            <td><a href="messenger#messenger_models_messagefrom">MessageFrom</a>
</td>
            <td>from</td>
            <td>The sender of the message as MessageFrom instance.</td>
        </tr><tr>
            <td><a href="messenger#messenger_models_messageto">MessageTo</a>
</td>
            <td>to</td>
            <td>The user and role ids and emails recieving the message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>whispered</td>
            <td>Whether the message is wispered (not visible for the contact/order linked to the message) or not.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>tags</td>
            <td>An array with tag IDs assigned to the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>preview</td>
            <td>The first two lines of the message without any markup</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>message</td>
            <td>The content of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attachedFilesCount</td>
            <td>The amount of attached files (readonly)</td>
        </tr><tr>
            <td><a href="messenger#messenger_models_messagereferrer">MessageReferrer</a>
</td>
            <td>referrer</td>
            <td>The message referrer.</td>
        </tr><tr>
            <td><a href="messenger#messenger_models_messagemetadata">MessageMetaData</a>
</td>
            <td>metaData</td>
            <td>The message metadata</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>doneAt</td>
            <td>The date the messages setted done.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The creation date of the message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The date of the last update of the message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deletedAt</td>
            <td>The date the message was deleted.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>deletedBy</td>
            <td>The id of the user deleted the message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>attachments</td>
            <td>The message attachments.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### MessageTo<a name="messenger_models_messageto"></a>

The messenger MessageTo model


#### Namespace

`Plenty\Modules\Messenger\Models`




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
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>user</td>
            <td>An array with user ids of user recieving the message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>role</td>
            <td>An array with user role ids of user roles recieving the message.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>email</td>
            <td>An array with emails recieving the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>allUsers</td>
            <td>A flag indicating that all system user recieve the message.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="messenger_messenger_events"></a>
### MessageCreated<a name="messenger_events_messagecreated"></a>

The event is triggered after a new message was created


#### Namespace

`Plenty\Modules\Messenger\Events`





#### Methods

<pre>public <strong>isFirstMessage</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
If &lt;tt&gt;TRUE&lt;/tt&gt;, the message is the first one, otherwise an answer message.
    
<pre>public <strong>getMessage</strong>():<a href="messenger#messenger_models_message">Message</a>
</pre>

    
Get the message.
    
## Services<a name="messenger_messenger_services"></a>
### MessagesSearchService<a name="messenger_services_messagessearchservice"></a>

Search service for the messenger


#### Namespace

`Plenty\Modules\Messenger\Services`





#### Methods

<pre>public <strong>find</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid):<a href="messenger#messenger_models_message">Message</a>
</pre>

    
Find the message with the given uuid.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findOrFail</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid):<a href="messenger#messenger_models_message">Message</a>
</pre>

    
Find the message with the given uuid.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findMany</strong>(<a target="_blank" href="http://php.net/string">string</a> $uuid):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Find a stream of messages.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$uuid</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>navigate</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the messages for the given navigation page.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>toArray</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>process</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getPostFilter</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getQuery</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getAggregations</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSuggestions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSources</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getName</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>setName</strong>($name):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$name</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setIsSourceDisabled</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $isSourceDisabled):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isSourceDisabled</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addPostFilter</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $filter):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$filter</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addQuery</strong>(<a href="cloud#cloud_type_typeinterface">TypeInterface</a>
 $query):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_type_typeinterface">TypeInterface</a>
</td>
        <td>$query</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSource</strong>(<a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
 $source):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_source_sourceinterface">SourceInterface</a>
</td>
        <td>$source</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setSorting</strong>(<a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
 $sorting):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_sorting_sortinginterface">SortingInterface</a>
</td>
        <td>$sorting</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addAggregation</strong>(<a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
 $aggregation):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_aggregation_aggregationinterface">AggregationInterface</a>
</td>
        <td>$aggregation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>addSuggestion</strong>(<a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
 $suggestion):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_suggestion_suggestioninterface">SuggestionInterface</a>
</td>
        <td>$suggestion</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setPage</strong>(<a target="_blank" href="http://php.net/int">int</a> $page, <a target="_blank" href="http://php.net/int">int</a> $rowsPerPage):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$rowsPerPage</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setCollapse</strong>(<a href="cloud#cloud_collapse_collapseinterface">CollapseInterface</a>
 $collapse):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_collapse_collapseinterface">CollapseInterface</a>
</td>
        <td>$collapse</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setScoreModifier</strong>(<a href="cloud#cloud_scoremodifier_scoremodifierinterface">ScoreModifierInterface</a>
 $scoreModifier):<a href="cloud#cloud_lib_search">Search</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="cloud#cloud_scoremodifier_scoremodifierinterface">ScoreModifierInterface</a>
</td>
        <td>$scoreModifier</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setMaxResultWindow</strong>(<a target="_blank" href="http://php.net/int">int</a> $maxResults = 10000):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$maxResults</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setIndex</strong>($index):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$index</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilterRaw</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getQueriesRaw</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getAggregationsRaw</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
<pre>public <strong>getSorting</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>getScoreModifier</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    

### MessageTypesService<a name="messenger_services_messagetypesservice"></a>

Types and type validation for several types in messenger


#### Namespace

`Plenty\Modules\Messenger\Services`





#### Methods

<pre>public static <strong>getValidLinkedToTypes</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the valid types for &quot;linked to&quot; references.
    
<pre>public static <strong>isValidLinkedTo</strong>(<a target="_blank" href="http://php.net/string">string</a> $linkType, $linkValue):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether the given link is valid or not.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$linkType</td>
        <td>The link type.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$linkValue</td>
        <td>The link value.</td>
    </tr>
</table>


<pre>public static <strong>getValidFromTypes</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the valid types for &quot;from&quot; references.
    
<pre>public static <strong>isValidFrom</strong>(<a target="_blank" href="http://php.net/string">string</a> $fromType, $fromValue):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether the given from is valid or not.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$fromType</td>
        <td>The from type.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$fromValue</td>
        <td>The from value.</td>
    </tr>
</table>


<pre>public static <strong>getValidReferrerTypes</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the valid types for &quot;referrer&quot; references.
    
<pre>public static <strong>isValidReferrer</strong>(<a target="_blank" href="http://php.net/string">string</a> $referrerType, $referrerValue, <a target="_blank" href="http://php.net/string">string</a> $referrerName = null):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether the given referrer reference is valid or not.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referrerType</td>
        <td>The reference to be checked</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$referrerValue</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referrerName</td>
        <td></td>
    </tr>
</table>


<pre>public static <strong>getValidToTypes</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the valid key types for the &#039;to&#039; array.
    
<pre>public static <strong>isValidTo</strong>(<a target="_blank" href="http://php.net/string">string</a> $toKey):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Checks whether the given key has a valid value for to.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$toKey</td>
        <td></td>
    </tr>
</table>


