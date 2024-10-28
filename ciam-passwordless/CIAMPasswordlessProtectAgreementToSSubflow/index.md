# CIAM-Passwordless-Protect-Agreement(ToS)-Subflow
Description: Imported on Thu Oct 24 2024 20:38:12 GMT&#43;0000 (Coordinated Universal Time) 


## Settings
An exhaustive list of settings including defaults.
| Setting                          | Value                                                                                                                                                                                   |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSP Value                        | worker-src &#39;self&#39; blob:; script-src &#39;self&#39; https://cdn.jsdelivr.net https://code.jquery.com https://devsdk.singularkey.com http://cdnjs.cloudflare.com &#39;unsafe-inline&#39; &#39;unsafe-eval&#39;; | 
 | CSS Links                        | |

## Input Schemas
| Property Name | Description | Expanded | Preferred Control Type | Preferred Data Type | Required |
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| checkRequired | To check if user has consent before directing user to agreement | true | textField | boolean | true | 
 | pingOneUserId |  | true | textField | string | true | 
 | ciam_agreementId |  | true | textField | string | false | 
 | ciam_agreementEnabled |  | true | textField | boolean | false | 
 | ciam_companyLogo |  | true | textField | string | false | 
 



### Custom CSS
~> Note: Custom CSS is applied to every node in the flow

```css

```


