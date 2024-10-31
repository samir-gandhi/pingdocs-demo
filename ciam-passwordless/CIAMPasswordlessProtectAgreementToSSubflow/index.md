# CIAM-Passwordless-Protect-Agreement(ToS)-Subflow

### Flow Diagram
```mermaid
flowchart LR
    gjg587c8af(("Evaluator")) --> yqx4phhtcl[["Node"]]
    ldx8d6ahwt(("EVAL")) --> 4qv73tz0ug[["Accept Agreement"]]
    6xfm9lpclg(("EVAL")) --> canivkxqjq[["Node"]]
    4h6hi1onkj(("Evaluator")) --> 6pm1x665h0[["Node"]]
    h22w6agh1(("Evaluator")) --> 1rvj1fvgpu[["Check If Consent Status Is Accepted"]]
    prjjhhmndv(("Evaluator")) --> 8jemlov0oc[["Check User Consent Status"]]
    6x74clj9zm[["Check For User Consent?"]] --> prjjhhmndv(("Evaluator"))
    1rvj1fvgpu[["Check If Consent Status Is Accepted"]] --> 4h6hi1onkj(("Evaluator"))
    2vij7q7i5j(("EVAL")) --> v68793bc1v[["Is Agreement Enabled?"]]
    v68793bc1v[["Is Agreement Enabled?"]] --> 6xfm9lpclg(("EVAL"))
    6xfm9lpclg(("EVAL")) --> 6x74clj9zm[["Check For User Consent?"]]
    prjjhhmndv(("Evaluator")) --> 8zvqjrwsj8[["Node"]]
    jcpocm4del(("EVAL")) --> ph62v3m7kl[["Decline Agreement"]]
    4qv73tz0ug[["Accept Agreement"]] --> npztwu892l(("EVAL"))
    it43isf5sm(("EVAL")) --> 8x2gjjcvxj[["Check User Action"]]
    4h6hi1onkj(("Evaluator")) --> 8zvqjrwsj8[["Node"]]
    je23nstva5(("EVAL")) --> 8ytvupm9en[["Get Agreement"]]
    8ytvupm9en[["Get Agreement"]] --> gjg587c8af(("Evaluator"))
    npztwu892l(("EVAL")) --> 3koaafiiox[["Node"]]
    8x2gjjcvxj[["Check User Action"]] --> jcpocm4del(("EVAL"))
    qhcqow5g8y[["Ask for agreement"]] --> je23nstva5(("EVAL"))
    h22w6agh1(("Evaluator")) --> 8zvqjrwsj8[["Node"]]
    8jemlov0oc[["Check User Consent Status"]] --> h22w6agh1(("Evaluator"))
    pt563yeug9[["Success"]] --> vomegm9y96(("EVAL"))
    vomegm9y96(("EVAL")) --> o5cgjow8id[["Return Success Response"]]
    8x2gjjcvxj[["Check User Action"]] --> ldx8d6ahwt(("EVAL"))
    gjg587c8af(("Evaluator")) --> 0h8so1sxqq[["Agreement Form"]]
    0h8so1sxqq[["Agreement Form"]] --> it43isf5sm(("EVAL"))
    64hrke1krq[["NOP UI Page"]] --> 2vij7q7i5j(("EVAL"))
    zv66jvh5ja[["Error"]] --> 0m7rxlhf9o(("EVAL"))
    0m7rxlhf9o(("EVAL")) --> zgq483nez5[["Return Error Response"]]
    npztwu892l(("EVAL")) --> hb77by4606[["Node"]]


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
| checkRequired | To check if user has consent before directing user to agreement | true | textField | boolean | true | 
 | pingOneUserId |  | true | textField | string | true | 
 | ciam_agreementId |  | true | textField | string | false | 
 | ciam_agreementEnabled |  | true | textField | boolean | false | 
 | ciam_companyLogo |  | true | textField | string | false | 
 



