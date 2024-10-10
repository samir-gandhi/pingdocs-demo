# CIAM-Passwordless-Protect-Registration-Authentication-Account-Recovery-Main Flow
Description: Imported on Wed Sep 13 2023 17:10:12 GMT&#43;0000 (Coordinated Universal Time) 

Color: #CACED3

## Settings
An exhaustive list of settings including defaults.
| Setting                          | Value                                                                                                                                                                                   |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSP Value                        | worker-src &#39;self&#39; blob:; script-src &#39;self&#39; https://cdn.jsdelivr.net https://code.jquery.com https://devsdk.singularkey.com http://cdnjs.cloudflare.com &#39;unsafe-inline&#39; &#39;unsafe-eval&#39;; | 
 | CSS Links                        | https://assets.pingone.com/ux/end-user-nano/0.1.0-alpha.1/end-user-nano.css,https://assets.pingone.com/ux/astro-nano/0.1.0-alpha.7/icons.css|

## Input Schemas
| Property Name | Description | Expanded | Preferred Control Type | Preferred Data Type | Required |
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| flowParameters |  | true | textField | object | false | 
 

## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| agreementId##SK##flowInstance | 29d5d681-93ee-4590-abdc-7d7cd94aa85c | flowInstance |  | string | 0 | 2000 | true | property | 
 | ciam_accountRecoveryEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_agreementEnabled##SK##company | false | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_appleEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_authMethod##SK##flowInstance |  | flowInstance |  | string | 0 | 2000 | true | property | 
 | ciam_companyName##SK##company | Ping Identity | company |  | string | 0 | 2000 | false | property | 
 | ciam_emailOtpEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_facebookEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_fidoPasskeyEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_googleEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_logoStyle##SK##company | width: 65px; height: 65px; | company | CSS style for company logo | string | 0 | 2000 | true | property | 
 | ciam_logoUrl##SK##company | https://assets.pingone.com/ux/ui-library/5.0.2/images/logo-pingidentity.png | company | URL of company logo | string | 0 | 2000 | true | property | 
 | ciam_magicLinkEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_passwordlessRequired##SK##company | false | company |  | boolean | 0 | 2000 | false | property | 
 | ciam_protectDeviceStatus##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne protect flow | string | 0 | 2000 | true | property | 
 | ciam_protectPredictor##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne Protect flows. | string | 0 | 2000 | true | property | 
 | ciam_protectRiskID##SK##flowInstance |  | flowInstance | This variable is used by CIAM Passwordless with pingone protect flows. | string | 0 | 2000 | true | property | 
 | ciam_protectRiskLevel##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne protect flows | string | 0 | 2000 | true | property | 
 | ciam_protectriskPolicyId##SK##flowInstance |  | flowInstance | This PingOne Protect Risk Policy ID will be passed by default. | string | 0 | 2000 | true | property | 
 | ciam_sessionLengthInMinute##SK##company | 5 | company |  | number | 0 | 2000 | false | property | 
 | ciam_smsOtpEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 

### Custom CSS
~> Note: Custom CSS is applied to every node in the flow

```css
.companyLogo {
    /* Ping Logo  */
    content: url("https://assets.pingone.com/ux/ui-library/5.0.2/images/logo-pingidentity.png");
    width: 65px;
    height: 65px;
}
```
