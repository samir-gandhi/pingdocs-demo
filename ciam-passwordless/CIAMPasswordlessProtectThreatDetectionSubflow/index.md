# CIAM-Passwordless-Protect-Threat-Detection-Subflow

![Flowchart Diagram](CIAMPasswordlessProtectThreatDetectionSubflow.svg) 

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
 



## Node List
| Node ID | Title | Description |
|----------------------------------|-----------------|-----------------|
| [2btocnrvnp](./nodes/2btocnrvnp.md) | Annotation |  | 
 | [5vw8zhr390](./nodes/5vw8zhr390.md) | Annotation |  | 
 | [7i8834bmpf](./nodes/7i8834bmpf.md) | Annotation |  | 
 | [ahgaglnbf3](./nodes/ahgaglnbf3.md) | Annotation |  | 
 | [c2ulwnph9p](./nodes/c2ulwnph9p.md) | Detect Threat | Check if PingOne protect has detected a BOT or AITM attack | 
 | [cilec71mva](./nodes/cilec71mva.md) | Annotation |  | 
 | [eagfn3lpbp](./nodes/eagfn3lpbp.md) | Return Success Response |  | 
 | [f994y44c9q](./nodes/f994y44c9q.md) | Error While creating a risk evaluation | Error While creating PingOne Protect Risk Evaluation | 
 | [ggprsb233e](./nodes/ggprsb233e.md) | Annotation |  | 
 | [h48xdltldb](./nodes/h48xdltldb.md) | Annotation |  | 
 | [k6hynhaety](./nodes/k6hynhaety.md) | Threat detected response. | Response back when a threat is detected. | 
 | [md3luzzdte](./nodes/md3luzzdte.md) | Annotation |  | 
 | [onzp625tsa](./nodes/onzp625tsa.md) | Annotation |  | 
 | [qbf0qv8qi0](./nodes/qbf0qv8qi0.md) | Flow Configuration Check | Add input variables to check for null/empty | 
 | [ue7utb27ym](./nodes/ue7utb27ym.md) | Error Message | Configuration value not set error | 
 | [y5vtbd5ej5](./nodes/y5vtbd5ej5.md) | Annotation |  | 
 | [y6rdbg2ky5](./nodes/y6rdbg2ky5.md) | Create PingOne Protect Risk with user and Environment details | Should have required variables to start the risk evaluation. | 
 