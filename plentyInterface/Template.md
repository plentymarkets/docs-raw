

# Config<a name="template_config"></a>
    
## Contracts<a name="template_config_contracts"></a>
### DesignConfigRepositoryContract<a name="template_contracts_designconfigrepositorycontract"></a>

DesignConfig

#### Namespace

`Plenty\Modules\Template\Design\Config\Contracts`



#### Methods

<pre>public <strong>findByDesignName</strong>(<a target="_blank" href="http://php.net/string">string</a> $designName):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$designName</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByDesignAndWebStore</strong>(<a target="_blank" href="http://php.net/string">string</a> $designName, <a target="_blank" href="http://php.net/int">int</a> $webStoreId):<a href="template#template_models_designconfig">DesignConfig</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$designName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webStoreId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByDesign</strong>(<a href="template#template_models_design">Design</a>
 $design):<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="template#template_models_design">Design</a>
</td>
        <td>$design</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/string">string</a> $designName, <a target="_blank" href="http://php.net/int">int</a> $webstoreId):<a href="template#template_models_designconfig">DesignConfig</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$designName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$webstoreId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>copyDesignConfig</strong>(<a target="_blank" href="http://php.net/string">string</a> $designName, <a target="_blank" href="http://php.net/string">string</a> $newDesignName):<a href="template#template_models_designconfig">DesignConfig</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$designName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$newDesignName</td>
        <td></td>
    </tr>
</table>



### DesignRepositoryContract<a name="template_contracts_designrepositorycontract"></a>

Design

#### Namespace

`Plenty\Modules\Template\Design\Config\Contracts`



#### Methods

<pre>public <strong>loadAll</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>
    

    
<pre>public <strong>findByDesignName</strong>(<a target="_blank" href="http://php.net/string">string</a> $designName, <a target="_blank" href="http://php.net/bool">bool</a> $withConfig = true):<a href="template#template_models_design">Design</a>
</pre>
    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$designName</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$withConfig</td>
        <td></td>
    </tr>
</table>


## Models<a name="template_config_models"></a>
### Design<a name="template_models_design"></a>

Design model

#### Namespace

`Plenty\Modules\Template\Design\Config\Models`


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
            <td>designName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>imageDir</td>
            <td>directory of images</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>export</td>
            <td>directory of images</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>updatedAt</td>
            <td>created at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>createdAt</td>
            <td>updated at date timestamp</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>config</td>
            <td>list of configurations of each webstore</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    

### DesignConfig<a name="template_models_designconfig"></a>

Design configuration model

#### Namespace

`Plenty\Modules\Template\Design\Config\Models`


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
            <td>webstoreId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>error404ContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>bankContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>cancellationRightsContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>termsConditionsContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>contactContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>legalDisclosureContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>helpContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemNotFoundContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paymentMethodsContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>privacyPolicyContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>frontPageContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerRegistrationPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderConfirmationPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>lostPasswordPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>loginPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>logoutPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>typeOfCheckout</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep1PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep2PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep3PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep4PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep5PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep6PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep7PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep8PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep9PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>checkoutStep10PageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pageDesignWebshop</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pageDesignCheckout</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pageDesignMyAccount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pageDesignBlog</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>pageDesignForum</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>
    
returns this model as an array
    
