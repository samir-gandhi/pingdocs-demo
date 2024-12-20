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
| [2btocnrvnp](./nodes/2btocnrvnp.md) | Annotation | Detect Threat using PingOne | 
 | [5vw8zhr390](./nodes/5vw8zhr390.md) | Annotation | CIAM-Passwordless-Protect-Threat-Detection-Subflow | 
 | [7i8834bmpf](./nodes/7i8834bmpf.md) | Annotation | Take action based on threat detected. Visit PingOne Protect documentation for more information on this. | 
 | [ahgaglnbf3](./nodes/ahgaglnbf3.md) | Annotation | Error while Creating Protect Risk Evaluation. | 
 | [c2ulwnph9p](./nodes/c2ulwnph9p.md) | Detect Threat | Check if PingOne protect has detected a BOT or AITM attack | 
 | [cilec71mva](./nodes/cilec71mva.md) | Annotation | Input Schema:  required are: skriskcomponent, userName, flowType, ipAddress and optional are: userID, applicationId, SessionId, riskPolicyID, customAttributes | 
 | [eagfn3lpbp](./nodes/eagfn3lpbp.md) | Return Success Response |  | 
 | [f994y44c9q](./nodes/f994y44c9q.md) | Error While creating a risk evaluation | Error While creating PingOne Protect Risk Evaluation | 
 | [ggprsb233e](./nodes/ggprsb233e.md) | Annotation | Input Schema: Configure the Environment ID, ClientID, Client Secret and Region in PingOne Protect Connector. | 
 | [h48xdltldb](./nodes/h48xdltldb.md) | Annotation | If existing user then disable them in main flow. | 
 | [k6hynhaety](./nodes/k6hynhaety.md) | Threat detected response. | Response back when a threat is detected. | 
 | [md3luzzdte](./nodes/md3luzzdte.md) | Annotation | More details: https://apidocs.pingidentity.com/pingone/platform/v1/api/#put-update-risk-evaluation | 
 | [onzp625tsa](./nodes/onzp625tsa.md) | Annotation | Sends back: PingOne Risk Level, PignOne Risk ID, PingOne Recommended Action values. | 
 | [qbf0qv8qi0](./nodes/qbf0qv8qi0.md) | Flow Configuration Check | Add input variables to check for null/empty | 
 | [ue7utb27ym](./nodes/ue7utb27ym.md) | Error Message | Configuration value not set error | 
 | [y5vtbd5ej5](./nodes/y5vtbd5ej5.md) | Annotation | Create Protect Risk Evaluation after getting required inputs. | 
 | [y6rdbg2ky5](./nodes/y6rdbg2ky5.md) | Create PingOne Protect Risk with user and Environment details | Should have required variables to start the risk evaluation. | 
 