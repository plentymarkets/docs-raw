

# EventProcedures<a name="eventprocedures_eventprocedures"></a>
    
## Events<a name="eventprocedures_eventprocedures_events"></a>
### EventProceduresTriggered<a name="eventprocedures_events_eventprocedurestriggered"></a>

plentymarkets event procedures triggered

#### Namespace

`Plenty\Modules\EventProcedures\Events`



#### Methods

<pre>public <strong>getOrder</strong>():<a href="order#order_models_order">Order</a>
</pre>
    
Get the order that triggered the event.
    
## Services<a name="eventprocedures_eventprocedures_services"></a>
### EventProceduresService<a name="eventprocedures_services_eventproceduresservice"></a>

This service class offers the possibility to register a procedure class and method that can be called by plentymarkets event procedures.

#### Namespace

`Plenty\Modules\EventProcedures\Services`



#### Methods

<pre>public <strong>registerProcedure</strong>(<a target="_blank" href="http://php.net/string">string</a> $moduleName, <a target="_blank" href="http://php.net/string">string</a> $eventType, <a target="_blank" href="http://php.net/array">array</a> $procedureNames, <a target="_blank" href="http://php.net/string">string</a> $procedureClass, <a target="_blank" href="http://php.net/string">string</a> $procedureGroup = Plenty\Modules\EventProcedures\Services\Entries\ProcedureEntry::PROCEDURE_GROUP_ORDER):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Register an procedure class (with method) for a given module, event type and procedure group with the given names.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$moduleName</td>
        <td>The name of the module for this entry.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$eventType</td>
        <td>The event type for this entry. Can be one of {@see ProcedureEntry::EVENT_TYPE_ORDER},
                             {@see ProcedureEntry::EVENT_TYPE_REORDER} or {@see ProcedureEntry::EVENT_TYPE_TICKET}.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$procedureNames</td>
        <td>The short descriptions for the procedure to be shown in the event procedure UI for german and english language.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$procedureClass</td>
        <td>The fully qualified name of procedure class to be called by event procedures.
                             If there is a "@" sign in the name, the right part will be interprated as a method name.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$procedureGroup</td>
        <td>The procedure group for this entry. Can be one of {@see ProcedureEntry::PROCEDURE_GROUP_ORDER},
                             {@see ProcedureEntry::PROCEDURE_GROUP_ITEM}, {@see ProcedureEntry::PROCEDURE_GROUP_DOCUMENT},
                             {@see ProcedureEntry::PROCEDURE_GROUP_CONTACT}, {@see ProcedureEntry::PROCEDURE_GROUP_SHIPPING},
                             {@see ProcedureEntry::PROCEDURE_GROUP_PAYMENT}, {@see ProcedureEntry::PROCEDURE_GROUP_RETURN} or
								{@see ProcedureEntry::PROCEDURE_GROUP_LISTING}. [optional, default={@see ProcedureEntry::PROCEDURE_GROUP_ORDER}]</td>
    </tr>
</table>


<pre>public <strong>hasProcedureEntry</strong>(<a target="_blank" href="http://php.net/string">string</a> $entryHash):<a target="_blank" href="http://php.net/bool">bool</a></pre>
    
Get whether a procedure entry with the given hash exists or not.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$entryHash</td>
        <td></td>
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


