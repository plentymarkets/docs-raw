

# Ticket<a name="ticket_ticket"></a>
    
## Contracts<a name="ticket_ticket_contracts"></a>
### TicketRepositoryContract<a name="ticket_contracts_ticketrepositorycontract"></a>

The TicketRepositoryContract is the interface for the ticket repository. This interface allows to list tickets by filters

#### Namespace

Plenty\Modules\Ticket\Contracts



#### Methods

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


## Models<a name="ticket_ticket_models"></a>
### Ticket<a name="ticket_models_ticket"></a>

The ticket model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priorityId</td>
            <td>The priority id of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>parentTicketId</td>
            <td>The id of the parent ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusId</td>
            <td>The status id of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>confidential</td>
            <td>The confidential value. Displays 1 if the ticket is confidential. Displays 0 if the ticket is not confidential.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactId</td>
            <td>The id of the contact that is linked with the ticket</td>
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
            <td>contactLastUpdate</td>
            <td>The time the contact was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deadline</td>
            <td>The date of the ticket deadline</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>done</td>
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
            <td>The id of the online store</td>
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
            <td>orderId</td>
            <td>The id of the order that is linked with the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>emailParseResult</td>
            <td>The parsed email of the ticket</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>hasDocuments</td>
            <td>Displays 1 if the ticket has one or more documents. Displays 0 if the ticket has no document.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>childsCount</td>
            <td>The number of child tickets</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>resubmission</td>
            <td>The date the ticket should be resubmitted</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketOwner<a name="ticket_models_ticketowner"></a>

The ticket owner model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the ticket.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The user id of the owner.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>roleId</td>
            <td>The role id of the owner.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketRole<a name="ticket_models_ticketrole"></a>

The ticket role model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the role.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the role.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketRoleName<a name="ticket_models_ticketrolename"></a>

The ticket role name model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the role name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>roleId</td>
            <td>The role id.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of role.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The role name.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketStatus<a name="ticket_models_ticketstatus"></a>

The ticket status model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id of the status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>positon</td>
            <td>The position of the status.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>statusGroupId</td>
            <td>The status group id of the status.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketStatusGroup<a name="ticket_models_ticketstatusgroup"></a>

The ticket status group model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the status group.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the status group.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>color</td>
            <td>The color of the status group.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketStatusGroupName<a name="ticket_models_ticketstatusgroupname"></a>

The ticket status group name model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the ticket.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lang</td>
            <td>The language of the status group.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the status group.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketStatusName<a name="ticket_models_ticketstatusname"></a>

The ticket status name model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the status name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id of the status name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language if the status name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the status.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketType<a name="ticket_models_tickettype"></a>

The ticket type model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the role.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the role.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### TicketTypeName<a name="ticket_models_tickettypename"></a>

The ticket type name model.

#### Namespace

Plenty\Modules\Ticket\Models


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
            <td>The id of the role name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeId</td>
            <td>The type id of the role name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language if the role name.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the role.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
