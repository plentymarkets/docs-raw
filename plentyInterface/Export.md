

# Idea<a name="export_idea"></a>
    
## Models<a name="export_idea_models"></a>
### Export<a name="export_models_export"></a>

The export model for IDEA exports.


#### Namespace

`Plenty\Modules\Export\Pos\Idea\Models`


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
            <td>The id of the export entry.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>token</td>
            <td>The token generated for the export entry.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>progress</td>
            <td>The progress of the export process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>currentModule</td>
            <td>The currently exporting module of the export process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>state</td>
            <td>The current state of the export process.</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>filename</td>
            <td>The filename of the export content.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>createdAt</td>
            <td>Specifies the creation date of the export entry.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_carbon_carbon">Carbon</a>
</td>
            <td>updatedAt</td>
            <td>Specifies the last update date of the export entry.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>modules</td>
            <td>The modules to be used by the export process.</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</td>
            <td>options</td>
            <td>The options for the export process. Currently only "year" is supported as option key.</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
