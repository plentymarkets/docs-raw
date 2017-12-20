

# Ticket<a name="ticket_ticket"></a>
    
## Contracts<a name="ticket_ticket_contracts"></a>
### TicketRepositoryContract<a name="ticket_contracts_ticketrepositorycontract"></a>

The TicketRepositoryContract is the interface for the ticket repository. This interface allows to list tickets by filters.


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>createTicket</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_ticket">Ticket</a>
</pre>

    
Create a new ticket.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The ticket data as associative array.</td>
    </tr>
</table>


<pre>public <strong>searchTickets</strong>(<a target="_blank" href="http://php.net/array">array</a> $filter, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List tickets by filter options.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filter</td>
        <td>The filter</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of tickets to be displayed per page. The default number of tickets per page is 50.</td>
    </tr>
</table>


<pre>public <strong>deleteTicket</strong>(<a target="_blank" href="http://php.net/int">int</a> $ticketId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a ticket by given ticketId
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createMessage</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketId):<a href="ticket#ticket_models_ticketmessage">TicketMessage</a>
</pre>

    
Creates a message for a ticket.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The message data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketId</td>
        <td>The ID of the ticket to associate this to</td>
    </tr>
</table>


<pre>public <strong>updateTicket</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketId):<a href="ticket#ticket_models_ticket">Ticket</a>
</pre>

    
Updates a ticket with given data.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The updating data as associative array</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketId</td>
        <td>The ID of the ticket to associate this to</td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $ticketId):<a href="ticket#ticket_models_ticket">Ticket</a>
</pre>

    
Get an ticket
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketId</td>
        <td>The ID of the ticket</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    

### TicketRoleNameRepositoryContract<a name="ticket_contracts_ticketrolenamerepositorycontract"></a>

TicketRoleName Repository


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketRoleNameId):<a href="ticket#ticket_models_ticketrolename">TicketRoleName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketRoleNameId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_ticketrolename">TicketRoleName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>



### TicketRoleRepositoryContract<a name="ticket_contracts_ticketrolerepositorycontract"></a>

Ticket role repository


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketRoleId):<a href="ticket#ticket_models_ticketrole">TicketRole</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketRoleId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_ticketrole">TicketRole</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>



### TicketStatusNameRepositoryContract<a name="ticket_contracts_ticketstatusnamerepositorycontract"></a>

TicketStatusName Repository


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketStatusNameId):<a href="ticket#ticket_models_ticketstatusname">TicketStatusName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketStatusNameId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_ticketstatusname">TicketStatusName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>



### TicketStatusRepositoryContract<a name="ticket_contracts_ticketstatusrepositorycontract"></a>

TicketStatus repository


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketStatusId):<a href="ticket#ticket_models_ticketstatus">TicketStatus</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketStatusId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_ticketstatus">TicketStatus</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByTypeId</strong>(<a target="_blank" href="http://php.net/int">int</a> $typeId):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$typeId</td>
        <td></td>
    </tr>
</table>



### TicketTypeNameRepositoryContract<a name="ticket_contracts_tickettypenamerepositorycontract"></a>

TicketTypeName repository


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketTypeNameId):<a href="ticket#ticket_models_tickettypename">TicketTypeName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketTypeNameId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_tickettypename">TicketTypeName</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByName</strong>(<a target="_blank" href="http://php.net/string">string</a> $name, <a target="_blank" href="http://php.net/string">string</a> $lang):<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$name</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td></td>
    </tr>
</table>



### TicketTypeRepositoryContract<a name="ticket_contracts_tickettyperepositorycontract"></a>

TicketType repository


#### Namespace

`Plenty\Modules\Ticket\Contracts`



#### Methods

<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $ticketTypeId):<a href="ticket#ticket_models_tickettype">TicketType</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$ticketTypeId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="ticket#ticket_models_tickettype">TicketType</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


