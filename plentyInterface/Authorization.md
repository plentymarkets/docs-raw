

# Authorization<a name="authorization_authorization"></a>
    
## Contracts<a name="authorization_authorization_contracts"></a>
### AuthorizedUserRepositoryContract<a name="authorization_contracts_authorizeduserrepositorycontract"></a>

service to get current authorized user


#### Namespace

`Plenty\Modules\Authorization\Contracts`



#### Methods

<pre>public <strong>getCurrentAuthorizedUser</strong>():<a href="authorization#authorization_models_authorizeduser">AuthorizedUser</a>
</pre>

    

    
## Exception<a name="authorization_authorization_exception"></a>
### AuthorizationException<a name="authorization_exception_authorizationexception"></a>

Class AuthorizationException


#### Namespace

`Plenty\Modules\Authorization\Exception`


## Models<a name="authorization_authorization_models"></a>
### AuthorizedUser<a name="authorization_models_authorizeduser"></a>

The current authorized user


#### Namespace

`Plenty\Modules\Authorization\Models`


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
            <td>realName</td>
            <td>The real name of the authorized user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>lang</td>
            <td>The back end language used by the authorized user</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>isSupportUser</td>
            <td>Shows whether the authorized user is a support user</td>
        </tr><tr>
            <td><a href="authentication#authentication_models_user">User</a>
</td>
            <td>user</td>
            <td>Further information about the user's class, roles and rights</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>oauthAccessTokensId</td>
            <td>The access token for OAUTH authentication</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Permission<a name="authorization_models_permission"></a>

The authentication Permission (REST) model


#### Namespace

`Plenty\Modules\Authorization\Models`


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
            <td>permission id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>permissionKey</td>
            <td>permission key</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>roles</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Role<a name="authorization_models_role"></a>

The Role authentication model


#### Namespace

`Plenty\Modules\Authorization\Models`


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
            <td>role id</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>role name</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>holdParents</td>
            <td>hold parents if there is a new child</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>hidden</td>
            <td>hidden status for internal roles</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>users</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>permissions</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Services<a name="authorization_authorization_services"></a>
### AuthHelper<a name="authorization_services_authhelper"></a>

Service to process unguarded php code


#### Namespace

`Plenty\Modules\Authorization\Services`



#### Methods

<pre>public <strong>processUnguarded</strong>(<a target="_blank" href="http://php.net/callable">callable</a> $callable):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/callable">callable</a></td>
        <td>$callable</td>
        <td></td>
    </tr>
</table>


