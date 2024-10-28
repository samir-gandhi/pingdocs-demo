# CIAM-Passwordless-Protect-Change-Password-Subflow
Description: Imported on Thu Oct 24 2024 20:38:13 GMT&#43;0000 (Coordinated Universal Time) 


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


### Flow Diagram
```mermaid
flowchart LR
    v738ey1b5y((EVAL)) --> xo4l1ngx8q[NOP UI Page]
    md8472gv2e[Show Success] --> v738ey1b5y((EVAL))
    ixq0pq1td7((EVAL)) --> 5vfn623mx7[Display password reset form]
    mjqbph9elz((Evaluator)) --> ur66q695u0[Node]
    d3ziqry02i((EVAL)) --> yo6nv4gud2[Node]
    d3ziqry02i((EVAL)) --> jn53bcmsnv[Boolean Check]
    w0jz1dtx27[Verify Passwords Match] --> 6oeo7c9bch((Evaluator))
    6oeo7c9bch((Evaluator)) --> 7eaxdz9nwk[Update password]
    h330sqhk7o[Empty Check] --> d3ziqry02i((EVAL))
    mjqbph9elz((Evaluator)) --> ut2v2s6fqq[Node]
    75iq81515r[Password reset submit?] --> o5jvuf0bwl((EVAL))
    79lag5unyk[NOP UI Page] --> a3oth8yspq((EVAL))
    a3oth8yspq((EVAL)) --> 5vfn623mx7[Display password reset form]
    ateb0l10nl((Evaluator)) --> h330sqhk7o[Empty Check]
    jn53bcmsnv[Boolean Check] --> mjqbph9elz((Evaluator))
    o5jvuf0bwl((EVAL)) --> dcq4ib3mce[Node]
    6oeo7c9bch((Evaluator)) --> 2m4whqb1dr[Passwords don&#39;t match]
    wv79oxt1fo((EVAL)) --> 9pswmi4mi1[Node]
    brpmsv8uag[Success Error] --> b900rty9pd((EVAL))
    30owhg6lfp((EVAL)) --> 75iq81515r[Password reset submit?]
    2inl0soj3i((EVAL)) --> w0jz1dtx27[Verify Passwords Match]
    7eaxdz9nwk[Update password] --> ateb0l10nl((Evaluator))
    8qr5bc3clq[Success] --> jf9akdpa1q((EVAL))
    5vfn623mx7[Display password reset form] --> 30owhg6lfp((EVAL))
    75iq81515r[Password reset submit?] --> 2inl0soj3i((EVAL))
    4tnam70cjm[Send Success Response] --> 2znw6pakac((Evaluator))
    75iq81515r[Password reset submit?] --> wv79oxt1fo((EVAL))
    b900rty9pd((EVAL)) --> hxmqf7sb52[Send Error Response]
    xo4l1ngx8q[NOP UI Page] --> ixq0pq1td7((EVAL))
    jf9akdpa1q((EVAL)) --> 4tnam70cjm[Send Success Response]
    2znw6pakac((Evaluator)) --> uj42vvvgjt[Node]
    ym31re8b7g((EVAL)) --> okw0g6i84d[Update error message]
    um3lcpaulo((EVAL)) --> abmzqz1u6f[Invalid password]
    okw0g6i84d[Update error message] --> um3lcpaulo((EVAL))
    rysh2x3iz2[Set error message] --> ym31re8b7g((EVAL))
    ateb0l10nl((Evaluator)) --> rysh2x3iz2[Set error message]

    click v738ey1b5y "v738ey1b5y" "v738ey1b5y"
    click xo4l1ngx8q "xo4l1ngx8q" "xo4l1ngx8q"
    click md8472gv2e "md8472gv2e" "md8472gv2e"
    click v738ey1b5y "v738ey1b5y" "v738ey1b5y"
    click ixq0pq1td7 "ixq0pq1td7" "ixq0pq1td7"
    click 5vfn623mx7 "5vfn623mx7" "5vfn623mx7"
    click mjqbph9elz "mjqbph9elz" "mjqbph9elz"
    click ur66q695u0 "ur66q695u0" "ur66q695u0"
    click d3ziqry02i "d3ziqry02i" "d3ziqry02i"
    click yo6nv4gud2 "yo6nv4gud2" "yo6nv4gud2"
    click d3ziqry02i "d3ziqry02i" "d3ziqry02i"
    click jn53bcmsnv "jn53bcmsnv" "jn53bcmsnv"
    click w0jz1dtx27 "w0jz1dtx27" "w0jz1dtx27"
    click 6oeo7c9bch "6oeo7c9bch" "6oeo7c9bch"
    click 6oeo7c9bch "6oeo7c9bch" "6oeo7c9bch"
    click 7eaxdz9nwk "7eaxdz9nwk" "7eaxdz9nwk"
    click h330sqhk7o "h330sqhk7o" "h330sqhk7o"
    click d3ziqry02i "d3ziqry02i" "d3ziqry02i"
    click mjqbph9elz "mjqbph9elz" "mjqbph9elz"
    click ut2v2s6fqq "ut2v2s6fqq" "ut2v2s6fqq"
    click 75iq81515r "75iq81515r" "75iq81515r"
    click o5jvuf0bwl "o5jvuf0bwl" "o5jvuf0bwl"
    click 79lag5unyk "79lag5unyk" "79lag5unyk"
    click a3oth8yspq "a3oth8yspq" "a3oth8yspq"
    click a3oth8yspq "a3oth8yspq" "a3oth8yspq"
    click 5vfn623mx7 "5vfn623mx7" "5vfn623mx7"
    click ateb0l10nl "ateb0l10nl" "ateb0l10nl"
    click h330sqhk7o "h330sqhk7o" "h330sqhk7o"
    click jn53bcmsnv "jn53bcmsnv" "jn53bcmsnv"
    click mjqbph9elz "mjqbph9elz" "mjqbph9elz"
    click o5jvuf0bwl "o5jvuf0bwl" "o5jvuf0bwl"
    click dcq4ib3mce "dcq4ib3mce" "dcq4ib3mce"
    click 6oeo7c9bch "6oeo7c9bch" "6oeo7c9bch"
    click 2m4whqb1dr "2m4whqb1dr" "2m4whqb1dr"
    click wv79oxt1fo "wv79oxt1fo" "wv79oxt1fo"
    click 9pswmi4mi1 "9pswmi4mi1" "9pswmi4mi1"
    click brpmsv8uag "brpmsv8uag" "brpmsv8uag"
    click b900rty9pd "b900rty9pd" "b900rty9pd"
    click 30owhg6lfp "30owhg6lfp" "30owhg6lfp"
    click 75iq81515r "75iq81515r" "75iq81515r"
    click 2inl0soj3i "2inl0soj3i" "2inl0soj3i"
    click w0jz1dtx27 "w0jz1dtx27" "w0jz1dtx27"
    click 7eaxdz9nwk "7eaxdz9nwk" "7eaxdz9nwk"
    click ateb0l10nl "ateb0l10nl" "ateb0l10nl"
    click 8qr5bc3clq "8qr5bc3clq" "8qr5bc3clq"
    click jf9akdpa1q "jf9akdpa1q" "jf9akdpa1q"
    click 5vfn623mx7 "5vfn623mx7" "5vfn623mx7"
    click 30owhg6lfp "30owhg6lfp" "30owhg6lfp"
    click 75iq81515r "75iq81515r" "75iq81515r"
    click 2inl0soj3i "2inl0soj3i" "2inl0soj3i"
    click 4tnam70cjm "4tnam70cjm" "4tnam70cjm"
    click 2znw6pakac "2znw6pakac" "2znw6pakac"
    click 75iq81515r "75iq81515r" "75iq81515r"
    click wv79oxt1fo "wv79oxt1fo" "wv79oxt1fo"
    click b900rty9pd "b900rty9pd" "b900rty9pd"
    click hxmqf7sb52 "hxmqf7sb52" "hxmqf7sb52"
    click xo4l1ngx8q "xo4l1ngx8q" "xo4l1ngx8q"
    click ixq0pq1td7 "ixq0pq1td7" "ixq0pq1td7"
    click jf9akdpa1q "jf9akdpa1q" "jf9akdpa1q"
    click 4tnam70cjm "4tnam70cjm" "4tnam70cjm"
    click 2znw6pakac "2znw6pakac" "2znw6pakac"
    click uj42vvvgjt "uj42vvvgjt" "uj42vvvgjt"
    click ym31re8b7g "ym31re8b7g" "ym31re8b7g"
    click okw0g6i84d "okw0g6i84d" "okw0g6i84d"
    click um3lcpaulo "um3lcpaulo" "um3lcpaulo"
    click abmzqz1u6f "abmzqz1u6f" "abmzqz1u6f"
    click okw0g6i84d "okw0g6i84d" "okw0g6i84d"
    click um3lcpaulo "um3lcpaulo" "um3lcpaulo"
    click rysh2x3iz2 "rysh2x3iz2" "rysh2x3iz2"
    click ym31re8b7g "ym31re8b7g" "ym31re8b7g"
    click ateb0l10nl "ateb0l10nl" "ateb0l10nl"
    click rysh2x3iz2 "rysh2x3iz2" "rysh2x3iz2"
```
