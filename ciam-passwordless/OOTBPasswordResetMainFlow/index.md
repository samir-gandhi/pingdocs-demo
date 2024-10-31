# OOTB - Password Reset - Main Flow

### Flow Diagram
```mermaid
flowchart LR
    avwmu6hzfh(("Evaluator")) --> wivhffesg6[["Teleport"]]
    52llz5ttng[["NOP UI Page"]] --> zbtrq27f5e(("EVAL"))
    h0oa9r1emk[["Change Password"]] --> 1xqdfym9yi(("EVAL"))
    0lyofgg9w1(("EVAL")) --> 52llz5ttng[["NOP UI Page"]]
    avwmu6hzfh(("Evaluator")) --> scja20ci5q[["Check If User Exists"]]
    qwwhmi6a6f[["Error Message"]] --> ppo83pmk4y(("EVAL"))
    scja20ci5q[["Check If User Exists"]] --> ld5015scb0(("EVAL"))
    0lyofgg9w1(("EVAL")) --> jivvj39cj7[["Teleport"]]
    ld5015scb0(("EVAL")) --> 4ujhiqp37g[["Teleport"]]
    ppo83pmk4y(("EVAL")) --> gyupuyv0tq[["Error Screen"]]
    40jmo5fihf[["Does user currently have password?"]] --> 0lyofgg9w1(("EVAL"))
    ld5015scb0(("EVAL")) --> 40jmo5fihf[["Does user currently have password?"]]
    zbtrq27f5e(("EVAL")) --> h0oa9r1emk[["Change Password"]]
    gyupuyv0tq[["Error Screen"]] --> kydkhvfnus(("EVAL"))
    7yrdpb4c81[["Set Flow Variables"]] --> avwmu6hzfh(("Evaluator"))
    1xqdfym9yi(("EVAL")) --> vx22j0r8wh[["Teleport"]]
    z9ium51c7v[["Send Success Response"]] --> fkin2w5zxa(("Evaluator"))
    fkin2w5zxa(("Evaluator")) --> x1qqx7ulgc[["Teleport"]]
    0r9p2q13sc(("EVAL")) --> z9ium51c7v[["Send Success Response"]]
    dyim6odd0k[["Success"]] --> 0r9p2q13sc(("EVAL"))
    kydkhvfnus(("EVAL")) --> yihsm2demx[["Send Response"]]


```

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
 




## Subflows
| Label | Capatability Name | Node ID | Node Title | Version ID |                                                                                                                                                             
|----------------------------------|-----------------|-----------------|-----------------|-----------------|
| [OOTB - Change Password - Subflow - 1](../OOTBChangePasswordSubflow1/index.md) | startUiSubFlow | [h0oa9r1emk](./nodes/h0oa9r1emk.md) | Change Password | -1 | 
 