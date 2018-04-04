

# Property<a name="property_property"></a>
    
## Contracts<a name="property_property_contracts"></a>
### PropertyAvailabilityRepositoryContract<a name="property_contracts_propertyavailabilityrepositorycontract"></a>

Get, create, update and delete property availability.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $availabilityId):<a href="property#property_models_propertyavailability">PropertyAvailability</a>
</pre>

    
Gets an availability. The ID of the availability must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$availabilityId</td>
        <td>The ID of the availability</td>
    </tr>
</table>


<pre>public <strong>listAvailabilities</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists availabilities
    
<pre>public <strong>createAvailability</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyavailability">PropertyAvailability</a>
</pre>

    
Creates an availability
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $availabilityId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyavailability">PropertyAvailability</a>
</pre>

    
Updates an availability. The ID of availability must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$availabilityId</td>
        <td>The ID of the availability</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteAvailability</strong>(<a target="_blank" href="http://php.net/int">int</a> $availabilityId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes an availability. The ID of availability must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$availabilityId</td>
        <td>The ID of the availability</td>
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
    

### PropertyGroupNameRepositoryContract<a name="property_contracts_propertygroupnamerepositorycontract"></a>

This interface allows you to get, list, create, update and delete property group names.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getGroupName</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupNameId):<a href="property#property_models_propertygroupname">PropertyGroupName</a>
</pre>

    
Gets a group name. The ID of the group name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupNameId</td>
        <td>The ID of the group name</td>
    </tr>
</table>


<pre>public <strong>listGroupNames</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists group names
    
<pre>public <strong>createGroupName</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertygroupname">PropertyGroupName</a>
</pre>

    
Creates a group name
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateGroupName</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupNameId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertygroupname">PropertyGroupName</a>
</pre>

    
Updates a group name. The ID of the group name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupNameId</td>
        <td>The ID of the group name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteGroupName</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupNameId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes a group name. The ID of group name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupNameId</td>
        <td>The ID of the group name</td>
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
    

### PropertyGroupOptionRepositoryContract<a name="property_contracts_propertygroupoptionrepositorycontract"></a>

This interface allows you to get, create, update and delete property group options.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getGroupOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupOptionId):<a href="property#property_models_propertygroupoption">PropertyGroupOption</a>
</pre>

    
Get a group option. The ID of the group option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupOptionId</td>
        <td>The ID of the group option</td>
    </tr>
</table>


<pre>public <strong>listGroupOptions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List group options
    
<pre>public <strong>createGroupOption</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertygroupoption">PropertyGroupOption</a>
</pre>

    
Creates a group option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateGroupOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupOptionId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertygroupoption">PropertyGroupOption</a>
</pre>

    
Updates a group option. The ID of group option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupOptionId</td>
        <td>The ID of the group option</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteGroupOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupOptionId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes a group option. The ID of group option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupOptionId</td>
        <td>The ID of the group option</td>
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
    

### PropertyGroupRepositoryContract<a name="property_contracts_propertygrouprepositorycontract"></a>

This interface allows you to get, list, create, update and delete property groups. Property groups help to structure properties.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getGroup</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupId):<a href="property#property_models_propertygroup">PropertyGroup</a>
</pre>

    
Gets a property group. The ID of the group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupId</td>
        <td>The ID of the group</td>
    </tr>
</table>


<pre>public <strong>listGroups</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $paginate = 1):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists property groups
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1. See also $paginate.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of groups to be displayed per page. The default number of groups per page is 50. See also $paginate.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations available are:
<ol><li>properties,</li>
    <li>options and</li>
    <li>names.</li></ol></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filters allow to reduce the results listed. The following filters are currently availablle:
<ol><li>ID</li>
    <li>name</li>
    <li>lang</li>
    <li>optionIdentifier</li>
    <li>groupType</li>
    <li>surchargeType/li></ol></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td>Defines whether or not the result will be a paginated result or a list with all results. If 1 is given for the parameter, the result will be paginated.</td>
    </tr>
</table>


