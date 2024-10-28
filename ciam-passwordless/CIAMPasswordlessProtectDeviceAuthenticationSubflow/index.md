# CIAM-Passwordless-Protect-Device-Authentication-Subflow
Description: Imported on Thu Oct 24 2024 20:38:13 GMT&#43;0000 (Coordinated Universal Time) 


## Settings
An exhaustive list of settings including defaults.
| Setting                          | Value                                                                                                                                                                                   |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSP Value                        | worker-src &#39;self&#39; blob:; script-src &#39;self&#39; https://cdn.jsdelivr.net https://code.jquery.com https://devsdk.singularkey.com http://cdnjs.cloudflare.com &#39;unsafe-inline&#39; &#39;unsafe-eval&#39;; | 
 | CSS Links                        | https://assets.pingone.com/ux/end-user-nano/0.1.0-alpha.1/end-user-nano.css,https://assets.pingone.com/ux/astro-nano/0.1.0-alpha.7/icons.css|

## Input Schemas
| Property Name | Description | Expanded | Preferred Control Type | Preferred Data Type | Required |
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| pingOneUserId | PingOne User ID | true | textField | string | true | 
 | email | PingOne User Email(Username) | true | textField | string | true | 
 | ciam_magicLinkEnabled |  | true | textField | boolean | false | 
 | allowedDeviceTypes |  | true | textField | string | false | 
 | ciam_companyLogo |  | true | textField | string | false | 
 


## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| ciam_protectriskPolicyId##SK##flowInstance |  | flowInstance | This PingOne Protect Risk Policy ID will be passed by default. | string | 0 | 2000 | true | property | 
 | ciam_protectRiskLevel##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne protect flows | string | 0 | 2000 | true | property | 
 | ciam_protectRiskID##SK##flowInstance |  | flowInstance | This variable is used by CIAM Passwordless with pingone protect flows. | string | 0 | 2000 | true | property | 
 | ciam_protectPredictor##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne Protect flows. | string | 0 | 2000 | true | property | 
 | ciam_protectDeviceStatus##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne protect flow | string | 0 | 2000 | true | property | 
 

### Custom CSS
~> Note: Custom CSS is applied to every node in the flow

```css

```


