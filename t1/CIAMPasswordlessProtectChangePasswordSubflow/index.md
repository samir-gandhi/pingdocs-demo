# CIAM-Passwordless-Protect-Change-Password-Subflow

### Flow Diagram
```mermaid
flowchart LR
    v738ey1b5y(("EVAL")) --> xo4l1ngx8q["NOP UI Page"]
    md8472gv2e["Show Success"] --> v738ey1b5y(("EVAL"))
    ixq0pq1td7(("EVAL")) --> 5vfn623mx7["Display password reset form"]
    mjqbph9elz(("Evaluator")) --> ur66q695u0["Node"]
    d3ziqry02i(("EVAL")) --> yo6nv4gud2["Node"]
    d3ziqry02i(("EVAL")) --> jn53bcmsnv["Boolean Check"]
    w0jz1dtx27["Verify Passwords Match"] --> 6oeo7c9bch(("Evaluator"))
    6oeo7c9bch(("Evaluator")) --> 7eaxdz9nwk["Update password"]
    h330sqhk7o["Empty Check"] --> d3ziqry02i(("EVAL"))
    mjqbph9elz(("Evaluator")) --> ut2v2s6fqq["Node"]
    75iq81515r["Password reset submit?"] --> o5jvuf0bwl(("EVAL"))
    79lag5unyk["NOP UI Page"] --> a3oth8yspq(("EVAL"))
    a3oth8yspq(("EVAL")) --> 5vfn623mx7["Display password reset form"]
    ateb0l10nl(("Evaluator")) --> h330sqhk7o["Empty Check"]
    jn53bcmsnv["Boolean Check"] --> mjqbph9elz(("Evaluator"))
    o5jvuf0bwl(("EVAL")) --> dcq4ib3mce["Node"]
    6oeo7c9bch(("Evaluator")) --> 2m4whqb1dr["Passwords don&#39;t match"]
    wv79oxt1fo(("EVAL")) --> 9pswmi4mi1["Node"]
    brpmsv8uag["Success Error"] --> b900rty9pd(("EVAL"))
    30owhg6lfp(("EVAL")) --> 75iq81515r["Password reset submit?"]
    2inl0soj3i(("EVAL")) --> w0jz1dtx27["Verify Passwords Match"]
    7eaxdz9nwk["Update password"] --> ateb0l10nl(("Evaluator"))
    8qr5bc3clq["Success"] --> jf9akdpa1q(("EVAL"))
    5vfn623mx7["Display password reset form"] --> 30owhg6lfp(("EVAL"))
    75iq81515r["Password reset submit?"] --> 2inl0soj3i(("EVAL"))
    4tnam70cjm["Send Success Response"] --> 2znw6pakac(("Evaluator"))
    75iq81515r["Password reset submit?"] --> wv79oxt1fo(("EVAL"))
    b900rty9pd(("EVAL")) --> hxmqf7sb52["Send Error Response"]
    xo4l1ngx8q["NOP UI Page"] --> ixq0pq1td7(("EVAL"))
    jf9akdpa1q(("EVAL")) --> 4tnam70cjm["Send Success Response"]
    2znw6pakac(("Evaluator")) --> uj42vvvgjt["Node"]
    ym31re8b7g(("EVAL")) --> okw0g6i84d["Update error message"]
    um3lcpaulo(("EVAL")) --> abmzqz1u6f["Invalid password"]
    okw0g6i84d["Update error message"] --> um3lcpaulo(("EVAL"))
    rysh2x3iz2["Set error message"] --> ym31re8b7g(("EVAL"))
    ateb0l10nl(("Evaluator")) --> rysh2x3iz2["Set error message"]
    6oeo7c9bch(("Evaluator")) --> t0vllny9q["Http"]

    click v738ey1b5y "vscode://file/./nodes/v738ey1b5y.md" _parent
    click xo4l1ngx8q "vscode://file/./nodes/xo4l1ngx8q.md" _parent
    click md8472gv2e "vscode://file/./nodes/md8472gv2e.md" _parent
    click v738ey1b5y "vscode://file/./nodes/v738ey1b5y.md" _parent
    click ixq0pq1td7 "vscode://file/./nodes/ixq0pq1td7.md" _parent
    click 5vfn623mx7 "vscode://file/./nodes/5vfn623mx7.md" _parent
    click mjqbph9elz "vscode://file/./nodes/mjqbph9elz.md" _parent
    click ur66q695u0 "vscode://file/./nodes/ur66q695u0.md" _parent
    click d3ziqry02i "vscode://file/./nodes/d3ziqry02i.md" _parent
    click yo6nv4gud2 "vscode://file/./nodes/yo6nv4gud2.md" _parent
    click d3ziqry02i "vscode://file/./nodes/d3ziqry02i.md" _parent
    click jn53bcmsnv "vscode://file/./nodes/jn53bcmsnv.md" _parent
    click w0jz1dtx27 "vscode://file/./nodes/w0jz1dtx27.md" _parent
    click 6oeo7c9bch "vscode://file/./nodes/6oeo7c9bch.md" _parent
    click 6oeo7c9bch "vscode://file/./nodes/6oeo7c9bch.md" _parent
    click 7eaxdz9nwk "vscode://file/./nodes/7eaxdz9nwk.md" _parent
    click h330sqhk7o "vscode://file/./nodes/h330sqhk7o.md" _parent
    click d3ziqry02i "vscode://file/./nodes/d3ziqry02i.md" _parent
    click mjqbph9elz "vscode://file/./nodes/mjqbph9elz.md" _parent
    click ut2v2s6fqq "vscode://file/./nodes/ut2v2s6fqq.md" _parent
    click 75iq81515r "vscode://file/./nodes/75iq81515r.md" _parent
    click o5jvuf0bwl "vscode://file/./nodes/o5jvuf0bwl.md" _parent
    click 79lag5unyk "vscode://file/./nodes/79lag5unyk.md" _parent
    click a3oth8yspq "vscode://file/./nodes/a3oth8yspq.md" _parent
    click a3oth8yspq "vscode://file/./nodes/a3oth8yspq.md" _parent
    click 5vfn623mx7 "vscode://file/./nodes/5vfn623mx7.md" _parent
    click ateb0l10nl "vscode://file/./nodes/ateb0l10nl.md" _parent
    click h330sqhk7o "vscode://file/./nodes/h330sqhk7o.md" _parent
    click jn53bcmsnv "vscode://file/./nodes/jn53bcmsnv.md" _parent
    click mjqbph9elz "vscode://file/./nodes/mjqbph9elz.md" _parent
    click o5jvuf0bwl "vscode://file/./nodes/o5jvuf0bwl.md" _parent
    click dcq4ib3mce "vscode://file/./nodes/dcq4ib3mce.md" _parent
    click 6oeo7c9bch "vscode://file/./nodes/6oeo7c9bch.md" _parent
    click 2m4whqb1dr "vscode://file/./nodes/2m4whqb1dr.md" _parent
    click wv79oxt1fo "vscode://file/./nodes/wv79oxt1fo.md" _parent
    click 9pswmi4mi1 "vscode://file/./nodes/9pswmi4mi1.md" _parent
    click brpmsv8uag "vscode://file/./nodes/brpmsv8uag.md" _parent
    click b900rty9pd "vscode://file/./nodes/b900rty9pd.md" _parent
    click 30owhg6lfp "vscode://file/./nodes/30owhg6lfp.md" _parent
    click 75iq81515r "vscode://file/./nodes/75iq81515r.md" _parent
    click 2inl0soj3i "vscode://file/./nodes/2inl0soj3i.md" _parent
    click w0jz1dtx27 "vscode://file/./nodes/w0jz1dtx27.md" _parent
    click 7eaxdz9nwk "vscode://file/./nodes/7eaxdz9nwk.md" _parent
    click ateb0l10nl "vscode://file/./nodes/ateb0l10nl.md" _parent
    click 8qr5bc3clq "vscode://file/./nodes/8qr5bc3clq.md" _parent
    click jf9akdpa1q "vscode://file/./nodes/jf9akdpa1q.md" _parent
    click 5vfn623mx7 "vscode://file/./nodes/5vfn623mx7.md" _parent
    click 30owhg6lfp "vscode://file/./nodes/30owhg6lfp.md" _parent
    click 75iq81515r "vscode://file/./nodes/75iq81515r.md" _parent
    click 2inl0soj3i "vscode://file/./nodes/2inl0soj3i.md" _parent
    click 4tnam70cjm "vscode://file/./nodes/4tnam70cjm.md" _parent
    click 2znw6pakac "vscode://file/./nodes/2znw6pakac.md" _parent
    click 75iq81515r "vscode://file/./nodes/75iq81515r.md" _parent
    click wv79oxt1fo "vscode://file/./nodes/wv79oxt1fo.md" _parent
    click b900rty9pd "vscode://file/./nodes/b900rty9pd.md" _parent
    click hxmqf7sb52 "vscode://file/./nodes/hxmqf7sb52.md" _parent
    click xo4l1ngx8q "vscode://file/./nodes/xo4l1ngx8q.md" _parent
    click ixq0pq1td7 "vscode://file/./nodes/ixq0pq1td7.md" _parent
    click jf9akdpa1q "vscode://file/./nodes/jf9akdpa1q.md" _parent
    click 4tnam70cjm "vscode://file/./nodes/4tnam70cjm.md" _parent
    click 2znw6pakac "vscode://file/./nodes/2znw6pakac.md" _parent
    click uj42vvvgjt "vscode://file/./nodes/uj42vvvgjt.md" _parent
    click ym31re8b7g "vscode://file/./nodes/ym31re8b7g.md" _parent
    click okw0g6i84d "vscode://file/./nodes/okw0g6i84d.md" _parent
    click um3lcpaulo "vscode://file/./nodes/um3lcpaulo.md" _parent
    click abmzqz1u6f "vscode://file/./nodes/abmzqz1u6f.md" _parent
    click okw0g6i84d "vscode://file/./nodes/okw0g6i84d.md" _parent
    click um3lcpaulo "vscode://file/./nodes/um3lcpaulo.md" _parent
    click rysh2x3iz2 "vscode://file/./nodes/rysh2x3iz2.md" _parent
    click ym31re8b7g "vscode://file/./nodes/ym31re8b7g.md" _parent
    click ateb0l10nl "vscode://file/./nodes/ateb0l10nl.md" _parent
    click rysh2x3iz2 "vscode://file/./nodes/rysh2x3iz2.md" _parent
    click 6oeo7c9bch "vscode://file/./nodes/6oeo7c9bch.md" _parent
    click t0vllny9q "vscode://file/./nodes/t0vllny9q.md" _parent
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
 


## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| ciam_errorMessage##SK##flowInstance |  | flowInstance |  | string | 0 | 2000 | true | property | 
 

### Custom CSS
~> Note: Custom CSS is applied to every node in the flow

```css

```