<pre>public <strong>createGroup</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertygroup">PropertyGroup</a>
</pre>

    
Creates a property group
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateGroup</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertygroup">PropertyGroup</a>
</pre>

    
Updates a property group. The ID of group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupId</td>
        <td>The ID of the group</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteGroup</strong>(<a target="_blank" href="http://php.net/int">int</a> $groupId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes a property group. The ID of group must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$groupId</td>
        <td>The ID of the group</td>
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
    

### PropertyMarketRepositoryContract<a name="property_contracts_propertymarketrepositorycontract"></a>

This interface allows you to get, list, create, update and delete property markets.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getPropertyMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyMarketId):<a href="property#property_models_propertymarket">PropertyMarket</a>
</pre>

    
Gets a property market. The ID of the property market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyMarketId</td>
        <td>The ID of the property market</td>
    </tr>
</table>


<pre>public <strong>listPropertyMarkets</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists property markets
    
<pre>public <strong>createPropertyMarket</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertymarket">PropertyMarket</a>
</pre>

    
Creates a property market
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updatePropertyMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyMarketId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertymarket">PropertyMarket</a>
</pre>

    
Updates a property market. The ID of property market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyMarketId</td>
        <td>The ID of the property market</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deletePropertyMarket</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyMarketId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes a property market. The ID of property market must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyMarketId</td>
        <td>The ID of the property market</td>
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
    

### PropertyNameRepositoryContract<a name="property_contracts_propertynamerepositorycontract"></a>

This interface allows you to get, list, create, update and delete property names.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getName</strong>(<a target="_blank" href="http://php.net/int">int</a> $nameId):<a href="property#property_models_propertyname">PropertyName</a>
</pre>

    
Gets a property name. The ID of the property name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$nameId</td>
        <td>The ID of the name</td>
    </tr>
</table>


<pre>public <strong>listNames</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists property names
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createName</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyname">PropertyName</a>
</pre>

    
Creates a property name
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateName</strong>(<a target="_blank" href="http://php.net/int">int</a> $nameId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyname">PropertyName</a>
</pre>

    
Updates a property name. The ID of property name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$nameId</td>
        <td>The ID of the name</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteName</strong>(<a target="_blank" href="http://php.net/int">int</a> $nameId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes a property name. The ID of property name must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$nameId</td>
        <td>The ID of the name</td>
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
    

### PropertyOptionRepositoryContract<a name="property_contracts_propertyoptionrepositorycontract"></a>

This interface allows you to get, list, create, update and delete property options.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getPropertyOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyOptionId):<a href="property#property_models_propertyoption">PropertyOption</a>
</pre>

    
Gets a property option. The ID of the property option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyOptionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listPropertyOptions</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List property options
    
<pre>public <strong>createPropertyOption</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyoption">PropertyOption</a>
</pre>

    
Creates a property option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updatePropertyOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyOptionId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyoption">PropertyOption</a>
</pre>

    
Updates a property option. The ID of property option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyOptionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deletePropertyOption</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyOptionId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Deletes a property option. The ID of property option must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyOptionId</td>
        <td></td>
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
    

### PropertyRelationMarkupRepositoryContract<a name="property_contracts_propertyrelationmarkuprepositorycontract"></a>

This interface allows you to get, list, create, update and delete property relation markups.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getRelationMarkup</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationMarkupId):<a href="property#property_models_propertyrelationmarkup">PropertyRelationMarkup</a>
</pre>

    
Get a property relation markup. The ID of the property relation markup must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationMarkupId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listRelationMarkups</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List property relation markups
    
<pre>public <strong>createRelationMarkup</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelationmarkup">PropertyRelationMarkup</a>
</pre>

    
Creates a property relation markup
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateRelationMarkup</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationMarkupId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelationmarkup">PropertyRelationMarkup</a>
</pre>

    
Updates a property relation markup. The ID of property relation markup must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationMarkupId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteRelationMarkup</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationMarkupId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a property relation markup. The ID of property relation markup must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationMarkupId</td>
        <td></td>
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
    

