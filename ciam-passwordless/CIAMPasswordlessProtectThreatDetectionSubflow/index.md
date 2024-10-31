# CIAM-Passwordless-Protect-Threat-Detection-Subflow

### Flow Diagram
```mermaid
flowchart LR
    6b03psy0ol(("EVAL")) --> ue7utb27ym[["Error Message"]]
    uizc04ybxq(("Evaluator")) --> k6hynhaety[["Threat detected response."]]
    uizc04ybxq(("Evaluator")) --> eagfn3lpbp[["Return Success Response"]]
    y6rdbg2ky5[["Create PingOne Protect Risk with user and Environment details"]] --> vknqtnu7y2(("EVAL"))
    c2ulwnph9p[["Detect Threat"]] --> uizc04ybxq(("Evaluator"))
    vknqtnu7y2(("EVAL")) --> f994y44c9q[["Error While creating a risk evaluation"]]
    vknqtnu7y2(("EVAL")) --> c2ulwnph9p[["Detect Threat"]]
    6b03psy0ol(("EVAL")) --> y6rdbg2ky5[["Create PingOne Protect Risk with user and Environment details"]]
    qbf0qv8qi0[["Flow Configuration Check"]] --> 6b03psy0ol(("EVAL"))


```

## Settings
An exhaustive list of settings including defaults.
| Setting                          | Value                                                                                                                                                                                   |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSP Value                        | worker-src &#39;self&#39; blob:; script-src &#39;self&#39; https://cdn.jsdelivr.net https://code.jquery.com https://devsdk.singularkey.com http://cdnjs.cloudflare.com &#39;unsafe-inline&#39; &#39;unsafe-eval&#39;; | 
 |

## Input Schemas
| Property Name | Description | Expanded | Preferred Control Type | Preferred Data Type | Required |
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| skriskcomponent | PingOne Protect skrisk component | true | textField | string | true | 
 | userName | UserName to be passed to PingOne Protect | true | textField | string | true | 
 | riskPolicyID | Risk Policy ID to be passed to PingOne Protect | true | textField | string | true | 
 | flowType | Flow Type to be passed to PingOne Protect | true | textField | string | true | 
 | ipAddress | user IP Address to be passed to PingOne Protect | true | textField | string | true | 
 | userID | The User ID to be passed to PingOne Protect | true | textField | string | false | 
 | applicationId | ApplicationId to be passed to PingOne Protect | true | textField | string | false | 
 | SessionId | Session Id to be passed to PingOne Protect | true | textField | string | false | 
 | customAttributes | Custom Attributes in PingOne Environment to be passed to PingOne Protect | true | textField | string | false | 
 | userAgent | PingOne Protect User Agent to trigger flow. | true | textField | string | false | 
 | usercookie | PingOne Protect User Cookie to trigger flow. | true | textField | string | false | 
 


## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| companyName##SK##flowInstance |  | flowInstance |  | string | 0 | 2000 | true | property | 
 

