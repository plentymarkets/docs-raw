

# ShopBuilder<a name="shopbuilder_shopbuilder"></a>
    
## Contracts<a name="shopbuilder_shopbuilder_contracts"></a>
### Widget<a name="shopbuilder_contracts_widget"></a>

Contract for content widgets


#### Namespace

`Plenty\Modules\ShopBuilder\Contracts`





#### Methods

<pre>public <strong>getPreview</strong>(<a target="_blank" href="http://php.net/array">array</a> $widgetSettings = [], <a target="_blank" href="http://php.net/array">array</a> $children = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Get the html representation of the widget
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$widgetSettings</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$children</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>render</strong>(<a target="_blank" href="http://php.net/array">array</a> $widgetSettings = [], <a target="_blank" href="http://php.net/array">array</a> $children = []):<a target="_blank" href="http://php.net/string">string</a></pre>

    
Render the widget
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$widgetSettings</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$children</td>
        <td></td>
    </tr>
</table>



### ContentLinkRepositoryContract<a name="shopbuilder_contracts_contentlinkrepositorycontract"></a>

Get, create, delete and update links between shop builder contents and layout containers.


#### Namespace

`Plenty\Modules\ShopBuilder\Contracts`





#### Methods

<pre>public <strong>getContentLinks</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId):<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all linked contents for a plugin set
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getContentLink</strong>(<a target="_blank" href="http://php.net/int">int</a> $contentLinkId):<a href="shopbuilder#shopbuilder_models_contentlink">ContentLink</a>
</pre>

    
Get a single connection between a content and a layout container
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentLinkId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createContentLink</strong>($data):<a href="shopbuilder#shopbuilder_models_contentlink">ContentLink</a>
</pre>

    
Link a content to a layout container
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updateContentLink</strong>(<a target="_blank" href="http://php.net/int">int</a> $contentLinkId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="shopbuilder#shopbuilder_models_contentlink">ContentLink</a>
</pre>

    
Update a link between a content and a layout container
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentLinkId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteContentLink</strong>(<a target="_blank" href="http://php.net/int">int</a> $contentLinkId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Unlink a content from a layout container. The content itself will remain
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentLinkId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getContentLinksForContainer</strong>(<a target="_blank" href="http://php.net/string">string</a> $containerName, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId = null, <a target="_blank" href="http://php.net/string">string</a> $lang = null, <a target="_blank" href="http://php.net/string">string</a> $contentType = null):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get all content links for a specific layout container.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$containerName</td>
        <td>The name of the layout container to get content links for.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>An id of a plugin set to get content links for. Active plugin set will be used by default.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$lang</td>
        <td>The language to get content links for. Current language will be get from session if not defined.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contentType</td>
        <td>Type of the content to get</td>
    </tr>
</table>



### ContentPreset<a name="shopbuilder_contracts_contentpreset"></a>

Contract for content presets


#### Namespace

`Plenty\Modules\ShopBuilder\Contracts`





#### Methods

<pre>public <strong>getWidgets</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get the widget configurations of the presets to be assigned to the created content.
    

### GlobalSettingsHandler<a name="shopbuilder_contracts_globalsettingshandler"></a>

Contract for classes handling global settings for the ShopBuilder.


#### Namespace

`Plenty\Modules\ShopBuilder\Contracts`





#### Methods

<pre>public <strong>readSettings</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Read values of global settings.
    
<pre>public <strong>writeSettings</strong>($values):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Store values of global settings.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$values</td>
        <td></td>
    </tr>
</table>



### ContentRepositoryContract<a name="shopbuilder_contracts_contentrepositorycontract"></a>

Get, create, delete und update shop builder contents.


#### Namespace

`Plenty\Modules\ShopBuilder\Contracts`





#### Methods

<pre>public <strong>getContents</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Get all contents to be edited in the shop builder.
    
<pre>public <strong>searchContents</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 20, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    
Search for contents
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td>Maximum number of items to be returned on each page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td>Current page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>Search parameters</td>
    </tr>
</table>


<pre>public <strong>getContent</strong>(<a target="_blank" href="http://php.net/int">int</a> $contentId, <a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/string">string</a> $frontendLanguage = null):<a href="shopbuilder#shopbuilder_models_content">Content</a>
</pre>

    
Get a single content.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentId</td>
        <td>Id of the content to get information for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>Plugin set id to be used for rendering widgets.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$frontendLanguage</td>
        <td>The language to be used for rendering the widgets.</td>
    </tr>
</table>


<pre>public <strong>createContent</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, $data, <a target="_blank" href="http://php.net/string">string</a> $frontendLanguage = null):<a href="shopbuilder#shopbuilder_models_content">Content</a>
</pre>

    
Create new content. New content will not be linked to any layout container.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>The plugin set to be used to render the content. The raw content data are not depending on a plugin set.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>The raw content data.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$frontendLanguage</td>
        <td>The language to be used for rendering the widgets.</td>
    </tr>
</table>


<pre>public <strong>updateContent</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/int">int</a> $contentId, $data, <a target="_blank" href="http://php.net/string">string</a> $frontendLanguage = null):<a href="shopbuilder#shopbuilder_models_content">Content</a>
</pre>

    
Update content.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>The plugin set to be used to render the content. The raw content data are not depending on a plugin set.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentId</td>
        <td>The id of the content to be updated.</td>
    </tr>
    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$data</td>
        <td>The raw data of the content.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$frontendLanguage</td>
        <td>The language to be used for rendering the widgets.</td>
    </tr>
</table>


<pre>public <strong>deleteContent</strong>(<a target="_blank" href="http://php.net/int">int</a> $pluginSetId, <a target="_blank" href="http://php.net/int">int</a> $contentId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete content. Any connections to layout containers will be removed too.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$pluginSetId</td>
        <td>The plugin set to be used to render the content. The raw content data are not depending on a plugin set.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentId</td>
        <td>The id of the content to be deleted.</td>
    </tr>
</table>


<pre>public <strong>duplicateContent</strong>(<a target="_blank" href="http://php.net/int">int</a> $contentId, <a target="_blank" href="http://php.net/int">int</a> $targetPluginSetId, <a target="_blank" href="http://php.net/string">string</a> $language, <a target="_blank" href="http://php.net/string">string</a> $containerName, <a target="_blank" href="http://php.net/string">string</a> $contentName):<a href="shopbuilder#shopbuilder_models_content">Content</a>
</pre>

    
Duplicate a content and its link
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contentId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$targetPluginSetId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$language</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$containerName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contentName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>rebuildContents</strong>(<a target="_blank" href="http://php.net/string">string</a> $containerName = null):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Rebuild all contents linked to the current plugin set.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$containerName</td>
        <td>Name of the layout container to rebuild contents for.</td>
    </tr>
</table>


## Providers<a name="shopbuilder_shopbuilder_providers"></a>
### DataFieldProvider<a name="shopbuilder_providers_datafieldprovider"></a>

Base class for data field providers.


#### Namespace

`Plenty\Modules\ShopBuilder\Providers`





#### Methods

<pre>public <strong>register</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
<pre>public <strong>addField</strong>(<a target="_blank" href="http://php.net/string">string</a> $identifier, <a target="_blank" href="http://php.net/string">string</a> $label, <a target="_blank" href="http://php.net/string">string</a> $expression):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a new data field.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$identifier</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$label</td>
        <td>The label of the field</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$expression</td>
        <td>The twig expression to be inserted by this field</td>
    </tr>
</table>


<pre>public <strong>addChildProvider</strong>(<a target="_blank" href="http://php.net/string">string</a> $label, <a target="_blank" href="http://php.net/string">string</a> $childProviderClass, <a target="_blank" href="http://php.net/array">array</a> $params = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Register a nested provider containing a list of child data fields.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$label</td>
        <td>The label of the group</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$childProviderClass</td>
        <td>The class name of the nested data fields provider.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$params</td>
        <td>Additional parameters to be passed to provider constructor method.</td>
    </tr>
</table>


<pre>public <strong>addSearchKeywords</strong>(<a target="_blank" href="http://php.net/string">string</a> $identifier, <a target="_blank" href="http://php.net/array">array</a> $keywords = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Assign keywords to a field to be respected during search.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$identifier</td>
        <td>The identifier of the field to assign keywords to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$keywords</td>
        <td>A list of keywords. Each keyword may contain a translation key. A single keyword could be a comma separated list of words.</td>
    </tr>
</table>


## Models<a name="shopbuilder_shopbuilder_models"></a>
### ContentWidget<a name="shopbuilder_models_contentwidget"></a>

Content widget provided by a frontend plugin


#### Namespace

`Plenty\Modules\ShopBuilder\Models`




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
            <td>identifier</td>
            <td>The identifier of the content widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>widgetClass</td>
            <td>The class of the content widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>label</td>
            <td>The label of the content widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>tooltip</td>
            <td>The tooltip of the content widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>previewImageURL</td>
            <td>The preview image the content widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxPerPage</td>
            <td>Maximum occurrences per content of the widget</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>categories</td>
            <td>List of categories</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>allowedNestingTypes</td>
            <td>Allowed types to be nested inside this widget</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>settings</td>
            <td>The settings of the content widget</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContentPageDropzone<a name="shopbuilder_models_contentpagedropzone"></a>

Layout container of a content page where to display link contents generated by the shop builder.


#### Namespace

`Plenty\Modules\ShopBuilder\Models`




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
            <td>container</td>
            <td>The container where dropped contents should be linked to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of contents which can be linked to this dropzone.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContentWidgetPreview<a name="shopbuilder_models_contentwidgetpreview"></a>

The rendered preview of a content widget


#### Namespace

`Plenty\Modules\ShopBuilder\Models`




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
            <td>identifier</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>content</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Content<a name="shopbuilder_models_content"></a>

Content created by the shop builder. May be linked to layout containers.


#### Namespace

`Plenty\Modules\ShopBuilder\Models`




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
            <td>The ID of the content</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>dataProviderName</td>
            <td>The name of the data provider</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the content was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the content was last updated</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the content</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>widgets</td>
            <td>The configured widgets of the content</td>
        </tr><tr>
            <td><a href="shopbuilder#shopbuilder_models_contentlink">ContentLink</a>
</td>
            <td>link</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContentPage<a name="shopbuilder_models_contentpage"></a>

A content page provided by a frontend plugin.


#### Namespace

`Plenty\Modules\ShopBuilder\Models`




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
            <td>identifier</td>
            <td>The identifier of the content page</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>caption</td>
            <td>Translation key to read the caption from</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>dropzones</td>
            <td>Available dropzones of this page to put contents into.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### ContentLink<a name="shopbuilder_models_contentlink"></a>

Links a content from the shop builder to a layout container of the frontend plugin.


#### Namespace

`Plenty\Modules\ShopBuilder\Models`




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
            <td>The ID of the content link</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contentId</td>
            <td>The ID of the content</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>containerName</td>
            <td>The name of the container</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>pluginSetId</td>
            <td>The Id of the plugin set</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>language</td>
            <td>The language where the content is linked to.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>active</td>
            <td>Indicates if the link is active and the content should be visible for the frontend.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relatedContentType</td>
            <td>The content type the content is linked to</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>relatedContainerName</td>
            <td>The container name the content is linked to</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the content was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the content was last updated</td>
        </tr><tr>
            <td><a href="shopbuilder#shopbuilder_models_content">Content</a>
</td>
            <td>content</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Helper<a name="shopbuilder_shopbuilder_helper"></a>
### ShopBuilderRequest<a name="shopbuilder_helper_shopbuilderrequest"></a>

Information provided by each request made from the shop builder preview.


#### Namespace

`Plenty\Modules\ShopBuilder\Helper`





#### Methods

<pre>public <strong>isShopBuilder</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getPreviewContentType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getMainContentType</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setMainContentType</strong>(<a target="_blank" href="http://php.net/string">string</a> $mainContentType):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mainContentType</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getMainContainerName</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>setMainContainerName</strong>(<a target="_blank" href="http://php.net/string">string</a> $mainContainerName):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$mainContainerName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>setMainCategory</strong>($mainCategory):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="miscellaneous#miscellaneous__"></a>
</td>
        <td>$mainCategory</td>
        <td></td>
    </tr>
</table>



### MappableSettingsHandler<a name="shopbuilder_helper_mappablesettingshandler"></a>

Helper to map global configurations to plugin configs.


#### Namespace

`Plenty\Modules\ShopBuilder\Helper`