### PropertyRelationRepositoryContract<a name="property_contracts_propertyrelationrepositorycontract"></a>

This interface allows you to get, create, update and delete property relations.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationId):<a href="property#property_models_propertyrelation">PropertyRelation</a>
</pre>

    
Gets a property relation. The ID of the property relation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listRelations</strong>($filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List property relations
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createRelation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelation">PropertyRelation</a>
</pre>

    
Creates a property relation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelation">PropertyRelation</a>
</pre>

    
Updates a property relation. The ID of property relation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteRelation</strong>(<a target="_blank" href="http://php.net/int">int</a> $relationId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a property relation. The ID of property relation must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$relationId</td>
        <td></td>
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
    

### PropertyRelationValueRepositoryContract<a name="property_contracts_propertyrelationvaluerepositorycontract"></a>

This interface allows you to get, create, update and delete property relation values.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getPropertyRelationValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyRelationValueId):<a href="property#property_models_propertyrelationvalue">PropertyRelationValue</a>
</pre>

    
Gets an property relation value. The ID of the property relation value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyRelationValueId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listPropertyRelationValues</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List property relation values
    
<pre>public <strong>createPropertyRelationValue</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelationvalue">PropertyRelationValue</a>
</pre>

    
Creates an property relation value
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updatePropertyRelationValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyRelationValueId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelationvalue">PropertyRelationValue</a>
</pre>

    
Updates a property relation value. The ID of property relation value must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyRelationValueId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updatePropertyRelationValues</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyrelationvalue">PropertyRelationValue</a>
</pre>

    
Update multiple property relation values
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deletePropertyRelationValue</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyRelationValueId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a property relation value
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyRelationValueId</td>
        <td></td>
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
    

### PropertyRepositoryContract<a name="property_contracts_propertyrepositorycontract"></a>

This interface allows you to get, create, update and delete properties.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getProperty</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="property#property_models_property">Property</a>
</pre>

    
Gets a property. The ID of the property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listProperties</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = [], <a target="_blank" href="http://php.net/int">int</a> $paginate = 1, <a target="_blank" href="http://php.net/array">array</a> $orderBy = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Lists properties
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1. See also $paginate.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of properties to be displayed per page. The default number of properties per page is 50. See also $paginate.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations available are:
<ol><li>availibilities</li>
    <li>relation</li>
    <li>selections</li>
    <li>names</li>
    <li>options</li>
    <li>markets</li>
    <li>groups</li></ol></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The following filters are available:
<ol><li>id</li>
    <li>cast</li>
    <li>position</li>
    <li>name</li>
    <li>lang</li>
    <li>group</li></ol></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$paginate</td>
        <td>Defines whether or not the result will be a paginated result or a list with all results. If 1 is given for the parameter, the result will be paginated.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$orderBy</td>
        <td>The order after which the result is sorted</td>
    </tr>
</table>


<pre>public <strong>createProperty</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_property">Property</a>
</pre>

    
Creates a property
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updateProperty</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_property">Property</a>
</pre>

    
Updates a property. The ID of property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteProperty</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertyId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a property. The ID of property must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertyId</td>
        <td></td>
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
    

### PropertySelectionRepositoryContract<a name="property_contracts_propertyselectionrepositorycontract"></a>

This interface allows you to get, create, update and delete property selections.


#### Namespace

`Plenty\Modules\Property\Contracts`





#### Methods

<pre>public <strong>getPropertySelection</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertySelectionId):<a href="property#property_models_propertyselection">PropertySelection</a>
</pre>

    
Gets a property selection. The ID of the property selection must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertySelectionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listPropertySelections</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List property selections
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>The page to get. The default page that will be returned is page 1. See also $paginate.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>The number of property selections to be displayed per page. The default number of selections per page is 50. See also $paginate.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td>The relations available are:
<ol><li>property</li>
    <li>relation</li></ol></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td>The filter available is:
<ol><li>porpertyId</li></ol></td>
    </tr>
