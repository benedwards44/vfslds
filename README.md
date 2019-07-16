# vfslds
Basic SLDS components for VisualForce

## VisualForce Boilerplate

```
<apex:page standardController="Account" docType="html-5.0">

    <apex:slds />

    <div class="slds-scope">

        <c:Spinner />

        <apex:form >

            <c:SectionHeader title="{!Account.Name}"
                subtitle="View Account"
                iconClassName="slds-icon-standard-account"
                iconUrl="{!URLFOR($Asset.SLDS, '/assets/icons/standard-sprite/svg/symbols.svg#account')}"
            >
                <li><apex:commandButton value="Cancel" action="{!cancel}" styleClass="slds-button slds-button_neutral" onclick="showSpinner();"/></li>
            </c:SectionHeader>

            <c:PageMessages />

        </apex:form>

    </div>

</apex:page>
```

<a href="https://githubsfdeploy.herokuapp.com?owner=benedwards44&repo=vfslds&ref=master">
    <img alt="Deploy to Salesforce" src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>
