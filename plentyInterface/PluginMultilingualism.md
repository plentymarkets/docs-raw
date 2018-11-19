

# PluginMultilingualism<a name="pluginmultilingualism_pluginmultilingualism"></a>
    
## Contracts<a name="pluginmultilingualism_pluginmultilingualism_contracts"></a>
### PluginTranslationRepositoryContract<a name="pluginmultilingualism_contracts_plugintranslationrepositorycontract"></a>

Get, create , update and delete plugin translations.


#### Namespace

`Plenty\Modules\PluginMultilingualism\Contracts`





#### Methods

<pre>public <strong>listTranslations</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters):<a target="_blank" href="http://php.net/array">array</a></pre>

    
List translations for plugin set
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getTranslation</strong>(<a target="_blank" href="http://php.net/int">int</a> $translationId):<a href="pluginmultilingualism#pluginmultilingualism_models_plugintranslation">PluginTranslation</a>
</pre>

    
Get a translation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$translationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createTranslation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="pluginmultilingualism#pluginmultilingualism_models_plugintranslation">PluginTranslation</a>
</pre>

    
Create a translation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateTranslation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $translationId):<a href="pluginmultilingualism#pluginmultilingualism_models_plugintranslation">PluginTranslation</a>
</pre>

    
Update a translation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$translationId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteTranslation</strong>(<a target="_blank" href="http://php.net/int">int</a> $id):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a translation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$id</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteTranslations</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/string">string</a> $languageCode):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete multiple translation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$languageCode</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateOrCreateTranslation</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="pluginmultilingualism#pluginmultilingualism_models_plugintranslation">PluginTranslation</a>
</pre>

    
Update or create a translation
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
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
    
## Models<a name="pluginmultilingualism_pluginmultilingualism_models"></a>
### PluginTranslation<a name="pluginmultilingualism_models_plugintranslation"></a>

The plugin translation model.


#### Namespace

`Plenty\Modules\PluginMultilingualism\Models`




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
            <td>The ID of the translation</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pluginSetId</td>
            <td>The ID of the plugin set</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pluginName</td>
            <td>The name of the plugin</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>languageCode</td>
            <td>The code of the language</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>fileName</td>
            <td>The file of the key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>key</td>
            <td>The translation key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>value</td>
            <td>The translation value</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the translation was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the translation was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
