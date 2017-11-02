

# EventProcedures<a name="eventprocedures_eventprocedures"></a>
    
## Events<a name="eventprocedures_eventprocedures_events"></a>
### EventProceduresTriggered<a name="eventprocedures_events_eventprocedurestriggered"></a>

plentymarkets event procedures triggered


#### Namespace

`Plenty\Modules\EventProcedures\Events`



#### Methods

<pre>public <strong>getTicket</strong>():<a href="ticket#ticket_models_ticket">Ticket</a>
</pre>

    

    
<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>

    
Get the order that triggered the event.
    
## Services<a name="eventprocedures_eventprocedures_services"></a>
### EventProceduresService<a name="eventprocedures_services_eventproceduresservice"></a>

The EventProcedureService class offers the possibility to register a procedure class and method that can be called by plentymarkets event procedures.


#### Namespace

`Plenty\Modules\EventProcedures\Services`



#### Methods

<pre>public <strong>registerProcedure</strong>(<a target="_blank" href="http://php.net/string">string</a> $moduleName, <a target="_blank" href="http://php.net/string">string</a> $eventType, <a target="_blank" href="http://php.net/array">array</a> $procedureNames, <a target="_blank" href="http://php.net/string">string</a> $procedureClass, <a target="_blank" href="http://php.net/string">string</a> $procedureGroup = \Plenty\Modules\EventProcedures\Services\Entries\ProcedureEntry::PROCEDURE_GROUP_ORDER):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Register a procedure class
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$moduleName</td>
        <td>The name of the module. The name of the module can be choosen freely.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$eventType</td>
        <td>The name of the event type. The event types are determined and can be one of the following:
<ul>
<li> {@see \ProcedureEntry::EVENT_TYPE_ORDER}, </li>
        					<li> {@see \ProcedureEntry::EVENT_TYPE_REORDER} or </li>
<li> {@see \ProcedureEntry::EVENT_TYPE_TICKET} </li>
</ul></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$procedureNames</td>
        <td>The name for the procedure that will be shown in the event procedure UI. The name is unique and will be used for German and English.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$procedureClass</td>
        <td>The fully qualified name of the procedure class to be called by event procedures.
                   		Each procedure class must either contain the execute method defined by plentymarkets or can contain an individual method. The individual method has to be provided along with procedure class.
The method is separated from the class by an "@" sign. The part following the "@" will be interpreted as method name. The part in front of the "@" is the name of the procedure class.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$procedureGroup</td>
        <td>The name of the procedure group. The procedure groups are determined and can be one of the following:
<ul>
<li> {@see \ProcedureEntry::PROCEDURE_GROUP_ORDER}, </li>
                   		<li> {@see \ProcedureEntry::PROCEDURE_GROUP_ITEM}, </li>
<li> {@see \ProcedureEntry::PROCEDURE_GROUP_DOCUMENT}, </li>
                   		<li> {@see \ProcedureEntry::PROCEDURE_GROUP_CONTACT}, </li>
<li> {@see \ProcedureEntry::PROCEDURE_GROUP_SHIPPING}, </li>
                   		<li> {@see \ProcedureEntry::PROCEDURE_GROUP_PAYMENT}, </li>
<li> {@see \ProcedureEntry::PROCEDURE_GROUP_RETURN} or </li>
<li> {@see \ProcedureEntry::PROCEDURE_GROUP_LISTING} </li>
<li> [optional, default={@see \ProcedureEntry::PROCEDURE_GROUP_ORDER}] </li>
</ul></td>
    </tr>
</table>


# Services<a name="eventprocedures_services"></a>
    
## Entries<a name="eventprocedures_services_entries"></a>
### ProcedureEntry<a name="eventprocedures_entries_procedureentry"></a>

The procedure entry contains all information needed to use module procedures in plentymarkets event procedures.


#### Namespace

`Plenty\Modules\EventProcedures\Services\Entries`



#### Methods

<pre>public <strong>getModuleName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the
    
<pre>public <strong>setModuleName</strong>(<a target="_blank" href="http://php.net/string">string</a> $moduleName):<a href="eventprocedures#eventprocedures_entries_procedureentry">ProcedureEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$moduleName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getEventType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the
    
<pre>public <strong>setEventType</strong>(<a target="_blank" href="http://php.net/string">string</a> $eventType):<a href="eventprocedures#eventprocedures_entries_procedureentry">ProcedureEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$eventType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getProcedureNames</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get the
    
<pre>public <strong>setProcedureNames</strong>(<a target="_blank" href="http://php.net/array">array</a> $procedureNames):<a href="eventprocedures#eventprocedures_entries_procedureentry">ProcedureEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$procedureNames</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getProcedureGroup</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the
    
<pre>public <strong>setProcedureGroup</strong>(<a target="_blank" href="http://php.net/string">string</a> $procedureGroup):<a href="eventprocedures#eventprocedures_entries_procedureentry">ProcedureEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$procedureGroup</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getProcedureClass</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the
    
<pre>public <strong>setProcedureClass</strong>(<a target="_blank" href="http://php.net/string">string</a> $procedureClass):<a href="eventprocedures#eventprocedures_entries_procedureentry">ProcedureEntry</a>
</pre>

    
Set the
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$procedureClass</td>
        <td></td>
    </tr>
</table>