</table>


<pre>public <strong>createPropertySelection</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyselection">PropertySelection</a>
</pre>

    
Creates a property selection
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>updatePropertySelection</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertySelectionId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="property#property_models_propertyselection">PropertySelection</a>
</pre>

    
Updates a property selection. The ID of property selection must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertySelectionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deletePropertySelection</strong>(<a target="_blank" href="http://php.net/int">int</a> $propertySelectionId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Deletes a property selection. The ID of property selection must be specified.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$propertySelectionId</td>
        <td></td>
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
    
## Models<a name="property_property_models"></a>
### Property<a name="property_models_property"></a>

The property model. Properties allow to further describe items, categories etc. A property can have one name per language. The property names have an own model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>cast</td>
            <td>The cast of the property (array values: 'empty','int','float','selection','shortText','longText','date','file')</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the property</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyAvailability<a name="property_models_propertyavailability"></a>

The property availability model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property availability</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the property availability</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>value</td>
            <td>The value of the property availability</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property availability was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property availability was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyGroup<a name="property_models_propertygroup"></a>

The property group model. A property group allows to group several properties together and helps to structure properties. Property groups can have different names per language. The property group names have an own model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the property group</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property group was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property group was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyGroupName<a name="property_models_propertygroupname"></a>

The property group name model. A property group can have several names. One name per language. Each name has a unique ID.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property group name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyGroupId</td>
            <td>The ID of the property group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the property group name as ISO 639-1 language code, e.g. en for English</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the property group</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property group name was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property group name was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyGroupOption<a name="property_models_propertygroupoption"></a>

The property group option model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property group option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyGroupId</td>
            <td>The ID of the property group</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>groupOptionIdentifier</td>
            <td>The identifier of the property group option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property group option</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property group option was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property group option was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyGroupRelation<a name="property_models_propertygrouprelation"></a>

The property group relation model. The model shows which property is related to which property group.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyGroupId</td>
            <td>The ID of the property group</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyMarket<a name="property_models_propertymarket"></a>

The property market model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property market</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>referrerId</td>
            <td>The ID of the referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>referrerSubId</td>
            <td>The ID of the sub referrer</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property market</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property market was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property market was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyName<a name="property_models_propertyname"></a>

The property name model. A property can have several names. One name per language. Each name has a unique ID.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the property name as ISO 639-1 language code, e.g. en for English</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the property</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property name was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property name was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyOption<a name="property_models_propertyoption"></a>

The property option model. Property options allow to add further specification to a property. Each property option can have several values. The porperty option values have an own model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>typeOptionIdentifier</td>
            <td>The identifier of the type option</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property option was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property option was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyOptionValue<a name="property_models_propertyoptionvalue"></a>

The property option value model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property option value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>optionId</td>
            <td>The ID of the property option</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property option</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property option value was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property option value was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyRelation<a name="property_models_propertyrelation"></a>

The property relation model allows to relate a property e.g. to a variation or other targets.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relationTypeIdentifier</td>
            <td>The identifier of the property relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>relationTargetId</td>
            <td>The ID of the target of the relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>selectionRelationId</td>
            <td>The ID of the selection relation</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyRelationMarkup<a name="property_models_propertyrelationmarkup"></a>

The property relation markup model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property relation markup</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyRelationId</td>
            <td>The ID of the property relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>variationSalesPriceId</td>
            <td>The variation sales price id of the property relation markup</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>markup</td>
            <td>The markup of the property relation markup</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertyRelationValue<a name="property_models_propertyrelationvalue"></a>

The property relation value model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property relation value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyRelationId</td>
            <td>The ID of the property relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The language of the property relation value</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The value of the property relation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description of the property relation value</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property relation value was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property relation value was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### PropertySelection<a name="property_models_propertyselection"></a>

The property selection model.


#### Namespace

`Plenty\Modules\Property\Models`




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
            <td>The ID of the property selection</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>propertyId</td>
            <td>The ID of the property</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td>The position of the property selection</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the property selection was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the property selection was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
