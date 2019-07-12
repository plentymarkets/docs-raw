

# Wizard<a name="wizard_wizard"></a>
    
## Contracts<a name="wizard_wizard_contracts"></a>
### WizardDataRepositoryContract<a name="wizard_contracts_wizarddatarepositorycontract"></a>

This interface provides methods to create, get, list, update and delete wizard data


#### Namespace

`Plenty\Modules\Wizard\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/array">array</a> $steps = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Creates a new WizardData.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$steps</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createDataOption</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/array">array</a> $data = [], <a target="_blank" href="http://php.net/string">string</a> $optionId = &quot;default&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Creates a new WizardData option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a single WizardData by its ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getByOptionId</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/string">string</a> $optionId = &quot;default&quot;):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a single WizardData for an option ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByWizardKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>list</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all WizardData for current plenty ID.
    
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
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/array">array</a> $properties):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update data for a WizardData
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateDataOption</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/string">string</a> $optionId, <a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/string">string</a> $stepKey, <a target="_blank" href="http://php.net/bool">bool</a> $skipValidation = false):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update data for a WizardData option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$stepKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$skipValidation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a single WizardData by its ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteDataOption</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/string">string</a> $optionId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a single WizardData by its ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>finalize</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/string">string</a> $optionId = &quot;default&quot;, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Finalize wizard
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
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
    

### WizardContainerContract<a name="wizard_contracts_wizardcontainercontract"></a>

This interface provides methods to register, get and list all wizards.


#### Namespace

`Plenty\Modules\Wizard\Contracts`





#### Methods

<pre>public <strong>register</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/string">string</a> $wizard):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a wizard
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizard</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>registerFolders</strong>(<a target="_blank" href="http://php.net/string">string</a> $folderClass):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a wizard folder
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$folderClass</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey, <a target="_blank" href="http://php.net/bool">bool</a> $skipTranslation = false):<a href="wizard#wizard_models_wizard">Wizard</a>
</pre>

    
Get a single wizard by its key
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$skipTranslation</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>all</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all wizards class names
    
<pre>public <strong>folders</strong>(<a target="_blank" href="http://php.net/bool">bool</a> $hierarchy = false):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List all wizard folders
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$hierarchy</td>
        <td></td>
    </tr>
</table>



### WizardActionHandler<a name="wizard_contracts_wizardactionhandler"></a>

This interface provides a template for an action handler for Wizards


#### Namespace

`Plenty\Modules\Wizard\Contracts`





### WizardRepositoryContract<a name="wizard_contracts_wizardrepositorycontract"></a>

This interface provides methods to get and list wizards.


#### Namespace

`Plenty\Modules\Wizard\Contracts`





### WizardDynamicLoader<a name="wizard_contracts_wizarddynamicloader"></a>

This interface provides methods to dynamically load data in the wizard ui.


#### Namespace

`Plenty\Modules\Wizard\Contracts`





### WizardDataModifier<a name="wizard_contracts_wizarddatamodifier"></a>

This interface provides methods to modify wizard data.


#### Namespace

`Plenty\Modules\Wizard\Contracts`





#### Methods

<pre>public <strong>modify</strong>(<a target="_blank" href="http://php.net/array">array</a> $parameters):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Modify a wizard data for a step
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
</table>



### WizardSettingsHandler<a name="wizard_contracts_wizardsettingshandler"></a>

This interface provides methods to handle final wizard data.


#### Namespace

`Plenty\Modules\Wizard\Contracts`





#### Methods

<pre>public <strong>handle</strong>(<a target="_blank" href="http://php.net/array">array</a> $parameters):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Handle wizard data for a finalized wizard
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$parameters</td>
        <td></td>
    </tr>
</table>


## Models<a name="wizard_wizard_models"></a>
### Wizard<a name="wizard_models_wizard"></a>

The wizard model.


#### Namespace

`Plenty\Modules\Wizard\Models`




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
            <td>title</td>
            <td>The title</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>The wizard's key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>settingsHandlerClass</td>
            <td>Settings handler</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td>The short description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>translationKey</td>
            <td>The translation key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>deleteConfirmationText</td>
            <td>Delete confirmation Text in deletion overlay</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>topics</td>
            <td>The topics</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>steps</td>
            <td>Wizard's structure</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priority</td>
            <td>Wizard's listing priority in the overview</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relevance</td>
            <td>Wizard's level of relevance</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WizardData<a name="wizard_models_wizarddata"></a>

The wizard data model.


#### Namespace

`Plenty\Modules\Wizard\Models`




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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>plentyIdHash</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>wizardKey</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>data</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>steps</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WizardSection<a name="wizard_models_wizardsection"></a>

The wizard step section model.


#### Namespace

`Plenty\Modules\Wizard\Models`




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
            <td>title</td>
            <td>The title</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>form</td>
            <td>The form</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WizardStep<a name="wizard_models_wizardstep"></a>

The wizard step model.


#### Namespace

`Plenty\Modules\Wizard\Models`




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
            <td>title</td>
            <td>The title</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td>The short description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>modifierClass</td>
            <td>The modifier class</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>validationClass</td>
            <td>The validation class</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>sections</td>
            <td>The sections</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WizardFolder<a name="wizard_models_wizardfolder"></a>

The wizard folder.


#### Namespace

`Plenty\Modules\Wizard\Models`




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
            <td>The name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>priority</td>
            <td>The priority</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>shortDescription</td>
            <td>The short description</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>parent</td>
            <td>The parent</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### WizardFormOption<a name="wizard_models_wizardformoption"></a>

The wizard form option.


#### Namespace

`Plenty\Modules\Wizard\Models`




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
            <td>The name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>placeholder</td>
            <td>The placeholder</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>caption</td>
            <td>The caption. Only for checkboxValues.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>label</td>
            <td>The label</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tooltip</td>
            <td>The tooltip</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="wizard_wizard_services"></a>
### WizardFolderProvider<a name="wizard_services_wizardfolderprovider"></a>

Register a wizard folder.


#### Namespace

`Plenty\Modules\Wizard\Services`





#### Methods

<pre>public <strong>folders</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### WizardProvider<a name="wizard_services_wizardprovider"></a>

Register a wizard.


#### Namespace

`Plenty\Modules\Wizard\Services`





#### Methods

<pre>public <strong>structure</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    
# Services<a name="wizard_services"></a>
    
## DataSources<a name="wizard_services_datasources"></a>
### BaseWizardDataSource<a name="wizard_datasources_basewizarddatasource"></a>

Base data source for wizards


#### Namespace

`Plenty\Modules\Wizard\Services\DataSources`




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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>wizardKey</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>dataStructure</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>setWizardKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $wizardKey):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the wizard key for this data source
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$wizardKey</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getIdentifiers</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
List of option identifiers
    
<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $steps = []):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Create data
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$steps</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>get</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get data
    
<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $properties = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update data
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$properties</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>delete</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete data
    
<pre>public <strong>createDataOption</strong>(<a target="_blank" href="http://php.net/array">array</a> $data = [], <a target="_blank" href="http://php.net/string">string</a> $optionId = &quot;default&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Create data option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getByOptionId</strong>(<a target="_blank" href="http://php.net/string">string</a> $optionId = &quot;default&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get data option by its option ID
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateDataOption</strong>(<a target="_blank" href="http://php.net/string">string</a> $optionId = &quot;default&quot;, <a target="_blank" href="http://php.net/array">array</a> $data = [], <a target="_blank" href="http://php.net/string">string</a> $stepKey = &quot;&quot;):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Update data option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$stepKey</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteDataOption</strong>(<a target="_blank" href="http://php.net/string">string</a> $optionId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete data option
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>finalize</strong>(<a target="_blank" href="http://php.net/string">string</a> $optionId, <a target="_blank" href="http://php.net/array">array</a> $data = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$optionId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