## Models<a name="ticket_ticket_models"></a>
### Ticket<a name="ticket_models_ticket"></a>

The ticket model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type ID of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priorityId</td>
            <td>The priority ID of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentTicketId</td>
            <td>The ID of the parent ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusId</td>
            <td>The status ID of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>confidential</td>
            <td>The confidential value. Displays 1 if the ticket is confidential. Displays 0 if the ticket is not confidential.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The ID of the contact that is linked with the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the ticket was created as unix timestamp or carbon object</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>The time the ticket was last updated as unix timestamp or carbon object</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contactLastUpdateAt</td>
            <td>The time the contact was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deadlineAt</td>
            <td>The date of the ticket deadline</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>finishedAt</td>
            <td>The date the ticket is solved and displays 100 percent in the progress bar</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>progress</td>
            <td>The progress of the ticket in percent</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>plentyId</td>
            <td>The ID of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>source</td>
            <td>The source of the ticket. Possible values are 'frontend', 'backend', 'ebay' and 'email'.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>documentsCount</td>
            <td>The number of documents that are attached to the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>hasDocuments</td>
            <td>Displays 1 if the ticket has one or more documents. Displays 0 if the ticket has no document.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>childrenCount</td>
            <td>The number of child tickets</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>resubmissionAt</td>
            <td>The date the ticket should be resubmitted</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>parseData</td>
            <td>The ParseData from the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>owners</td>
            <td>The owners of the ticket. It is a combination of the user ID and the role ID.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>messages</td>
            <td>The messages of the ticket</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketMessage<a name="ticket_models_ticketmessage"></a>

The ticket message model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ticketId</td>
            <td>The ticket ID the message belongs to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The user of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>The time the ticket message was created as unix timestamp or carbon object</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>text</td>
            <td>The content of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>type</td>
            <td>The type of the message. Two types are available:
<ul>
<li>message (visible for the customer)</li>
<li>comment (not visible for the customer)</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>source</td>
            <td>The origin of the message. The following sources are available by default and cannot be deleted.
<ul>
<li>backend</li>
<li>frontend</li>
<li>ebay</li>
<li>email</li>
</ul></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>topicId</td>
            <td>The ID of the topic the message is assigned to</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketMessageTopic<a name="ticket_models_ticketmessagetopic"></a>

The ticket message topic model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The id of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the topic</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketMessageTopicName<a name="ticket_models_ticketmessagetopicname"></a>

The ticket message topic name model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the message</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>topicId</td>
            <td>The ID of the topic</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the topic</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the topic</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketOwner<a name="ticket_models_ticketowner"></a>

The ticket owner model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>ticketId</td>
            <td>The ID of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The user ID of the owner</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>roleId</td>
            <td>The role ID of the owner</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketRole<a name="ticket_models_ticketrole"></a>

The ticket role model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the role</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the role</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketRoleName<a name="ticket_models_ticketrolename"></a>

The ticket role name model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the role name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>roleId</td>
            <td>The ID of the role</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of the role</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the role</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketStatus<a name="ticket_models_ticketstatus"></a>

The ticket status model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type ID of the status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusGroupId</td>
            <td>The status group ID of the status</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketStatusGroup<a name="ticket_models_ticketstatusgroup"></a>

The ticket status group model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the status group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the status group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>color</td>
            <td>The color of the status group</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketStatusGroupName<a name="ticket_models_ticketstatusgroupname"></a>

The ticket status group name model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of the status group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the status group</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketStatusName<a name="ticket_models_ticketstatusname"></a>

The ticket status name model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the status name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusId</td>
            <td>The status ID of the status name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the status name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the status</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketType<a name="ticket_models_tickettype"></a>

The ticket type model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the role</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the role</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>names</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### TicketTypeName<a name="ticket_models_tickettypename"></a>

The ticket type name model.


#### Namespace

`Plenty\Modules\Ticket\Models`


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
            <td>The ID of the role name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id of the role name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the role name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the role</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
