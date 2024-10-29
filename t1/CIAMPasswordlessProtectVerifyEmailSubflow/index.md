# CIAM-Passwordless-Protect-Verify-Email-Subflow

### Flow Diagram
```mermaid
flowchart LR
    r8sc175hhf(("EVAL")) --> wweoq86mfw["Return Success Response"]
    hpve55zazv(("EVAL")) --> gf3bwis6oi["Node"]
    ru45xolut1(("EVAL")) --> 5d5o5ia81u["Is Validation Limit Reached?"]
    rjau0njx5i["Form Button Check"] --> t92nqcnwux(("EVAL"))
    rjau0njx5i["Form Button Check"] --> n5icn97kyh(("EVAL"))
    8l8a54vefk(("Evaluator")) --> ab91zkjrgx["Node"]
    hpve55zazv(("EVAL")) --> 1vyzcyazgf["Validate verification code"]
    sju60xf677(("EVAL")) --> rjau0njx5i["Form Button Check"]
    8l8a54vefk(("Evaluator")) --> 527m4tr2s2["Verification Code Resent"]
    n5icn97kyh(("EVAL")) --> 9lrqw38492["Resend Verification Code"]
    xsb00g2t92["Set Validation Attempt To Zero"] --> qskpbqg2yf(("EVAL"))
    qskpbqg2yf(("EVAL")) --> s5yykzv8zd["Prompt For Verification Code"]
    5d5o5ia81u["Is Validation Limit Reached?"] --> hpve55zazv(("EVAL"))
    r8sc175hhf(("EVAL")) --> 8gqiq4sagn["Could not validate the verification code"]
    t92nqcnwux(("EVAL")) --> wfe8dz7k7v["Increment Validation Attempt"]
    1vyzcyazgf["Validate verification code"] --> r8sc175hhf(("EVAL"))
    wfe8dz7k7v["Increment Validation Attempt"] --> ru45xolut1(("EVAL"))
    9lrqw38492["Resend Verification Code"] --> 8l8a54vefk(("Evaluator"))
    s5yykzv8zd["Prompt For Verification Code"] --> sju60xf677(("EVAL"))
    xbvfnq8o31["Error"] --> 90g8cf6l2u(("EVAL"))
    90g8cf6l2u(("EVAL")) --> rfo66ayuok["Return Error Response"]

    click r8sc175hhf "vscode://file/./nodes/r8sc175hhf.md" _parent
    click wweoq86mfw "vscode://file/./nodes/wweoq86mfw.md" _parent
    click hpve55zazv "vscode://file/./nodes/hpve55zazv.md" _parent
    click gf3bwis6oi "vscode://file/./nodes/gf3bwis6oi.md" _parent
    click ru45xolut1 "vscode://file/./nodes/ru45xolut1.md" _parent
    click 5d5o5ia81u "vscode://file/./nodes/5d5o5ia81u.md" _parent
    click rjau0njx5i "vscode://file/./nodes/rjau0njx5i.md" _parent
    click t92nqcnwux "vscode://file/./nodes/t92nqcnwux.md" _parent
    click rjau0njx5i "vscode://file/./nodes/rjau0njx5i.md" _parent
    click n5icn97kyh "vscode://file/./nodes/n5icn97kyh.md" _parent
    click 8l8a54vefk "vscode://file/./nodes/8l8a54vefk.md" _parent
    click ab91zkjrgx "vscode://file/./nodes/ab91zkjrgx.md" _parent
    click hpve55zazv "vscode://file/./nodes/hpve55zazv.md" _parent
    click 1vyzcyazgf "vscode://file/./nodes/1vyzcyazgf.md" _parent
    click sju60xf677 "vscode://file/./nodes/sju60xf677.md" _parent
    click rjau0njx5i "vscode://file/./nodes/rjau0njx5i.md" _parent
    click 8l8a54vefk "vscode://file/./nodes/8l8a54vefk.md" _parent
    click 527m4tr2s2 "vscode://file/./nodes/527m4tr2s2.md" _parent
    click n5icn97kyh "vscode://file/./nodes/n5icn97kyh.md" _parent
    click 9lrqw38492 "vscode://file/./nodes/9lrqw38492.md" _parent
    click xsb00g2t92 "vscode://file/./nodes/xsb00g2t92.md" _parent
    click qskpbqg2yf "vscode://file/./nodes/qskpbqg2yf.md" _parent
    click qskpbqg2yf "vscode://file/./nodes/qskpbqg2yf.md" _parent
    click s5yykzv8zd "vscode://file/./nodes/s5yykzv8zd.md" _parent
    click 5d5o5ia81u "vscode://file/./nodes/5d5o5ia81u.md" _parent
    click hpve55zazv "vscode://file/./nodes/hpve55zazv.md" _parent
    click r8sc175hhf "vscode://file/./nodes/r8sc175hhf.md" _parent
    click 8gqiq4sagn "vscode://file/./nodes/8gqiq4sagn.md" _parent
    click t92nqcnwux "vscode://file/./nodes/t92nqcnwux.md" _parent
    click wfe8dz7k7v "vscode://file/./nodes/wfe8dz7k7v.md" _parent
    click 1vyzcyazgf "vscode://file/./nodes/1vyzcyazgf.md" _parent
    click r8sc175hhf "vscode://file/./nodes/r8sc175hhf.md" _parent
    click wfe8dz7k7v "vscode://file/./nodes/wfe8dz7k7v.md" _parent
    click ru45xolut1 "vscode://file/./nodes/ru45xolut1.md" _parent
    click 9lrqw38492 "vscode://file/./nodes/9lrqw38492.md" _parent
    click 8l8a54vefk "vscode://file/./nodes/8l8a54vefk.md" _parent
    click s5yykzv8zd "vscode://file/./nodes/s5yykzv8zd.md" _parent
    click sju60xf677 "vscode://file/./nodes/sju60xf677.md" _parent
    click xbvfnq8o31 "vscode://file/./nodes/xbvfnq8o31.md" _parent
    click 90g8cf6l2u "vscode://file/./nodes/90g8cf6l2u.md" _parent
    click 90g8cf6l2u "vscode://file/./nodes/90g8cf6l2u.md" _parent
    click rfo66ayuok "vscode://file/./nodes/rfo66ayuok.md" _parent
```


## Settings
An exhaustive list of settings including defaults.
| Setting                          | Value                                                                                                                                                                                   |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSP Value                        | worker-src &#39;self&#39; blob:; script-src &#39;self&#39; https://cdn.jsdelivr.net https://code.jquery.com https://devsdk.singularkey.com http://cdnjs.cloudflare.com &#39;unsafe-inline&#39; &#39;unsafe-eval&#39;; | 
 | CSS Links                        | |

## Input Schemas
| Property Name | Description | Expanded | Preferred Control Type | Preferred Data Type | Required |
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| pingOneUserId |  | true | textField | string | true | 
 | ciam_companyLogo |  | true | textField | string | false | 
 


## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| ciam_verificationValidationAttempts##SK##flowInstance |  | flowInstance |  | number | 0 | 2000 | true | property | 
 | ciam_verificationLimit##SK##company | 5 | company |  | number | 0 | 2000 | false | property | 
 

### Custom CSS
~> Note: Custom CSS is applied to every node in the flow

```css

```
