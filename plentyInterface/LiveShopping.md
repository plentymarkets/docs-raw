

# LiveShopping<a name="liveshopping_liveshopping"></a>
    
## Contracts<a name="liveshopping_liveshopping_contracts"></a>
### LiveShoppingRepositoryContract<a name="liveshopping_contracts_liveshoppingrepositorycontract"></a>

Interface for Live Shopping


#### Namespace

`Plenty\Modules\LiveShopping\Contracts`





#### Methods

<pre>public <strong>getLiveShopping</strong>(<a target="_blank" href="http://php.net/int">int</a> $liveShoppingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$liveShoppingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getActiveByItemId</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getActive</strong>(<a target="_blank" href="http://php.net/int">int</a> $liveShoppingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$liveShoppingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getNextActive</strong>(<a target="_blank" href="http://php.net/int">int</a> $liveShoppingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$liveShoppingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getLastExpired</strong>(<a target="_blank" href="http://php.net/int">int</a> $liveShoppingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$liveShoppingId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getRecentlyStartedOrExpired</strong>(<a target="_blank" href="http://php.net/int">int</a> $time, <a target="_blank" href="http://php.net/int">int</a> $interval):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$time</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$interval</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>itemHasActiveLiveShopping</strong>(<a target="_blank" href="http://php.net/int">int</a> $itemId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemId</td>
        <td></td>
    </tr>
</table>


## Models<a name="liveshopping_liveshopping_models"></a>
### LiveShopping<a name="liveshopping_models_liveshopping"></a>

The LiveShopping Model


#### Namespace

`Plenty\Modules\LiveShopping\Models`




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
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>fromTime</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>toTime</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantitySold</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantitySoldReal</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quantityMax</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>liveShoppingId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>link</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