### Flow Diagram
```mermaid
flowchart LR
    mtaqacdw1m((Evaluator)) --> 8jrbqcts2g[Create MFA Device]
    hk00gx2f95((EVAL)) --> onogvjusk6[Prompt For OTP]
    qw4n733f3t((EVAL)) --> li0d8slgjx[Send email for new device]
    7jufzmg1rk[Activate MFA Device] --> qw4n733f3t((EVAL))
    8jrbqcts2g[Create MFA Device] --> hk00gx2f95((EVAL))
    kho2rpwvb7((Evaluator)) --> 7jufzmg1rk[Activate MFA Device]
    onogvjusk6[Prompt For OTP] --> kho2rpwvb7((Evaluator))
    78i0a08xfl[Send email for threat detection] --> iz5nper189((EVAL))
    gsmghrxxoy[Check for KNOWN DEVICE] --> nl0cxyid0x((EVAL))
    99q38lg97t((EVAL)) --> sqdggkol0g[Node]
    iloobtovwh((EVAL)) --> dxowhkk5n5[Check if Risk Policy ID is empty]
    iz5nper189((EVAL)) --> 7hwtzuxjwc[Disable user]
    n69ynlsgag((EVAL)) --> nf4hv96sui[Check MFA devices size]
    cb4rka2li0((EVAL)) --> 78i0a08xfl[Send email for threat detection]
    x8ainlbr6x((EVAL)) --> ndm5er34sv[Risk Score from PingOne Protect]
    j6salon8z4[Get Values from PingOne Protect analysis] --> cb4rka2li0((EVAL))
    ahjplbui3q[PingOne Notifications] --> x8ainlbr6x((EVAL))
    pt24r4nafa((EVAL)) --> 3y03qc0kxe[Find user details]
    mtaqacdw1m((Evaluator)) --> 5231692i67[Return to calling node.]
    4oyc5l9npk((EVAL)) --> 737gi6ip3e[Node]
    u22hch23vs((EVAL)) --> gsmghrxxoy[Check for KNOWN DEVICE]
    zfpuewwuhl[PingOne Protect Analysis] --> pt24r4nafa((EVAL))
    3y03qc0kxe[Find user details] --> qxdd8mlll5((EVAL))
    nl0cxyid0x((EVAL)) --> ahjplbui3q[PingOne Notifications]
    li0d8slgjx[Send email for new device] --> e3httj56zd((EVAL))
    737gi6ip3e[Node] --> 9vk797lpxx((EVAL))
    nf4hv96sui[Check MFA devices size] --> mtaqacdw1m((Evaluator))
    1cbcpbc5no((EVAL)) --> 4psx471uwp[Authentication Required]
    h8dtvwld36((EVAL)) --> 76reddil11[Node]
    r0hto2xun7[Present OTP Form] --> l5z3ngnhjv((EVAL))
    1gtc5d0awz((EVAL)) --> kok73n8hkt[to otp]
    4psx471uwp[Authentication Required] --> 1gtc5d0awz((EVAL))
    qurffyxc2d[Split by user selection ] --> gsw5wwtm7t((EVAL))
    en7y953x31[Get authMethod Value] --> 0w6twuixxq((EVAL))
    fzjj3nuh7m((EVAL)) --> dxsjn36392[Node]
    mt9kvt7hnn((EVAL)) --> fgc8woctfo[Validate Passcode]
    qurffyxc2d[Split by user selection ] --> 00j11fkhbx((EVAL))
    fzjj3nuh7m((EVAL)) --> uz6hhdt9gv[OTP Resent Message]
    zxfluj3oxa[OTP] --> b0csz8cgnl((EVAL))
    qurffyxc2d[Split by user selection ] --> ig2ndq8bf2((EVAL))
    00j11fkhbx((EVAL)) --> beakf43h8t[Node]
    gsw5wwtm7t((EVAL)) --> r6lnkuy0yh[Transform Passcode To Lowercase]
    ig2ndq8bf2((EVAL)) --> m1e0cw0ygl[Resend OTP]
    m1e0cw0ygl[Resend OTP] --> fzjj3nuh7m((EVAL))
    r6lnkuy0yh[Transform Passcode To Lowercase] --> mt9kvt7hnn((EVAL))
    hdc8oa72ci[Is invalidOTP Error] --> 8h5tjkrug9((EVAL))
    v97rmwpban((EVAL)) --> 5pixttpidw[Invalid Passcode Error]
    gntsn38l9s[CIAM - Magic Link Authentication] --> 51zazld6jz((EVAL))
    5uyrxkfgza((EVAL)) --> tidk1pmqix[Return Success Response]
    8h5tjkrug9((EVAL)) --> mmojm56jlj[Node]
    uoyh9kzwil[Device Selection] --> bhgtvbjvu1((EVAL))
    se271xaurx((EVAL)) --> uwfrx6s60u[Node]
    vr1msssq3l((EVAL)) --> wpbqyomp7z[Node]
    wa07p8s7qm[Not Magic Link?] --> vr1msssq3l((EVAL))
    vul5k2q2dw((EVAL)) --> te0bcdks99[Magic Link Authentication]
    wa07p8s7qm[Not Magic Link?] --> vul5k2q2dw((EVAL))
    imhudhsy1w((EVAL)) --> e717up82dy[Device Selected By The User]
    wa07p8s7qm[Not Magic Link?] --> imhudhsy1w((EVAL))
    j8lmuiytzs[Is MFA Enabled?] --> bf9jlbogz1((EVAL))
    bhgtvbjvu1((EVAL)) --> 1qtib8s0uu[Select Authentication Device]
    0sua91hqk7((EVAL)) --> 10oaokas61[Start MFA Authentication]
    845xzgf4bk((EVAL)) --> ulsqznx6ut[Is Constraint Violation Error]
    51zazld6jz((EVAL)) --> 5gs9h0ar04[Node]
    3a77bpgwom((EVAL)) --> y7f8x8dkw2[Node]
    zfsjjfa5h6[Present FIDO2 Form ] --> 9pb86bg0qi((EVAL))
    wf0h6fo6h8[Split By User&#39;s Selection] --> ay2mm4z4xe((EVAL))
    ulsqznx6ut[Is Constraint Violation Error] --> fu06ckn12l((EVAL))
    fj8w62y4z3[Assert FIDO Device Authentication] --> 845xzgf4bk((EVAL))
    fu06ckn12l((EVAL)) --> y8pxpynfle[Invalid Device Error]
    7vrrd3uuhm((EVAL)) --> en7y953x31[Get authMethod Value]
    1lam7h7jbc[Split By Subflow&#39;s Result] --> 9fzm9oj8fd((EVAL))
    qsu3efxcsp((EVAL)) --> 1lam7h7jbc[Split By Subflow&#39;s Result]
    6yu5p2iz3r((EVAL)) --> ms19ql02hi[Get MFA Status]
    en7y953x31[Get authMethod Value] --> 0w6twuixxq((EVAL))
    t6p5s6t603[Get WebAuthn Browser Compatibility] --> 4oyc5l9npk((EVAL))
    10uwd1ccc4[Filter Unusable Devices] --> se271xaurx((EVAL))
    wzzac3ucto[Create Masked Devices] --> 6yu5p2iz3r((EVAL))
    fd7o3icva4((EVAL)) --> j8lmuiytzs[Is MFA Enabled?]
    ms19ql02hi[Get MFA Status] --> fd7o3icva4((EVAL))
    3nn0mw8jkt((EVAL)) --> 61c9e2dt59[Node]
    51zazld6jz((EVAL)) --> nvxwg0vum3[Node]
    9fzm9oj8fd((EVAL)) --> lgn9kliiqj[Node]
    b0csz8cgnl((EVAL)) --> fq7l0s8w2s[Mask Device]
    1lam7h7jbc[Split By Subflow&#39;s Result] --> lylme68jbw((EVAL))
    0w6twuixxq((EVAL)) --> 5sb0db3vb0[Node]
    7vpjww2ek2[FIDO2] --> t04dles3gs((EVAL))
    9vk797lpxx((EVAL)) --> 10uwd1ccc4[Filter Unusable Devices]
    wf0h6fo6h8[Split By User&#39;s Selection] --> 3nn0mw8jkt((EVAL))
    k46n95w9eo[Success ] --> 5uyrxkfgza((EVAL))
    hdc8oa72ci[Is invalidOTP Error] --> v97rmwpban((EVAL))
    7vrrd3uuhm((EVAL)) --> hdc8oa72ci[Is invalidOTP Error]
    fgc8woctfo[Validate Passcode] --> 7vrrd3uuhm((EVAL))
    zbhvblc83s[Authentication Method Selection] --> ybwxgols9w((EVAL))
    4psx471uwp[Authentication Required] --> h8dtvwld36((EVAL))
    ybwxgols9w((EVAL)) --> 9zctbmveoc[Enrich Device Details]
    iloobtovwh((EVAL)) --> dwhgyxkavz[Error Error Response]
    qsu3efxcsp((EVAL)) --> muund54c7j[Node]
    6p4frzqpp1[Get Origin] --> sk7vd2o3r7((EVAL))
    845xzgf4bk((EVAL)) --> dp43hy7h76[Get authMethod Value]
    5v1i2f1az4((EVAL)) --> cbapcifpyy[Node]
    nydopq0ve3((EVAL)) --> qzuk2c4cdb[Node]
    nydopq0ve3((EVAL)) --> t6p5s6t603[Get WebAuthn Browser Compatibility]
    fq7l0s8w2s[Mask Device] --> bdjeulfdki((EVAL))
    jd87iaho99[Error] --> iloobtovwh((EVAL))
    7vz1yqkdqo((Evaluator)) --> gntsn38l9s[CIAM - Magic Link Authentication]
    bdjeulfdki((EVAL)) --> r0hto2xun7[Present OTP Form]
    9m5a2f4emp[Get User&#39;s Existing Devices] --> nydopq0ve3((EVAL))
    dp43hy7h76[Get authMethod Value] --> zep1ojf98g((EVAL))
    czzrbt1dsb[Magic Link Enabled] --> 7vz1yqkdqo((Evaluator))
    ulsqznx6ut[Is Constraint Violation Error] --> 3a77bpgwom((EVAL))
    ay2mm4z4xe((EVAL)) --> fj8w62y4z3[Assert FIDO Device Authentication]
    0sua91hqk7((EVAL)) --> czzrbt1dsb[Magic Link Enabled]
    sk7vd2o3r7((EVAL)) --> 9m5a2f4emp[Get User&#39;s Existing Devices]
    lylme68jbw((EVAL)) --> fkkub10ukt[Node]
    zep1ojf98g((EVAL)) --> 9f0dokmcu9[Node]
    10oaokas61[Start MFA Authentication] --> 4l39ap532m((Evaluator))
    47qta86y95((EVAL)) --> x0jx5r2pyd[Node]
    frh74jp1jg[Only One Usable Device] --> ydyrhm9fkz((EVAL))
    47qta86y95((EVAL)) --> wphj1fy8ri[Node]
    b01n00fwkm[Continue MFA With Only Device] --> 47qta86y95((EVAL))
    7vz1yqkdqo((Evaluator)) --> 2uhj1oobbe[Node]
    4l39ap532m((Evaluator)) --> icy7kw57ll[Authentication Prompt]
    icy7kw57ll[Authentication Prompt] --> v0t14r4lv2((EVAL))
    v0t14r4lv2((EVAL)) --> frh74jp1jg[Only One Usable Device]
    4l39ap532m((Evaluator)) --> t4cuk82upd[Node]
    icy7kw57ll[Authentication Prompt] --> wj5284rjb8((EVAL))
    wj5284rjb8((EVAL)) --> l7i5qjffz1[Node]
    icy7kw57ll[Authentication Prompt] --> vw8zbuzgod((EVAL))
    vw8zbuzgod((EVAL)) --> j55n69o5i7[Node]
    ydyrhm9fkz((EVAL)) --> a58tdqlgfb[Node]
    t04dles3gs((EVAL)) --> zfsjjfa5h6[Present FIDO2 Form ]
    5v1i2f1az4((EVAL)) --> 4vf8sqyl70[Node]
    9pb86bg0qi((EVAL)) --> wf0h6fo6h8[Split By User&#39;s Selection]
    1qtib8s0uu[Select Authentication Device] --> iagfrg0an6((EVAL))
    e717up82dy[Device Selected By The User] --> 5v1i2f1az4((EVAL))
    bf9jlbogz1((EVAL)) --> 2n3az4vori[User Has Active Devices]
    iagfrg0an6((EVAL)) --> wa07p8s7qm[Not Magic Link?]
    bf9jlbogz1((EVAL)) --> czzrbt1dsb[Magic Link Enabled]
    2n3az4vori[User Has Active Devices] --> 0sua91hqk7((EVAL))
    te0bcdks99[Magic Link Authentication] --> qsu3efxcsp((EVAL))
    ydyrhm9fkz((EVAL)) --> xsm25p5qf7[Magic Link Enabled]
    xsm25p5qf7[Magic Link Enabled] --> ayodtok1lb((EVAL))
    ayodtok1lb((EVAL)) --> x9k0uusly8[Node]
    ayodtok1lb((EVAL)) --> b01n00fwkm[Continue MFA With Only Device]
    9zctbmveoc[Enrich Device Details] --> 1cbcpbc5no((EVAL))
    l5z3ngnhjv((EVAL)) --> qurffyxc2d[Split by user selection ]
    se271xaurx((EVAL)) --> wzzac3ucto[Create Masked Devices]
    sk3dza5671((EVAL)) --> di86a7q7j0[Node]
    e3httj56zd((EVAL)) --> 5231692i67[Return to calling node.]
    qxdd8mlll5((EVAL)) --> u9ab712lfx[Invoke PingOne Protect subflow]
    u9ab712lfx[Invoke PingOne Protect subflow] --> vexxoicu6a((Evaluator))
    vexxoicu6a((Evaluator)) --> 3s5kidc2wc[Get Values from PingOne Protect analysis]
    vexxoicu6a((Evaluator)) --> j6salon8z4[Get Values from PingOne Protect analysis]
    3s5kidc2wc[Get Values from PingOne Protect analysis] --> u22hch23vs((EVAL))
    nl0cxyid0x((EVAL)) --> ndm5er34sv[Risk Score from PingOne Protect]
    ndm5er34sv[Risk Score from PingOne Protect] --> 4n12f0orqv((EVAL))
    4n12f0orqv((EVAL)) --> d2uumx5mpk[Return to calling node]
    ndm5er34sv[Risk Score from PingOne Protect] --> n69ynlsgag((EVAL))
    7hwtzuxjwc[Disable user] --> 99q38lg97t((EVAL))
    ndm5er34sv[Risk Score from PingOne Protect] --> sk3dza5671((EVAL))
    kgxiu8h9i5((EVAL)) --> 9w2fwmdjtp[PingOne Protect Risk ID is Empty/NULL]
    qw4n733f3t((EVAL)) --> sj6aezm25b[Node]
    dxowhkk5n5[Check if Risk Policy ID is empty] --> kgxiu8h9i5((EVAL))
    kgxiu8h9i5((EVAL)) --> p3914imkz7[Update Risk Evaluation - FAILURE]
    5uyrxkfgza((EVAL)) --> wi6hu0ai62[Check if Risk Policy ID is empty]
    wi6hu0ai62[Check if Risk Policy ID is empty] --> 33jpsgsdxv((EVAL))
    33jpsgsdxv((EVAL)) --> ilu6o9n2x7[Update Risk Evaluation - SUCCESS]
    33jpsgsdxv((EVAL)) --> 33kryo3flh[PingOne Protect Risk ID is Empty/NULL]
    fd7o3icva4((EVAL)) --> 9q9zj5ndao[Node]

    click mtaqacdw1m "mtaqacdw1m" "mtaqacdw1m"
    click 8jrbqcts2g "8jrbqcts2g" "8jrbqcts2g"
    click hk00gx2f95 "hk00gx2f95" "hk00gx2f95"
    click onogvjusk6 "onogvjusk6" "onogvjusk6"
    click qw4n733f3t "qw4n733f3t" "qw4n733f3t"
    click li0d8slgjx "li0d8slgjx" "li0d8slgjx"
    click 7jufzmg1rk "7jufzmg1rk" "7jufzmg1rk"
    click qw4n733f3t "qw4n733f3t" "qw4n733f3t"
    click 8jrbqcts2g "8jrbqcts2g" "8jrbqcts2g"
    click hk00gx2f95 "hk00gx2f95" "hk00gx2f95"
    click kho2rpwvb7 "kho2rpwvb7" "kho2rpwvb7"
    click 7jufzmg1rk "7jufzmg1rk" "7jufzmg1rk"
    click onogvjusk6 "onogvjusk6" "onogvjusk6"
    click kho2rpwvb7 "kho2rpwvb7" "kho2rpwvb7"
    click 78i0a08xfl "78i0a08xfl" "78i0a08xfl"
    click iz5nper189 "iz5nper189" "iz5nper189"
    click gsmghrxxoy "gsmghrxxoy" "gsmghrxxoy"
    click nl0cxyid0x "nl0cxyid0x" "nl0cxyid0x"
    click 99q38lg97t "99q38lg97t" "99q38lg97t"
    click sqdggkol0g "sqdggkol0g" "sqdggkol0g"
    click iloobtovwh "iloobtovwh" "iloobtovwh"
    click dxowhkk5n5 "dxowhkk5n5" "dxowhkk5n5"
    click iz5nper189 "iz5nper189" "iz5nper189"
    click 7hwtzuxjwc "7hwtzuxjwc" "7hwtzuxjwc"
    click n69ynlsgag "n69ynlsgag" "n69ynlsgag"
    click nf4hv96sui "nf4hv96sui" "nf4hv96sui"
    click cb4rka2li0 "cb4rka2li0" "cb4rka2li0"
    click 78i0a08xfl "78i0a08xfl" "78i0a08xfl"
    click x8ainlbr6x "x8ainlbr6x" "x8ainlbr6x"
    click ndm5er34sv "ndm5er34sv" "ndm5er34sv"
    click j6salon8z4 "j6salon8z4" "j6salon8z4"
    click cb4rka2li0 "cb4rka2li0" "cb4rka2li0"
    click ahjplbui3q "ahjplbui3q" "ahjplbui3q"
    click x8ainlbr6x "x8ainlbr6x" "x8ainlbr6x"
    click pt24r4nafa "pt24r4nafa" "pt24r4nafa"
    click 3y03qc0kxe "3y03qc0kxe" "3y03qc0kxe"
    click mtaqacdw1m "mtaqacdw1m" "mtaqacdw1m"
    click 5231692i67 "5231692i67" "5231692i67"
    click 4oyc5l9npk "4oyc5l9npk" "4oyc5l9npk"
    click 737gi6ip3e "737gi6ip3e" "737gi6ip3e"
    click u22hch23vs "u22hch23vs" "u22hch23vs"
    click gsmghrxxoy "gsmghrxxoy" "gsmghrxxoy"
    click zfpuewwuhl "zfpuewwuhl" "zfpuewwuhl"
    click pt24r4nafa "pt24r4nafa" "pt24r4nafa"
    click 3y03qc0kxe "3y03qc0kxe" "3y03qc0kxe"
    click qxdd8mlll5 "qxdd8mlll5" "qxdd8mlll5"
    click nl0cxyid0x "nl0cxyid0x" "nl0cxyid0x"
    click ahjplbui3q "ahjplbui3q" "ahjplbui3q"
    click li0d8slgjx "li0d8slgjx" "li0d8slgjx"
    click e3httj56zd "e3httj56zd" "e3httj56zd"
    click 737gi6ip3e "737gi6ip3e" "737gi6ip3e"
    click 9vk797lpxx "9vk797lpxx" "9vk797lpxx"
    click nf4hv96sui "nf4hv96sui" "nf4hv96sui"
    click mtaqacdw1m "mtaqacdw1m" "mtaqacdw1m"
    click 1cbcpbc5no "1cbcpbc5no" "1cbcpbc5no"
    click 4psx471uwp "4psx471uwp" "4psx471uwp"
    click h8dtvwld36 "h8dtvwld36" "h8dtvwld36"
    click 76reddil11 "76reddil11" "76reddil11"
    click r0hto2xun7 "r0hto2xun7" "r0hto2xun7"
    click l5z3ngnhjv "l5z3ngnhjv" "l5z3ngnhjv"
    click 1gtc5d0awz "1gtc5d0awz" "1gtc5d0awz"
    click kok73n8hkt "kok73n8hkt" "kok73n8hkt"
    click 4psx471uwp "4psx471uwp" "4psx471uwp"
    click 1gtc5d0awz "1gtc5d0awz" "1gtc5d0awz"
    click qurffyxc2d "qurffyxc2d" "qurffyxc2d"
    click gsw5wwtm7t "gsw5wwtm7t" "gsw5wwtm7t"
    click en7y953x31 "en7y953x31" "en7y953x31"
    click 0w6twuixxq "0w6twuixxq" "0w6twuixxq"
    click fzjj3nuh7m "fzjj3nuh7m" "fzjj3nuh7m"
    click dxsjn36392 "dxsjn36392" "dxsjn36392"
    click mt9kvt7hnn "mt9kvt7hnn" "mt9kvt7hnn"
    click fgc8woctfo "fgc8woctfo" "fgc8woctfo"
    click qurffyxc2d "qurffyxc2d" "qurffyxc2d"
    click 00j11fkhbx "00j11fkhbx" "00j11fkhbx"
    click fzjj3nuh7m "fzjj3nuh7m" "fzjj3nuh7m"
    click uz6hhdt9gv "uz6hhdt9gv" "uz6hhdt9gv"
    click zxfluj3oxa "zxfluj3oxa" "zxfluj3oxa"
    click b0csz8cgnl "b0csz8cgnl" "b0csz8cgnl"
    click qurffyxc2d "qurffyxc2d" "qurffyxc2d"
    click ig2ndq8bf2 "ig2ndq8bf2" "ig2ndq8bf2"
    click 00j11fkhbx "00j11fkhbx" "00j11fkhbx"
    click beakf43h8t "beakf43h8t" "beakf43h8t"
    click gsw5wwtm7t "gsw5wwtm7t" "gsw5wwtm7t"
    click r6lnkuy0yh "r6lnkuy0yh" "r6lnkuy0yh"
    click ig2ndq8bf2 "ig2ndq8bf2" "ig2ndq8bf2"
    click m1e0cw0ygl "m1e0cw0ygl" "m1e0cw0ygl"
    click m1e0cw0ygl "m1e0cw0ygl" "m1e0cw0ygl"
    click fzjj3nuh7m "fzjj3nuh7m" "fzjj3nuh7m"
    click r6lnkuy0yh "r6lnkuy0yh" "r6lnkuy0yh"
    click mt9kvt7hnn "mt9kvt7hnn" "mt9kvt7hnn"
    click hdc8oa72ci "hdc8oa72ci" "hdc8oa72ci"
    click 8h5tjkrug9 "8h5tjkrug9" "8h5tjkrug9"
    click v97rmwpban "v97rmwpban" "v97rmwpban"
    click 5pixttpidw "5pixttpidw" "5pixttpidw"
    click gntsn38l9s "gntsn38l9s" "gntsn38l9s"
    click 51zazld6jz "51zazld6jz" "51zazld6jz"
    click 5uyrxkfgza "5uyrxkfgza" "5uyrxkfgza"
    click tidk1pmqix "tidk1pmqix" "tidk1pmqix"
    click 8h5tjkrug9 "8h5tjkrug9" "8h5tjkrug9"
    click mmojm56jlj "mmojm56jlj" "mmojm56jlj"
    click uoyh9kzwil "uoyh9kzwil" "uoyh9kzwil"
    click bhgtvbjvu1 "bhgtvbjvu1" "bhgtvbjvu1"
    click se271xaurx "se271xaurx" "se271xaurx"
    click uwfrx6s60u "uwfrx6s60u" "uwfrx6s60u"
    click vr1msssq3l "vr1msssq3l" "vr1msssq3l"
    click wpbqyomp7z "wpbqyomp7z" "wpbqyomp7z"
    click wa07p8s7qm "wa07p8s7qm" "wa07p8s7qm"
    click vr1msssq3l "vr1msssq3l" "vr1msssq3l"
    click vul5k2q2dw "vul5k2q2dw" "vul5k2q2dw"
    click te0bcdks99 "te0bcdks99" "te0bcdks99"
    click wa07p8s7qm "wa07p8s7qm" "wa07p8s7qm"
    click vul5k2q2dw "vul5k2q2dw" "vul5k2q2dw"
    click imhudhsy1w "imhudhsy1w" "imhudhsy1w"
    click e717up82dy "e717up82dy" "e717up82dy"
    click wa07p8s7qm "wa07p8s7qm" "wa07p8s7qm"
    click imhudhsy1w "imhudhsy1w" "imhudhsy1w"
    click j8lmuiytzs "j8lmuiytzs" "j8lmuiytzs"
    click bf9jlbogz1 "bf9jlbogz1" "bf9jlbogz1"
    click bhgtvbjvu1 "bhgtvbjvu1" "bhgtvbjvu1"
    click 1qtib8s0uu "1qtib8s0uu" "1qtib8s0uu"
    click 0sua91hqk7 "0sua91hqk7" "0sua91hqk7"
    click 10oaokas61 "10oaokas61" "10oaokas61"
    click 845xzgf4bk "845xzgf4bk" "845xzgf4bk"
    click ulsqznx6ut "ulsqznx6ut" "ulsqznx6ut"
    click 51zazld6jz "51zazld6jz" "51zazld6jz"
    click 5gs9h0ar04 "5gs9h0ar04" "5gs9h0ar04"
    click 3a77bpgwom "3a77bpgwom" "3a77bpgwom"
    click y7f8x8dkw2 "y7f8x8dkw2" "y7f8x8dkw2"
    click zfsjjfa5h6 "zfsjjfa5h6" "zfsjjfa5h6"
    click 9pb86bg0qi "9pb86bg0qi" "9pb86bg0qi"
    click wf0h6fo6h8 "wf0h6fo6h8" "wf0h6fo6h8"
    click ay2mm4z4xe "ay2mm4z4xe" "ay2mm4z4xe"
    click ulsqznx6ut "ulsqznx6ut" "ulsqznx6ut"
    click fu06ckn12l "fu06ckn12l" "fu06ckn12l"
    click fj8w62y4z3 "fj8w62y4z3" "fj8w62y4z3"
    click 845xzgf4bk "845xzgf4bk" "845xzgf4bk"
    click fu06ckn12l "fu06ckn12l" "fu06ckn12l"
    click y8pxpynfle "y8pxpynfle" "y8pxpynfle"
    click 7vrrd3uuhm "7vrrd3uuhm" "7vrrd3uuhm"
    click en7y953x31 "en7y953x31" "en7y953x31"
    click 1lam7h7jbc "1lam7h7jbc" "1lam7h7jbc"
    click 9fzm9oj8fd "9fzm9oj8fd" "9fzm9oj8fd"
    click qsu3efxcsp "qsu3efxcsp" "qsu3efxcsp"
    click 1lam7h7jbc "1lam7h7jbc" "1lam7h7jbc"
    click 6yu5p2iz3r "6yu5p2iz3r" "6yu5p2iz3r"
    click ms19ql02hi "ms19ql02hi" "ms19ql02hi"
    click en7y953x31 "en7y953x31" "en7y953x31"
    click 0w6twuixxq "0w6twuixxq" "0w6twuixxq"
    click t6p5s6t603 "t6p5s6t603" "t6p5s6t603"
    click 4oyc5l9npk "4oyc5l9npk" "4oyc5l9npk"
    click 10uwd1ccc4 "10uwd1ccc4" "10uwd1ccc4"
    click se271xaurx "se271xaurx" "se271xaurx"
    click wzzac3ucto "wzzac3ucto" "wzzac3ucto"
    click 6yu5p2iz3r "6yu5p2iz3r" "6yu5p2iz3r"
    click fd7o3icva4 "fd7o3icva4" "fd7o3icva4"
    click j8lmuiytzs "j8lmuiytzs" "j8lmuiytzs"
    click ms19ql02hi "ms19ql02hi" "ms19ql02hi"
    click fd7o3icva4 "fd7o3icva4" "fd7o3icva4"
    click 3nn0mw8jkt "3nn0mw8jkt" "3nn0mw8jkt"
    click 61c9e2dt59 "61c9e2dt59" "61c9e2dt59"
    click 51zazld6jz "51zazld6jz" "51zazld6jz"
    click nvxwg0vum3 "nvxwg0vum3" "nvxwg0vum3"
    click 9fzm9oj8fd "9fzm9oj8fd" "9fzm9oj8fd"
    click lgn9kliiqj "lgn9kliiqj" "lgn9kliiqj"
    click b0csz8cgnl "b0csz8cgnl" "b0csz8cgnl"
    click fq7l0s8w2s "fq7l0s8w2s" "fq7l0s8w2s"
    click 1lam7h7jbc "1lam7h7jbc" "1lam7h7jbc"
    click lylme68jbw "lylme68jbw" "lylme68jbw"
    click 0w6twuixxq "0w6twuixxq" "0w6twuixxq"
    click 5sb0db3vb0 "5sb0db3vb0" "5sb0db3vb0"
    click 7vpjww2ek2 "7vpjww2ek2" "7vpjww2ek2"
    click t04dles3gs "t04dles3gs" "t04dles3gs"
    click 9vk797lpxx "9vk797lpxx" "9vk797lpxx"
    click 10uwd1ccc4 "10uwd1ccc4" "10uwd1ccc4"
    click wf0h6fo6h8 "wf0h6fo6h8" "wf0h6fo6h8"
    click 3nn0mw8jkt "3nn0mw8jkt" "3nn0mw8jkt"
    click k46n95w9eo "k46n95w9eo" "k46n95w9eo"
    click 5uyrxkfgza "5uyrxkfgza" "5uyrxkfgza"
    click hdc8oa72ci "hdc8oa72ci" "hdc8oa72ci"
    click v97rmwpban "v97rmwpban" "v97rmwpban"
    click 7vrrd3uuhm "7vrrd3uuhm" "7vrrd3uuhm"
    click hdc8oa72ci "hdc8oa72ci" "hdc8oa72ci"
    click fgc8woctfo "fgc8woctfo" "fgc8woctfo"
    click 7vrrd3uuhm "7vrrd3uuhm" "7vrrd3uuhm"
    click zbhvblc83s "zbhvblc83s" "zbhvblc83s"
    click ybwxgols9w "ybwxgols9w" "ybwxgols9w"
    click 4psx471uwp "4psx471uwp" "4psx471uwp"
    click h8dtvwld36 "h8dtvwld36" "h8dtvwld36"
    click ybwxgols9w "ybwxgols9w" "ybwxgols9w"
    click 9zctbmveoc "9zctbmveoc" "9zctbmveoc"
    click iloobtovwh "iloobtovwh" "iloobtovwh"
    click dwhgyxkavz "dwhgyxkavz" "dwhgyxkavz"
    click qsu3efxcsp "qsu3efxcsp" "qsu3efxcsp"
    click muund54c7j "muund54c7j" "muund54c7j"
    click 6p4frzqpp1 "6p4frzqpp1" "6p4frzqpp1"
    click sk7vd2o3r7 "sk7vd2o3r7" "sk7vd2o3r7"
    click 845xzgf4bk "845xzgf4bk" "845xzgf4bk"
    click dp43hy7h76 "dp43hy7h76" "dp43hy7h76"
    click 5v1i2f1az4 "5v1i2f1az4" "5v1i2f1az4"
    click cbapcifpyy "cbapcifpyy" "cbapcifpyy"
    click nydopq0ve3 "nydopq0ve3" "nydopq0ve3"
    click qzuk2c4cdb "qzuk2c4cdb" "qzuk2c4cdb"
    click nydopq0ve3 "nydopq0ve3" "nydopq0ve3"
    click t6p5s6t603 "t6p5s6t603" "t6p5s6t603"
    click fq7l0s8w2s "fq7l0s8w2s" "fq7l0s8w2s"
    click bdjeulfdki "bdjeulfdki" "bdjeulfdki"
    click jd87iaho99 "jd87iaho99" "jd87iaho99"
    click iloobtovwh "iloobtovwh" "iloobtovwh"
    click 7vz1yqkdqo "7vz1yqkdqo" "7vz1yqkdqo"
    click gntsn38l9s "gntsn38l9s" "gntsn38l9s"
    click bdjeulfdki "bdjeulfdki" "bdjeulfdki"
    click r0hto2xun7 "r0hto2xun7" "r0hto2xun7"
    click 9m5a2f4emp "9m5a2f4emp" "9m5a2f4emp"
    click nydopq0ve3 "nydopq0ve3" "nydopq0ve3"
    click dp43hy7h76 "dp43hy7h76" "dp43hy7h76"
    click zep1ojf98g "zep1ojf98g" "zep1ojf98g"
    click czzrbt1dsb "czzrbt1dsb" "czzrbt1dsb"
    click 7vz1yqkdqo "7vz1yqkdqo" "7vz1yqkdqo"
    click ulsqznx6ut "ulsqznx6ut" "ulsqznx6ut"
    click 3a77bpgwom "3a77bpgwom" "3a77bpgwom"
    click ay2mm4z4xe "ay2mm4z4xe" "ay2mm4z4xe"
    click fj8w62y4z3 "fj8w62y4z3" "fj8w62y4z3"
    click 0sua91hqk7 "0sua91hqk7" "0sua91hqk7"
    click czzrbt1dsb "czzrbt1dsb" "czzrbt1dsb"
    click sk7vd2o3r7 "sk7vd2o3r7" "sk7vd2o3r7"
    click 9m5a2f4emp "9m5a2f4emp" "9m5a2f4emp"
    click lylme68jbw "lylme68jbw" "lylme68jbw"
    click fkkub10ukt "fkkub10ukt" "fkkub10ukt"
    click zep1ojf98g "zep1ojf98g" "zep1ojf98g"
    click 9f0dokmcu9 "9f0dokmcu9" "9f0dokmcu9"
    click 10oaokas61 "10oaokas61" "10oaokas61"
    click 4l39ap532m "4l39ap532m" "4l39ap532m"
    click 47qta86y95 "47qta86y95" "47qta86y95"
    click x0jx5r2pyd "x0jx5r2pyd" "x0jx5r2pyd"
    click frh74jp1jg "frh74jp1jg" "frh74jp1jg"
    click ydyrhm9fkz "ydyrhm9fkz" "ydyrhm9fkz"
    click 47qta86y95 "47qta86y95" "47qta86y95"
    click wphj1fy8ri "wphj1fy8ri" "wphj1fy8ri"
    click b01n00fwkm "b01n00fwkm" "b01n00fwkm"
    click 47qta86y95 "47qta86y95" "47qta86y95"
    click 7vz1yqkdqo "7vz1yqkdqo" "7vz1yqkdqo"
    click 2uhj1oobbe "2uhj1oobbe" "2uhj1oobbe"
    click 4l39ap532m "4l39ap532m" "4l39ap532m"
    click icy7kw57ll "icy7kw57ll" "icy7kw57ll"
    click icy7kw57ll "icy7kw57ll" "icy7kw57ll"
    click v0t14r4lv2 "v0t14r4lv2" "v0t14r4lv2"
    click v0t14r4lv2 "v0t14r4lv2" "v0t14r4lv2"
    click frh74jp1jg "frh74jp1jg" "frh74jp1jg"
    click 4l39ap532m "4l39ap532m" "4l39ap532m"
    click t4cuk82upd "t4cuk82upd" "t4cuk82upd"
    click icy7kw57ll "icy7kw57ll" "icy7kw57ll"
    click wj5284rjb8 "wj5284rjb8" "wj5284rjb8"
    click wj5284rjb8 "wj5284rjb8" "wj5284rjb8"
    click l7i5qjffz1 "l7i5qjffz1" "l7i5qjffz1"
    click icy7kw57ll "icy7kw57ll" "icy7kw57ll"
    click vw8zbuzgod "vw8zbuzgod" "vw8zbuzgod"
    click vw8zbuzgod "vw8zbuzgod" "vw8zbuzgod"
    click j55n69o5i7 "j55n69o5i7" "j55n69o5i7"
    click ydyrhm9fkz "ydyrhm9fkz" "ydyrhm9fkz"
    click a58tdqlgfb "a58tdqlgfb" "a58tdqlgfb"
    click t04dles3gs "t04dles3gs" "t04dles3gs"
    click zfsjjfa5h6 "zfsjjfa5h6" "zfsjjfa5h6"
    click 5v1i2f1az4 "5v1i2f1az4" "5v1i2f1az4"
    click 4vf8sqyl70 "4vf8sqyl70" "4vf8sqyl70"
    click 9pb86bg0qi "9pb86bg0qi" "9pb86bg0qi"
    click wf0h6fo6h8 "wf0h6fo6h8" "wf0h6fo6h8"
    click 1qtib8s0uu "1qtib8s0uu" "1qtib8s0uu"
    click iagfrg0an6 "iagfrg0an6" "iagfrg0an6"
    click e717up82dy "e717up82dy" "e717up82dy"
    click 5v1i2f1az4 "5v1i2f1az4" "5v1i2f1az4"
    click bf9jlbogz1 "bf9jlbogz1" "bf9jlbogz1"
    click 2n3az4vori "2n3az4vori" "2n3az4vori"
    click iagfrg0an6 "iagfrg0an6" "iagfrg0an6"
    click wa07p8s7qm "wa07p8s7qm" "wa07p8s7qm"
    click bf9jlbogz1 "bf9jlbogz1" "bf9jlbogz1"
    click czzrbt1dsb "czzrbt1dsb" "czzrbt1dsb"
    click 2n3az4vori "2n3az4vori" "2n3az4vori"
    click 0sua91hqk7 "0sua91hqk7" "0sua91hqk7"
    click te0bcdks99 "te0bcdks99" "te0bcdks99"
    click qsu3efxcsp "qsu3efxcsp" "qsu3efxcsp"
    click ydyrhm9fkz "ydyrhm9fkz" "ydyrhm9fkz"
    click xsm25p5qf7 "xsm25p5qf7" "xsm25p5qf7"
    click xsm25p5qf7 "xsm25p5qf7" "xsm25p5qf7"
    click ayodtok1lb "ayodtok1lb" "ayodtok1lb"
    click ayodtok1lb "ayodtok1lb" "ayodtok1lb"
    click x9k0uusly8 "x9k0uusly8" "x9k0uusly8"
    click ayodtok1lb "ayodtok1lb" "ayodtok1lb"
    click b01n00fwkm "b01n00fwkm" "b01n00fwkm"
    click 9zctbmveoc "9zctbmveoc" "9zctbmveoc"
    click 1cbcpbc5no "1cbcpbc5no" "1cbcpbc5no"
    click l5z3ngnhjv "l5z3ngnhjv" "l5z3ngnhjv"
    click qurffyxc2d "qurffyxc2d" "qurffyxc2d"
    click se271xaurx "se271xaurx" "se271xaurx"
    click wzzac3ucto "wzzac3ucto" "wzzac3ucto"
    click sk3dza5671 "sk3dza5671" "sk3dza5671"
    click di86a7q7j0 "di86a7q7j0" "di86a7q7j0"
    click e3httj56zd "e3httj56zd" "e3httj56zd"
    click 5231692i67 "5231692i67" "5231692i67"
    click qxdd8mlll5 "qxdd8mlll5" "qxdd8mlll5"
    click u9ab712lfx "u9ab712lfx" "u9ab712lfx"
    click u9ab712lfx "u9ab712lfx" "u9ab712lfx"
    click vexxoicu6a "vexxoicu6a" "vexxoicu6a"
    click vexxoicu6a "vexxoicu6a" "vexxoicu6a"
    click 3s5kidc2wc "3s5kidc2wc" "3s5kidc2wc"
    click vexxoicu6a "vexxoicu6a" "vexxoicu6a"
    click j6salon8z4 "j6salon8z4" "j6salon8z4"
    click 3s5kidc2wc "3s5kidc2wc" "3s5kidc2wc"
    click u22hch23vs "u22hch23vs" "u22hch23vs"
    click nl0cxyid0x "nl0cxyid0x" "nl0cxyid0x"
    click ndm5er34sv "ndm5er34sv" "ndm5er34sv"
    click ndm5er34sv "ndm5er34sv" "ndm5er34sv"
    click 4n12f0orqv "4n12f0orqv" "4n12f0orqv"
    click 4n12f0orqv "4n12f0orqv" "4n12f0orqv"
    click d2uumx5mpk "d2uumx5mpk" "d2uumx5mpk"
    click ndm5er34sv "ndm5er34sv" "ndm5er34sv"
    click n69ynlsgag "n69ynlsgag" "n69ynlsgag"
    click 7hwtzuxjwc "7hwtzuxjwc" "7hwtzuxjwc"
    click 99q38lg97t "99q38lg97t" "99q38lg97t"
    click ndm5er34sv "ndm5er34sv" "ndm5er34sv"
    click sk3dza5671 "sk3dza5671" "sk3dza5671"
    click kgxiu8h9i5 "kgxiu8h9i5" "kgxiu8h9i5"
    click 9w2fwmdjtp "9w2fwmdjtp" "9w2fwmdjtp"
    click qw4n733f3t "qw4n733f3t" "qw4n733f3t"
    click sj6aezm25b "sj6aezm25b" "sj6aezm25b"
    click dxowhkk5n5 "dxowhkk5n5" "dxowhkk5n5"
    click kgxiu8h9i5 "kgxiu8h9i5" "kgxiu8h9i5"
    click kgxiu8h9i5 "kgxiu8h9i5" "kgxiu8h9i5"
    click p3914imkz7 "p3914imkz7" "p3914imkz7"
    click 5uyrxkfgza "5uyrxkfgza" "5uyrxkfgza"
    click wi6hu0ai62 "wi6hu0ai62" "wi6hu0ai62"
    click wi6hu0ai62 "wi6hu0ai62" "wi6hu0ai62"
    click 33jpsgsdxv "33jpsgsdxv" "33jpsgsdxv"
    click 33jpsgsdxv "33jpsgsdxv" "33jpsgsdxv"
    click ilu6o9n2x7 "ilu6o9n2x7" "ilu6o9n2x7"
    click 33jpsgsdxv "33jpsgsdxv" "33jpsgsdxv"
    click 33kryo3flh "33kryo3flh" "33kryo3flh"
    click fd7o3icva4 "fd7o3icva4" "fd7o3icva4"
    click 9q9zj5ndao "9q9zj5ndao" "9q9zj5ndao"
```
