# CIAM-Passwordless-Protect-Account-Recovery-Subflow
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
| ciam_companyLogo |  | true | textField | string | false | 
 


## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| ciam_recoveryValidationAttempts##SK##flowInstance |  | flowInstance |  | number | 0 | 2000 | true | property | 
 | ciam_recoveryLimit##SK##company | 5 | company |  | number | 0 | 2000 | true | property | 
 | ciam_errorMessage##SK##flowInstance |  | flowInstance |  | string | 0 | 2000 | true | property | 
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
    nc1ozqg2dy[Disable User] --> ymg2y1p8tf((EVAL))
    7050iwhzic[Check if Risk ID is empty] --> p46u12kavc((Evaluator))
    m1lp5172g7[PingOne Protect Analysis] --> zpg6zu1p21((EVAL))
    mxiurb5xux[Send email for threat detected] --> jozexysssa((EVAL))
    zmdygh0diw[Check if RiskID is empty] --> x1gd8ktif6((Evaluator))
    jozexysssa((EVAL)) --> nc1ozqg2dy[Disable User]
    8fh7taswpw((EVAL)) --> g3ie4cp1z5[Find user details]
    g3ie4cp1z5[Find user details] --> 0gubix0onw((EVAL))
    82g5jqcpg1((EVAL)) --> 5pgnxcibnw[PingOne Notifications]
    lonpqbsfiu((EVAL)) --> yj3z2ix7ge[Find user details]
    p46u12kavc((Evaluator)) --> 7dwvsl8sa8[Update Risk Evaluation - FAILURE]
    u0kjt3cxvi((EVAL)) --> 7050iwhzic[Check if Risk ID is empty]
    c69lo2tfh8((EVAL)) --> xj97e6huu4[Check for KNOWN DEVICE]
    yj3z2ix7ge[Find user details] --> 82g5jqcpg1((EVAL))
    8u4731kx7c((EVAL)) --> o4xxassgqz[Risk Score from PingOne Protect]
    5pgnxcibnw[PingOne Notifications] --> 8u4731kx7c((EVAL))
    3pbs4ekm6u[Is Validation Limit Reached?] --> 1brhauigps((EVAL))
    c6tyb3dxi1((EVAL)) --> ccqivhr3uh[Set error message]
    n0ympwqzwl((EVAL)) --> z1uxnr4psu[Set Validation Attempt To Zero]
    h4u1as8yg4[Recovery Code Form] --> n9tgrbpiz4((EVAL))
    ccqivhr3uh[Set error message] --> uh6ap9pj4p((EVAL))
    zvl6xidgq9((EVAL)) --> h4u1as8yg4[Recovery Code Form]
    z1uxnr4psu[Set Validation Attempt To Zero] --> zvl6xidgq9((EVAL))
    uh6ap9pj4p((EVAL)) --> 5vhs0j1lcd[Update error message]
    1brhauigps((EVAL)) --> xebw2nujq5[Node]
    t6hyz30ejn((EVAL)) --> rfwgqmb87x[Resend recovery code]
    mcc4xn7khm((EVAL)) --> ux2xzdhk0a[Does User Have Existing Password]
    1brhauigps((EVAL)) --> p7gnqv4r4t[Set New Password]
    n0ympwqzwl((EVAL)) --> ycc8uizvh4[User Cancelled]
    9o0jtjpq4i((Evaluator)) --> gm535zgls3[Passwords Do Not Match Error]
    4mpcqubv22((EVAL)) --> tfdqp94azq[OTP Resent Message]
    bl9wn96q7z((EVAL)) --> ao6h6cnxrq[Node]
    rtv1hwltfy[Split By User&#39;s Selection] --> bl9wn96q7z((EVAL))
    mkork4kg94((Evaluator)) --> km7ojt5kyt[Return Success Response]
    c6tyb3dxi1((EVAL)) --> jb2xut5506[Display Success Message]
    mcc4xn7khm((EVAL)) --> ixpij6bdtq[No User Found Error]
    jb2xut5506[Display Success Message] --> wy1q3vva1r((EVAL))
    klrsk927mu[Forgot Password Form] --> c52w1izn8f((EVAL))
    fecpsdg3u3((EVAL)) --> 16hlhgpr5h[Verify Passwords Match]
    eph6l2tfnr((EVAL)) --> fzf96tttyw[User Cancelled]
    u0kjt3cxvi((EVAL)) --> br93gz6bmz[Return Error Response]
    xd56mfv9sc[NOP UI Page] --> n9k3edxufj((EVAL))
    n9k3edxufj((EVAL)) --> klrsk927mu[Forgot Password Form]
    b9635u4i3w((EVAL)) --> klrsk927mu[Forgot Password Form]
    rtv1hwltfy[Split By User&#39;s Selection] --> fecpsdg3u3((EVAL))
    k0gh9sf1l8((EVAL)) --> 0jvt7xvej2[Lookup User]
    ux2xzdhk0a[Does User Have Existing Password] --> eph6l2tfnr((EVAL))
    dvr3wi8hib[Split By User&#39;s Selection] --> e6u7p021mj((EVAL))
    dvr3wi8hib[Split By User&#39;s Selection] --> v28wjjz61p((EVAL))
    eph6l2tfnr((EVAL)) --> ujwd58v2j5[Send Recovery Code]
    o88xkrpbve[Forgot Password Form] --> b9635u4i3w((EVAL))
    ujwd58v2j5[Send Recovery Code] --> n0ympwqzwl((EVAL))
    rfwgqmb87x[Resend recovery code] --> 4mpcqubv22((EVAL))
    c52w1izn8f((EVAL)) --> dvr3wi8hib[Split By User&#39;s Selection]
    0jvt7xvej2[Lookup User] --> mcc4xn7khm((EVAL))
    o8lq26j99n[Error] --> u0kjt3cxvi((EVAL))
    j3hvs9dks4[Success] --> mkork4kg94((Evaluator))
    e6u7p021mj((EVAL)) --> hu2l38mo64[User Cancelled]
    rtv1hwltfy[Split By User&#39;s Selection] --> t6hyz30ejn((EVAL))
    4mpcqubv22((EVAL)) --> vp9pfw2l9i[User Cancelled]
    wy1q3vva1r((EVAL)) --> sili5r3wur[Go to Sign On Success]
    n9tgrbpiz4((EVAL)) --> rtv1hwltfy[Split By User&#39;s Selection]
    p7gnqv4r4t[Set New Password] --> c6tyb3dxi1((EVAL))
    16hlhgpr5h[Verify Passwords Match] --> 9o0jtjpq4i((Evaluator))
    kj7e51zikv((EVAL)) --> jx18l5yjj0[Invalid password]
    xkvo347q5m((EVAL)) --> 3pbs4ekm6u[Is Validation Limit Reached?]
    v4rlsooi5t[Increment Validation Attempt] --> xkvo347q5m((EVAL))
    9o0jtjpq4i((Evaluator)) --> v4rlsooi5t[Increment Validation Attempt]
    5vhs0j1lcd[Update error message] --> kj7e51zikv((EVAL))
    xj97e6huu4[Check for KNOWN DEVICE] --> lonpqbsfiu((EVAL))
    zpg6zu1p21((EVAL)) --> m71wjatj9v[Invoke PingOne Protect subflow]
    m71wjatj9v[Invoke PingOne Protect subflow] --> pz7469or4k((Evaluator))
    pz7469or4k((Evaluator)) --> 5mvyk1j6oz[Get Values from PingOne Protect analysis]
    pz7469or4k((Evaluator)) --> akl8h5d22x[Get Values from PingOne Protect analysis]
    5mvyk1j6oz[Get Values from PingOne Protect analysis] --> c69lo2tfh8((EVAL))
    lonpqbsfiu((EVAL)) --> o4xxassgqz[Risk Score from PingOne Protect]
    o4xxassgqz[Risk Score from PingOne Protect] --> f4he7cr9jf((EVAL))
    f4he7cr9jf((EVAL)) --> llvrblwi3q[Return to calling node]
    o4xxassgqz[Risk Score from PingOne Protect] --> tr6ask2nn2((EVAL))
    tr6ask2nn2((EVAL)) --> 3b5q91z8tx[Return to calling node]
    o4xxassgqz[Risk Score from PingOne Protect] --> 4tfnhsx2bw((EVAL))
    mkork4kg94((Evaluator)) --> zmdygh0diw[Check if RiskID is empty]
    akl8h5d22x[Get Values from PingOne Protect analysis] --> 8fh7taswpw((EVAL))
    v28wjjz61p((EVAL)) --> 0wx52cpso1[Node]
    0gubix0onw((EVAL)) --> mxiurb5xux[Send email for threat detected]
    ymg2y1p8tf((EVAL)) --> 8eguhqxqpn[Node]
    0wx52cpso1[Node] --> k0gh9sf1l8((EVAL))
    4tfnhsx2bw((EVAL)) --> rsu5s043qp[Node]
    x1gd8ktif6((Evaluator)) --> hhileu4ydz[Update Risk Evaluation - SUCCESS]

    click nc1ozqg2dy "nc1ozqg2dy" "nc1ozqg2dy"
    click ymg2y1p8tf "ymg2y1p8tf" "ymg2y1p8tf"
    click 7050iwhzic "7050iwhzic" "7050iwhzic"
    click p46u12kavc "p46u12kavc" "p46u12kavc"
    click m1lp5172g7 "m1lp5172g7" "m1lp5172g7"
    click zpg6zu1p21 "zpg6zu1p21" "zpg6zu1p21"
    click mxiurb5xux "mxiurb5xux" "mxiurb5xux"
    click jozexysssa "jozexysssa" "jozexysssa"
    click zmdygh0diw "zmdygh0diw" "zmdygh0diw"
    click x1gd8ktif6 "x1gd8ktif6" "x1gd8ktif6"
    click jozexysssa "jozexysssa" "jozexysssa"
    click nc1ozqg2dy "nc1ozqg2dy" "nc1ozqg2dy"
    click 8fh7taswpw "8fh7taswpw" "8fh7taswpw"
    click g3ie4cp1z5 "g3ie4cp1z5" "g3ie4cp1z5"
    click g3ie4cp1z5 "g3ie4cp1z5" "g3ie4cp1z5"
    click 0gubix0onw "0gubix0onw" "0gubix0onw"
    click 82g5jqcpg1 "82g5jqcpg1" "82g5jqcpg1"
    click 5pgnxcibnw "5pgnxcibnw" "5pgnxcibnw"
    click lonpqbsfiu "lonpqbsfiu" "lonpqbsfiu"
    click yj3z2ix7ge "yj3z2ix7ge" "yj3z2ix7ge"
    click p46u12kavc "p46u12kavc" "p46u12kavc"
    click 7dwvsl8sa8 "7dwvsl8sa8" "7dwvsl8sa8"
    click u0kjt3cxvi "u0kjt3cxvi" "u0kjt3cxvi"
    click 7050iwhzic "7050iwhzic" "7050iwhzic"
    click c69lo2tfh8 "c69lo2tfh8" "c69lo2tfh8"
    click xj97e6huu4 "xj97e6huu4" "xj97e6huu4"
    click yj3z2ix7ge "yj3z2ix7ge" "yj3z2ix7ge"
    click 82g5jqcpg1 "82g5jqcpg1" "82g5jqcpg1"
    click 8u4731kx7c "8u4731kx7c" "8u4731kx7c"
    click o4xxassgqz "o4xxassgqz" "o4xxassgqz"
    click 5pgnxcibnw "5pgnxcibnw" "5pgnxcibnw"
    click 8u4731kx7c "8u4731kx7c" "8u4731kx7c"
    click 3pbs4ekm6u "3pbs4ekm6u" "3pbs4ekm6u"
    click 1brhauigps "1brhauigps" "1brhauigps"
    click c6tyb3dxi1 "c6tyb3dxi1" "c6tyb3dxi1"
    click ccqivhr3uh "ccqivhr3uh" "ccqivhr3uh"
    click n0ympwqzwl "n0ympwqzwl" "n0ympwqzwl"
    click z1uxnr4psu "z1uxnr4psu" "z1uxnr4psu"
    click h4u1as8yg4 "h4u1as8yg4" "h4u1as8yg4"
    click n9tgrbpiz4 "n9tgrbpiz4" "n9tgrbpiz4"
    click ccqivhr3uh "ccqivhr3uh" "ccqivhr3uh"
    click uh6ap9pj4p "uh6ap9pj4p" "uh6ap9pj4p"
    click zvl6xidgq9 "zvl6xidgq9" "zvl6xidgq9"
    click h4u1as8yg4 "h4u1as8yg4" "h4u1as8yg4"
    click z1uxnr4psu "z1uxnr4psu" "z1uxnr4psu"
    click zvl6xidgq9 "zvl6xidgq9" "zvl6xidgq9"
    click uh6ap9pj4p "uh6ap9pj4p" "uh6ap9pj4p"
    click 5vhs0j1lcd "5vhs0j1lcd" "5vhs0j1lcd"
    click 1brhauigps "1brhauigps" "1brhauigps"
    click xebw2nujq5 "xebw2nujq5" "xebw2nujq5"
    click t6hyz30ejn "t6hyz30ejn" "t6hyz30ejn"
    click rfwgqmb87x "rfwgqmb87x" "rfwgqmb87x"
    click mcc4xn7khm "mcc4xn7khm" "mcc4xn7khm"
    click ux2xzdhk0a "ux2xzdhk0a" "ux2xzdhk0a"
    click 1brhauigps "1brhauigps" "1brhauigps"
    click p7gnqv4r4t "p7gnqv4r4t" "p7gnqv4r4t"
    click n0ympwqzwl "n0ympwqzwl" "n0ympwqzwl"
    click ycc8uizvh4 "ycc8uizvh4" "ycc8uizvh4"
    click 9o0jtjpq4i "9o0jtjpq4i" "9o0jtjpq4i"
    click gm535zgls3 "gm535zgls3" "gm535zgls3"
    click 4mpcqubv22 "4mpcqubv22" "4mpcqubv22"
    click tfdqp94azq "tfdqp94azq" "tfdqp94azq"
    click bl9wn96q7z "bl9wn96q7z" "bl9wn96q7z"
    click ao6h6cnxrq "ao6h6cnxrq" "ao6h6cnxrq"
    click rtv1hwltfy "rtv1hwltfy" "rtv1hwltfy"
    click bl9wn96q7z "bl9wn96q7z" "bl9wn96q7z"
    click mkork4kg94 "mkork4kg94" "mkork4kg94"
    click km7ojt5kyt "km7ojt5kyt" "km7ojt5kyt"
    click c6tyb3dxi1 "c6tyb3dxi1" "c6tyb3dxi1"
    click jb2xut5506 "jb2xut5506" "jb2xut5506"
    click mcc4xn7khm "mcc4xn7khm" "mcc4xn7khm"
    click ixpij6bdtq "ixpij6bdtq" "ixpij6bdtq"
    click jb2xut5506 "jb2xut5506" "jb2xut5506"
    click wy1q3vva1r "wy1q3vva1r" "wy1q3vva1r"
    click klrsk927mu "klrsk927mu" "klrsk927mu"
    click c52w1izn8f "c52w1izn8f" "c52w1izn8f"
    click fecpsdg3u3 "fecpsdg3u3" "fecpsdg3u3"
    click 16hlhgpr5h "16hlhgpr5h" "16hlhgpr5h"
    click eph6l2tfnr "eph6l2tfnr" "eph6l2tfnr"
    click fzf96tttyw "fzf96tttyw" "fzf96tttyw"
    click u0kjt3cxvi "u0kjt3cxvi" "u0kjt3cxvi"
    click br93gz6bmz "br93gz6bmz" "br93gz6bmz"
    click xd56mfv9sc "xd56mfv9sc" "xd56mfv9sc"
    click n9k3edxufj "n9k3edxufj" "n9k3edxufj"
    click n9k3edxufj "n9k3edxufj" "n9k3edxufj"
    click klrsk927mu "klrsk927mu" "klrsk927mu"
    click b9635u4i3w "b9635u4i3w" "b9635u4i3w"
    click klrsk927mu "klrsk927mu" "klrsk927mu"
    click rtv1hwltfy "rtv1hwltfy" "rtv1hwltfy"
    click fecpsdg3u3 "fecpsdg3u3" "fecpsdg3u3"
    click k0gh9sf1l8 "k0gh9sf1l8" "k0gh9sf1l8"
    click 0jvt7xvej2 "0jvt7xvej2" "0jvt7xvej2"
    click ux2xzdhk0a "ux2xzdhk0a" "ux2xzdhk0a"
    click eph6l2tfnr "eph6l2tfnr" "eph6l2tfnr"
    click dvr3wi8hib "dvr3wi8hib" "dvr3wi8hib"
    click e6u7p021mj "e6u7p021mj" "e6u7p021mj"
    click dvr3wi8hib "dvr3wi8hib" "dvr3wi8hib"
    click v28wjjz61p "v28wjjz61p" "v28wjjz61p"
    click eph6l2tfnr "eph6l2tfnr" "eph6l2tfnr"
    click ujwd58v2j5 "ujwd58v2j5" "ujwd58v2j5"
    click o88xkrpbve "o88xkrpbve" "o88xkrpbve"
    click b9635u4i3w "b9635u4i3w" "b9635u4i3w"
    click ujwd58v2j5 "ujwd58v2j5" "ujwd58v2j5"
    click n0ympwqzwl "n0ympwqzwl" "n0ympwqzwl"
    click rfwgqmb87x "rfwgqmb87x" "rfwgqmb87x"
    click 4mpcqubv22 "4mpcqubv22" "4mpcqubv22"
    click c52w1izn8f "c52w1izn8f" "c52w1izn8f"
    click dvr3wi8hib "dvr3wi8hib" "dvr3wi8hib"
    click 0jvt7xvej2 "0jvt7xvej2" "0jvt7xvej2"
    click mcc4xn7khm "mcc4xn7khm" "mcc4xn7khm"
    click o8lq26j99n "o8lq26j99n" "o8lq26j99n"
    click u0kjt3cxvi "u0kjt3cxvi" "u0kjt3cxvi"
    click j3hvs9dks4 "j3hvs9dks4" "j3hvs9dks4"
    click mkork4kg94 "mkork4kg94" "mkork4kg94"
    click e6u7p021mj "e6u7p021mj" "e6u7p021mj"
    click hu2l38mo64 "hu2l38mo64" "hu2l38mo64"
    click rtv1hwltfy "rtv1hwltfy" "rtv1hwltfy"
    click t6hyz30ejn "t6hyz30ejn" "t6hyz30ejn"
    click 4mpcqubv22 "4mpcqubv22" "4mpcqubv22"
    click vp9pfw2l9i "vp9pfw2l9i" "vp9pfw2l9i"
    click wy1q3vva1r "wy1q3vva1r" "wy1q3vva1r"
    click sili5r3wur "sili5r3wur" "sili5r3wur"
    click n9tgrbpiz4 "n9tgrbpiz4" "n9tgrbpiz4"
    click rtv1hwltfy "rtv1hwltfy" "rtv1hwltfy"
    click p7gnqv4r4t "p7gnqv4r4t" "p7gnqv4r4t"
    click c6tyb3dxi1 "c6tyb3dxi1" "c6tyb3dxi1"
    click 16hlhgpr5h "16hlhgpr5h" "16hlhgpr5h"
    click 9o0jtjpq4i "9o0jtjpq4i" "9o0jtjpq4i"
    click kj7e51zikv "kj7e51zikv" "kj7e51zikv"
    click jx18l5yjj0 "jx18l5yjj0" "jx18l5yjj0"
    click xkvo347q5m "xkvo347q5m" "xkvo347q5m"
    click 3pbs4ekm6u "3pbs4ekm6u" "3pbs4ekm6u"
    click v4rlsooi5t "v4rlsooi5t" "v4rlsooi5t"
    click xkvo347q5m "xkvo347q5m" "xkvo347q5m"
    click 9o0jtjpq4i "9o0jtjpq4i" "9o0jtjpq4i"
    click v4rlsooi5t "v4rlsooi5t" "v4rlsooi5t"
    click 5vhs0j1lcd "5vhs0j1lcd" "5vhs0j1lcd"
    click kj7e51zikv "kj7e51zikv" "kj7e51zikv"
    click xj97e6huu4 "xj97e6huu4" "xj97e6huu4"
    click lonpqbsfiu "lonpqbsfiu" "lonpqbsfiu"
    click zpg6zu1p21 "zpg6zu1p21" "zpg6zu1p21"
    click m71wjatj9v "m71wjatj9v" "m71wjatj9v"
    click m71wjatj9v "m71wjatj9v" "m71wjatj9v"
    click pz7469or4k "pz7469or4k" "pz7469or4k"
    click pz7469or4k "pz7469or4k" "pz7469or4k"
    click 5mvyk1j6oz "5mvyk1j6oz" "5mvyk1j6oz"
    click pz7469or4k "pz7469or4k" "pz7469or4k"
    click akl8h5d22x "akl8h5d22x" "akl8h5d22x"
    click 5mvyk1j6oz "5mvyk1j6oz" "5mvyk1j6oz"
    click c69lo2tfh8 "c69lo2tfh8" "c69lo2tfh8"
    click lonpqbsfiu "lonpqbsfiu" "lonpqbsfiu"
    click o4xxassgqz "o4xxassgqz" "o4xxassgqz"
    click o4xxassgqz "o4xxassgqz" "o4xxassgqz"
    click f4he7cr9jf "f4he7cr9jf" "f4he7cr9jf"
    click f4he7cr9jf "f4he7cr9jf" "f4he7cr9jf"
    click llvrblwi3q "llvrblwi3q" "llvrblwi3q"
    click o4xxassgqz "o4xxassgqz" "o4xxassgqz"
    click tr6ask2nn2 "tr6ask2nn2" "tr6ask2nn2"
    click tr6ask2nn2 "tr6ask2nn2" "tr6ask2nn2"
    click 3b5q91z8tx "3b5q91z8tx" "3b5q91z8tx"
    click o4xxassgqz "o4xxassgqz" "o4xxassgqz"
    click 4tfnhsx2bw "4tfnhsx2bw" "4tfnhsx2bw"
    click mkork4kg94 "mkork4kg94" "mkork4kg94"
    click zmdygh0diw "zmdygh0diw" "zmdygh0diw"
    click akl8h5d22x "akl8h5d22x" "akl8h5d22x"
    click 8fh7taswpw "8fh7taswpw" "8fh7taswpw"
    click v28wjjz61p "v28wjjz61p" "v28wjjz61p"
    click 0wx52cpso1 "0wx52cpso1" "0wx52cpso1"
    click 0gubix0onw "0gubix0onw" "0gubix0onw"
    click mxiurb5xux "mxiurb5xux" "mxiurb5xux"
    click ymg2y1p8tf "ymg2y1p8tf" "ymg2y1p8tf"
    click 8eguhqxqpn "8eguhqxqpn" "8eguhqxqpn"
    click 0wx52cpso1 "0wx52cpso1" "0wx52cpso1"
    click k0gh9sf1l8 "k0gh9sf1l8" "k0gh9sf1l8"
    click 4tfnhsx2bw "4tfnhsx2bw" "4tfnhsx2bw"
    click rsu5s043qp "rsu5s043qp" "rsu5s043qp"
    click x1gd8ktif6 "x1gd8ktif6" "x1gd8ktif6"
    click hhileu4ydz "hhileu4ydz" "hhileu4ydz"
```
