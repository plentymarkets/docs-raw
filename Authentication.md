

# Authentication<a name="authentication_authentication"></a>
    
## Contracts<a name="authentication_authentication_contracts"></a>
### ContactAuthenticationRepositoryContract<a name="authentication_contracts_contactauthenticationrepositorycontract"></a>

authentication repository

#### Namespace

`Plenty\Modules\Authentication\Contracts`



#### Methods

<pre>public <strong>authenticateWithContactEmail</strong>(<a target="_blank" href="http://php.net/string">string</a> $contactEmail, <a target="_blank" href="http://php.net/string">string</a> $password):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contactEmail</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$password</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>authenticateWithContactId</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/string">string</a> $password):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$password</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>logout</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>
    

    
## Events<a name="authentication_authentication_events"></a>
### AfterAccountAuthentication<a name="authentication_events_afteraccountauthentication"></a>

account contact authentication event

#### Namespace

`Plenty\Modules\Authentication\Events`



#### Methods

<pre>public <strong>isSuccessful</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>
    

    
<pre>public <strong>getAccountContact</strong>():<a href="account#account_models_contact">Contact</a>
</pre>
    

    

### AfterAccountContactLogout<a name="authentication_events_afteraccountcontactlogout"></a>

Account contact logged out

#### Namespace

`Plenty\Modules\Authentication\Events`


## Models<a name="authentication_authentication_models"></a>
### User<a name="authentication_models_user"></a>

User for authentification

#### Namespace

`Plenty\Modules\Authentication\Models`


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
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>pwd</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>pwd_md5</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>password</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>user</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
