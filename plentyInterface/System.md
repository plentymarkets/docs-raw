

# System<a name="system_system"></a>
    
## Contracts<a name="system_system_contracts"></a>
### SystemRepositoryContract<a name="system_contracts_systemrepositorycontract"></a>

The Contract for System settings


#### Namespace

`Plenty\Modules\System\Contracts`



#### Methods

<pre>public <strong>findMyPlentyIds</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Finds all plenty IDs for the current contact
    

### WebstoreRepositoryContract<a name="system_contracts_webstorerepositorycontract"></a>

Repository for Webstore


#### Namespace

`Plenty\Modules\System\Contracts`



#### Methods

<pre>public <strong>loadAll</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Shows all webstores
    
<pre>public <strong>loadAllPreview</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    
Shows a preview of all webstores with id and name
    
<pre>public <strong>findByPlentyId</strong>(<a target="_blank" href="http://php.net/int">int</a> $plentyId):<a href="system#system_models_webstore">Webstore</a>
</pre>

    
Shows a specific webstore from type plentymarkets
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$plentyId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findByStoreIdentifier</strong>(<a target="_blank" href="http://php.net/int">int</a> $storeIdentifier):<a href="system#system_models_webstore">Webstore</a>
</pre>

    
Shows a specific webstore
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$storeIdentifier</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>findById</strong>(<a target="_blank" href="http://php.net/int">int</a> $clientId):<a href="system#system_models_webstore">Webstore</a>
</pre>

    
Shows a specific webstore
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$clientId</td>
        <td>The client ID (webstore ID).</td>
    </tr>
</table>


## Models<a name="system_system_models"></a>
### Webstore<a name="system_models_webstore"></a>

The webstore model


#### Namespace

`Plenty\Modules\System\Models`


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
            <td>The ID of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td>The name of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>type</td>
            <td>The type of the client (store)</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>storeIdentifier</td>
            <td>The identifier of the client (store)</td>
        </tr><tr>
            <td><a href="system#system_models_webstoreconfiguration">WebstoreConfiguration</a>
</td>
            <td>configuration</td>
            <td>The configuration information of the client (store)</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
returns this model as an array
    

### WebstoreConfiguration<a name="system_models_webstoreconfiguration"></a>

The Webstore Configuration Model


#### Namespace

`Plenty\Modules\System\Models`


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
            <td>attributesDropDown</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeSelectDefaultOption</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeVariantCheck</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>attributeWithMarkup</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>bankContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>basketReservationTime</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>cancellationRightsContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryItemCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryLevelLimit</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>closed</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultAccountingLocation</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>defaultCurrency</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>defaultLanguage</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>defaultLayout</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultShippingCountryId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>defaultShippingCountryList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>defaultCurrencyList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultParcelServiceId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultParcelServicePresetId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultMethodOfPaymentId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>defaultCustomerClassId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>dhlPackstationValidation</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>dhlAllowPackstationActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>dhlLimitOrderAmountForPackstation</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>dhlAllowPostidentActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>displayAttributeMarkup</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>displayItemName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayItemOnly4Customer</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayPriceColumn</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayPriceNetto</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>doctype</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>domain</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>domainSsl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>dontSplitItemBundle</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>faviconPath</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>frontPageContentPageId</td>
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
            <td>contactContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>legalDisclosureContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blogRatingActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blogMaxRatingPoints</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blogCommentsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blogNewFeedbackVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>blogCustomerNameVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemMaxRatingPoints</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemCommentsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemNewFeedbackVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemCustomerNameVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryRatingActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryMaxRatingPoints</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryCommentsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryNewFeedbackVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryCustomerNameVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>choiceNominationRatingActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>choiceNominationMaxRatingPoints</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>choiceNominationCommentsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>choiceNominationNewFeedbackVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>choiceNominationCustomerNameVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackRatingActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackMaxRatingPoints</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackCommentsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackNewFeedbackVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackCustomerNameVisibility</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>languageList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>languageMode</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>loginMode</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>oversellingWarning</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>maxLoginAttempts</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mobileRedirectActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mobileRedirectUrl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>mobileRedirectItemUrl</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>name</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>newsletterDirId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>paypalAccount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ebayAccount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>privacyPolicyContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>rootDir</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>sessionLifetime</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>shippingContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>socialMedia</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>termsConditionsContentPageId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopsCertificationDeSealHtml</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopsCertificationDeTrustedShopsId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopsCertificationEnSealHtml</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopsCertificationEnTrustedShopsId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopsCertificationFrSealHtml</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>trustedShopsCertificationFrTrustedShopsId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlFacebook</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlFileExtension</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlGooglePlus</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlItemCategory</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlItemContent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlLinking</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlNeedle</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlTitleItemContent</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlTitleItemName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>urlTwitter</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>useCharacterCrossSelling</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>useDefaultShippingCountryAsShopCountry</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>calcEbayShippingCostsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>autoGroupOpenEbayTransactions</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>calcRicardoShippingCostsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>calcHoodShippingCostsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ebayDownsellingActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckRegistrationSave</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckRegistrationInput</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckInvoiceDetailsSave</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckInvoiceDetailsInput</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckShippingDetailsSave</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckShippingDetailsInput</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckCustomerDetailsSave</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckCustomerDetailsInput</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>addressCheckAfterDays</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>facebookLoginActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemCategorySorting1</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemCategorySorting2</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemSortByMonthlySales</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>showBasePriceActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>jumpPaymentActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>jumpShippingActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>showContentTermsFsk</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>newsletterRegistrationActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ignoreCouponMinOrderValueActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ipAddressSaveInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>reuseOrderActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>editOrderActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>currencySymbol</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>externalVatCheckInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerRegistrationCheck</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerPropertyID</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>customerLoginMethod</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>watchlistActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemwishlistActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>documentsActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>dynamicExportActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>couponVisibilityActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>retoureMethod</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemlistPrice</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemlistWeight</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>schedulerActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>editSchedulerPaymentMethodActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>showSEPAMandateDownload</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>changeEmailActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>changePasswordActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>changePasswordSendmail</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>logoutHiddenActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayStatusInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayMyAccountPaymentDateInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayMyAccountDeliveryDateInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayWeightInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayInvoiceDownload</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>displayShippingDateActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>minimumOrderValue</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemAvailabilityDisabledList</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/array">array</a></td>
            <td>itemMeasureUnit</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>quickloginValidDays</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>captchaCodeInactive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemListingOrderImportItemName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>orderRowDeliveryDate</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>browserLanguage</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>categoryRedirectActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>itemRedirectActive</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>itemSearchEngine</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
returns this model as an array
    