### Flow Diagram
```mermaid
flowchart LR
    gjg587c8af((Evaluator)) --> yqx4phhtcl[Node]
    ldx8d6ahwt((EVAL)) --> 4qv73tz0ug[Accept Agreement]
    6xfm9lpclg((EVAL)) --> canivkxqjq[Node]
    4h6hi1onkj((Evaluator)) --> 6pm1x665h0[Node]
    h22w6agh1((Evaluator)) --> 1rvj1fvgpu[Check If Consent Status Is Accepted]
    prjjhhmndv((Evaluator)) --> 8jemlov0oc[Check User Consent Status]
    6x74clj9zm[Check For User Consent?] --> prjjhhmndv((Evaluator))
    1rvj1fvgpu[Check If Consent Status Is Accepted] --> 4h6hi1onkj((Evaluator))
    2vij7q7i5j((EVAL)) --> v68793bc1v[Is Agreement Enabled?]
    v68793bc1v[Is Agreement Enabled?] --> 6xfm9lpclg((EVAL))
    6xfm9lpclg((EVAL)) --> 6x74clj9zm[Check For User Consent?]
    prjjhhmndv((Evaluator)) --> 8zvqjrwsj8[Node]
    jcpocm4del((EVAL)) --> ph62v3m7kl[Decline Agreement]
    4qv73tz0ug[Accept Agreement] --> npztwu892l((EVAL))
    it43isf5sm((EVAL)) --> 8x2gjjcvxj[Check User Action]
    4h6hi1onkj((Evaluator)) --> 8zvqjrwsj8[Node]
    je23nstva5((EVAL)) --> 8ytvupm9en[Get Agreement]
    8ytvupm9en[Get Agreement] --> gjg587c8af((Evaluator))
    npztwu892l((EVAL)) --> 3koaafiiox[Node]
    8x2gjjcvxj[Check User Action] --> jcpocm4del((EVAL))
    qhcqow5g8y[Ask for agreement] --> je23nstva5((EVAL))
    h22w6agh1((Evaluator)) --> 8zvqjrwsj8[Node]
    8jemlov0oc[Check User Consent Status] --> h22w6agh1((Evaluator))
    pt563yeug9[Success] --> vomegm9y96((EVAL))
    vomegm9y96((EVAL)) --> o5cgjow8id[Return Success Response]
    8x2gjjcvxj[Check User Action] --> ldx8d6ahwt((EVAL))
    gjg587c8af((Evaluator)) --> 0h8so1sxqq[Agreement Form]
    0h8so1sxqq[Agreement Form] --> it43isf5sm((EVAL))
    64hrke1krq[NOP UI Page] --> 2vij7q7i5j((EVAL))
    zv66jvh5ja[Error] --> 0m7rxlhf9o((EVAL))
    0m7rxlhf9o((EVAL)) --> zgq483nez5[Return Error Response]
    npztwu892l((EVAL)) --> hb77by4606[Node]

    click gjg587c8af "gjg587c8af" "gjg587c8af"
    click yqx4phhtcl "yqx4phhtcl" "yqx4phhtcl"
    click ldx8d6ahwt "ldx8d6ahwt" "ldx8d6ahwt"
    click 4qv73tz0ug "4qv73tz0ug" "4qv73tz0ug"
    click 6xfm9lpclg "6xfm9lpclg" "6xfm9lpclg"
    click canivkxqjq "canivkxqjq" "canivkxqjq"
    click 4h6hi1onkj "4h6hi1onkj" "4h6hi1onkj"
    click 6pm1x665h0 "6pm1x665h0" "6pm1x665h0"
    click h22w6agh1 "h22w6agh1" "h22w6agh1"
    click 1rvj1fvgpu "1rvj1fvgpu" "1rvj1fvgpu"
    click prjjhhmndv "prjjhhmndv" "prjjhhmndv"
    click 8jemlov0oc "8jemlov0oc" "8jemlov0oc"
    click 6x74clj9zm "6x74clj9zm" "6x74clj9zm"
    click prjjhhmndv "prjjhhmndv" "prjjhhmndv"
    click 1rvj1fvgpu "1rvj1fvgpu" "1rvj1fvgpu"
    click 4h6hi1onkj "4h6hi1onkj" "4h6hi1onkj"
    click 2vij7q7i5j "2vij7q7i5j" "2vij7q7i5j"
    click v68793bc1v "v68793bc1v" "v68793bc1v"
    click v68793bc1v "v68793bc1v" "v68793bc1v"
    click 6xfm9lpclg "6xfm9lpclg" "6xfm9lpclg"
    click 6xfm9lpclg "6xfm9lpclg" "6xfm9lpclg"
    click 6x74clj9zm "6x74clj9zm" "6x74clj9zm"
    click prjjhhmndv "prjjhhmndv" "prjjhhmndv"
    click 8zvqjrwsj8 "8zvqjrwsj8" "8zvqjrwsj8"
    click jcpocm4del "jcpocm4del" "jcpocm4del"
    click ph62v3m7kl "ph62v3m7kl" "ph62v3m7kl"
    click 4qv73tz0ug "4qv73tz0ug" "4qv73tz0ug"
    click npztwu892l "npztwu892l" "npztwu892l"
    click it43isf5sm "it43isf5sm" "it43isf5sm"
    click 8x2gjjcvxj "8x2gjjcvxj" "8x2gjjcvxj"
    click 4h6hi1onkj "4h6hi1onkj" "4h6hi1onkj"
    click 8zvqjrwsj8 "8zvqjrwsj8" "8zvqjrwsj8"
    click je23nstva5 "je23nstva5" "je23nstva5"
    click 8ytvupm9en "8ytvupm9en" "8ytvupm9en"
    click 8ytvupm9en "8ytvupm9en" "8ytvupm9en"
    click gjg587c8af "gjg587c8af" "gjg587c8af"
    click npztwu892l "npztwu892l" "npztwu892l"
    click 3koaafiiox "3koaafiiox" "3koaafiiox"
    click 8x2gjjcvxj "8x2gjjcvxj" "8x2gjjcvxj"
    click jcpocm4del "jcpocm4del" "jcpocm4del"
    click qhcqow5g8y "qhcqow5g8y" "qhcqow5g8y"
    click je23nstva5 "je23nstva5" "je23nstva5"
    click h22w6agh1 "h22w6agh1" "h22w6agh1"
    click 8zvqjrwsj8 "8zvqjrwsj8" "8zvqjrwsj8"
    click 8jemlov0oc "8jemlov0oc" "8jemlov0oc"
    click h22w6agh1 "h22w6agh1" "h22w6agh1"
    click pt563yeug9 "pt563yeug9" "pt563yeug9"
    click vomegm9y96 "vomegm9y96" "vomegm9y96"
    click vomegm9y96 "vomegm9y96" "vomegm9y96"
    click o5cgjow8id "o5cgjow8id" "o5cgjow8id"
    click 8x2gjjcvxj "8x2gjjcvxj" "8x2gjjcvxj"
    click ldx8d6ahwt "ldx8d6ahwt" "ldx8d6ahwt"
    click gjg587c8af "gjg587c8af" "gjg587c8af"
    click 0h8so1sxqq "0h8so1sxqq" "0h8so1sxqq"
    click 0h8so1sxqq "0h8so1sxqq" "0h8so1sxqq"
    click it43isf5sm "it43isf5sm" "it43isf5sm"
    click 64hrke1krq "64hrke1krq" "64hrke1krq"
    click 2vij7q7i5j "2vij7q7i5j" "2vij7q7i5j"
    click zv66jvh5ja "zv66jvh5ja" "zv66jvh5ja"
    click 0m7rxlhf9o "0m7rxlhf9o" "0m7rxlhf9o"
    click 0m7rxlhf9o "0m7rxlhf9o" "0m7rxlhf9o"
    click zgq483nez5 "zgq483nez5" "zgq483nez5"
    click npztwu892l "npztwu892l" "npztwu892l"
    click hb77by4606 "hb77by4606" "hb77by4606"
```
