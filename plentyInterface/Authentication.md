

# Authentication<a name="authentication_authentication"></a>
    
## Contracts<a name="authentication_authentication_contracts"></a>
### ContactAuthenticationRepositoryContract<a name="authentication_contracts_contactauthenticationrepositorycontract"></a>

The ContactAuthenticationRepositoryContract is the interface for the authentication repository. This interface allows to authenticate users in the client (store) by email and password or by contact ID and password. The interface also provides a method for logging out users from the client (store).


#### Namespace

`Plenty\Modules\Authentication\Contracts`





#### Methods

<pre>public <strong>authenticateWithContactEmail</strong>(<a target="_blank" href="http://php.net/string">string</a> $contactEmail, <a target="_blank" href="http://php.net/string">string</a> $password):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$contactEmail</td>
        <td>The email address of the contact of the user</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$password</td>
        <td>The password of the user</td>
    </tr>
</table>


<pre>public <strong>authenticateWithContactId</strong>(<a target="_blank" href="http://php.net/int">int</a> $contactId, <a target="_blank" href="http://php.net/string">string</a> $password):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$contactId</td>
        <td>The ID of the contact of the user</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$password</td>
        <td>The password of the user</td>
    </tr>
</table>


<pre>public <strong>authenticateWithPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId, <a target="_blank" href="http://php.net/string">string</a> $password):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td>The PlentyId of the plenty system of the user</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$password</td>
        <td>The password of the user</td>
    </tr>
</table>


<pre>public <strong>authenticateWithToken</strong>(<a target="_blank" href="http://php.net/string">string</a> $token):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$token</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>logout</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
## Models<a name="authentication_authentication_models"></a>
### User<a name="authentication_models_user"></a>

The user authentication model


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
            <td>The ID of the user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userId</td>
            <td>The ID of the user</td>
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
            <td>email</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>emailHash</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>timezone</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ticket</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>password</td>
            <td>The password of the user</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>user</td>
            <td>The login name of the user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>username</td>
            <td>The login name of the user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>userClass</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>userRights</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>uiConfig</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>permissions</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>pluginPermissions</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>roles</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>accessControl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>daysLeftToChangePassword</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isSupportUser</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>oauthAccessTokensId</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="authentication_authentication_events"></a>
### AfterAccountContactLogout<a name="authentication_events_afteraccountcontactlogout"></a>

The event is triggered after a user is logged out from the client (store).


#### Namespace

`Plenty\Modules\Authentication\Events`





### AfterAccountAuthentication<a name="authentication_events_afteraccountauthentication"></a>

The event is triggered after a user is authenticated in the client (store).


#### Namespace

`Plenty\Modules\Authentication\Events`





#### Methods

<pre>public <strong>isSuccessful</strong>():<a target="_blank" href="http://php.net/bool">bool</a></pre>

    

    
<pre>public <strong>getAccountContact</strong>():<a href="account#account_models_contact">Contact</a>
</pre>

    

    
