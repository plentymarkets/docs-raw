

# CustomerContract<a name="customercontract_customercontract"></a>
    
## Contracts<a name="customercontract_customercontract_contracts"></a>
### CustomerContractRepositoryContract<a name="customercontract_contracts_customercontractrepositorycontract"></a>

This interface provides methods to list contracts


#### Namespace

`Plenty\Modules\CustomerContract\Contracts`





#### Methods

<pre>public <strong>list</strong>():<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
List all contracts
    
<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $contractId):<a href="customercontract#customercontract_models_customercontract">CustomerContract</a>
</pre>

    
Returns a single contract
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contractId</td>
        <td>The contract Id</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="customercontract#customercontract_models_customercontract">CustomerContract</a>
</pre>

    
Add a contract
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Data of the new contract</td>
    </tr>
</table>


<pre>public <strong>document</strong>(<a target="_blank" href="http://php.net/string">string</a> $contractId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Download contract document
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contractId</td>
        <td>The contract Id</td>
    </tr>
</table>



### ContractSigningRepositoryContract<a name="customercontract_contracts_contractsigningrepositorycontract"></a>

This interface provides methods to digital sign contracts


#### Namespace

`Plenty\Modules\CustomerContract\Contracts`





#### Methods

<pre>public <strong>signContract</strong>(<a target="_blank" href="http://php.net/string">string</a> $contractId, <a target="_blank" href="http://php.net/string">string</a> $signerName):<a href="customercontract#customercontract_models_signing">Signing</a>
</pre>

    
Sign a contract
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contractId</td>
        <td>The contract Id</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$signerName</td>
        <td>Name of signer</td>
    </tr>
</table>


<pre>public <strong>getSigning</strong>(<a target="_blank" href="http://php.net/string">string</a> $contractId):<a href="customercontract#customercontract_models_signing">Signing</a>
</pre>

    
Returns signing of a contract
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contractId</td>
        <td>The contract Id</td>
    </tr>
</table>


<pre>public <strong>signedDocument</strong>(<a target="_blank" href="http://php.net/string">string</a> $contractId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Download the signed contract document
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contractId</td>
        <td>The contract Id</td>
    </tr>
</table>


## Models<a name="customercontract_customercontract_models"></a>
### Signing<a name="customercontract_models_signing"></a>

The customer contract model


#### Namespace

`Plenty\Modules\CustomerContract\Models`




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
            <td>contractId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contactId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>signerName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### CustomerContract<a name="customercontract_models_customercontract"></a>

The customer contract model


#### Namespace

`Plenty\Modules\CustomerContract\Models`




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
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contractLang</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>contractName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>contractVisible</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
