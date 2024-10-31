# OOTB - Change Password - Subflow - 1

### Flow Diagram
```mermaid
flowchart LR
    md8472gv2e[["Show Success"]] --> v738ey1b5y(("EVAL"))
    ixq0pq1td7(("EVAL")) --> 5vfn623mx7[["Display password reset form"]]
    mjqbph9elz(("Evaluator")) --> ur66q695u0[["Teleport"]]
    d3ziqry02i(("EVAL")) --> yo6nv4gud2[["Teleport"]]
    d3ziqry02i(("EVAL")) --> jn53bcmsnv[["Boolean Check"]]
    w0jz1dtx27[["Verify Passwords Match"]] --> 6oeo7c9bch(("Evaluator"))
    6oeo7c9bch(("Evaluator")) --> 7eaxdz9nwk[["Update password"]]
    h330sqhk7o[["Empty Check"]] --> d3ziqry02i(("EVAL"))
    mjqbph9elz(("Evaluator")) --> ut2v2s6fqq[["Teleport"]]
    75iq81515r[["Password reset submit?"]] --> o5jvuf0bwl(("EVAL"))
    79lag5unyk[["NOP UI Page"]] --> a3oth8yspq(("EVAL"))
    a3oth8yspq(("EVAL")) --> 5vfn623mx7[["Display password reset form"]]
    ateb0l10nl(("Evaluator")) --> h330sqhk7o[["Empty Check"]]
    jn53bcmsnv[["Boolean Check"]] --> mjqbph9elz(("Evaluator"))
    o5jvuf0bwl(("EVAL")) --> dcq4ib3mce[["Teleport"]]
    6oeo7c9bch(("Evaluator")) --> 2m4whqb1dr[["Passwords dont match"]]
    wv79oxt1fo(("EVAL")) --> 9pswmi4mi1[["Teleport"]]
    brpmsv8uag[["Success Error"]] --> b900rty9pd(("EVAL"))
    30owhg6lfp(("EVAL")) --> 75iq81515r[["Password reset submit?"]]
    2inl0soj3i(("EVAL")) --> w0jz1dtx27[["Verify Passwords Match"]]
    7eaxdz9nwk[["Update password"]] --> ateb0l10nl(("Evaluator"))
    8qr5bc3clq[["Success"]] --> jf9akdpa1q(("EVAL"))
    5vfn623mx7[["Display password reset form"]] --> 30owhg6lfp(("EVAL"))
    75iq81515r[["Password reset submit?"]] --> 2inl0soj3i(("EVAL"))
    4tnam70cjm[["Send Success Response"]] --> 2znw6pakac(("Evaluator"))
    75iq81515r[["Password reset submit?"]] --> wv79oxt1fo(("EVAL"))
    b900rty9pd(("EVAL")) --> hxmqf7sb52[["Send Error Response"]]
    ateb0l10nl(("Evaluator")) --> tfn7o3aug6[["Password update failed"]]
    jf9akdpa1q(("EVAL")) --> 4tnam70cjm[["Send Success Response"]]
    2znw6pakac(("Evaluator")) --> uj42vvvgjt[["Teleport"]]
    v738ey1b5y(("EVAL")) --> xo4l1ngx8q[["NOP UI Page"]]
    xo4l1ngx8q[["NOP UI Page"]] --> ixq0pq1td7(("EVAL"))


```

## Settings
An exhaustive list of settings including defaults.
| Setting                          | Value                                                                                                                                                                                   |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSP Value                        | worker-src &#39;self&#39; blob:; script-src &#39;self&#39; https://cdn.jsdelivr.net https://code.jquery.com https://devsdk.singularkey.com http://cdnjs.cloudflare.com &#39;unsafe-inline&#39; &#39;unsafe-eval&#39;; | 
 | CSS Links                        | https://assets.pingone.com/ux/end-user-nano/0.1.0-alpha.0/end-user-nano.css,https://assets.pingone.com/ux/astro-nano/0.1.0-alpha.6/icons.css|

## Input Schemas
| Property Name | Description | Expanded | Preferred Control Type | Preferred Data Type | Required |
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| userID |  | true | textField | string | true | 
 | showSuccessMessage |  | true | textField | boolean | false | 
 | ciam_companyLogo |  | true | textField | string | false | 
 



