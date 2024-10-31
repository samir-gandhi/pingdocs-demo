# CIAM-Passwordless-Protect-Account-Recovery-Subflow

### Flow Diagram
```mermaid
flowchart LR
    nc1ozqg2dy[["Disable User"]] --> ymg2y1p8tf(("EVAL"))
    7050iwhzic[["Check if Risk ID is empty"]] --> p46u12kavc(("Evaluator"))
    m1lp5172g7[["PingOne Protect Analysis"]] --> zpg6zu1p21(("EVAL"))
    mxiurb5xux[["Send email for threat detected"]] --> jozexysssa(("EVAL"))
    zmdygh0diw[["Check if RiskID is empty"]] --> x1gd8ktif6(("Evaluator"))
    jozexysssa(("EVAL")) --> nc1ozqg2dy[["Disable User"]]
    8fh7taswpw(("EVAL")) --> g3ie4cp1z5[["Find user details"]]
    g3ie4cp1z5[["Find user details"]] --> 0gubix0onw(("EVAL"))
    82g5jqcpg1(("EVAL")) --> 5pgnxcibnw[["PingOne Notifications"]]
    lonpqbsfiu(("EVAL")) --> yj3z2ix7ge[["Find user details"]]
    p46u12kavc(("Evaluator")) --> 7dwvsl8sa8[["Update Risk Evaluation - FAILURE"]]
    u0kjt3cxvi(("EVAL")) --> 7050iwhzic[["Check if Risk ID is empty"]]
    c69lo2tfh8(("EVAL")) --> xj97e6huu4[["Check for KNOWN DEVICE"]]
    yj3z2ix7ge[["Find user details"]] --> 82g5jqcpg1(("EVAL"))
    8u4731kx7c(("EVAL")) --> o4xxassgqz[["Risk Score from PingOne Protect"]]
    5pgnxcibnw[["PingOne Notifications"]] --> 8u4731kx7c(("EVAL"))
    3pbs4ekm6u[["Is Validation Limit Reached?"]] --> 1brhauigps(("EVAL"))
    c6tyb3dxi1(("EVAL")) --> ccqivhr3uh[["Set error message"]]
    n0ympwqzwl(("EVAL")) --> z1uxnr4psu[["Set Validation Attempt To Zero"]]
    h4u1as8yg4[["Recovery Code Form"]] --> n9tgrbpiz4(("EVAL"))
    ccqivhr3uh[["Set error message"]] --> uh6ap9pj4p(("EVAL"))
    zvl6xidgq9(("EVAL")) --> h4u1as8yg4[["Recovery Code Form"]]
    z1uxnr4psu[["Set Validation Attempt To Zero"]] --> zvl6xidgq9(("EVAL"))
    uh6ap9pj4p(("EVAL")) --> 5vhs0j1lcd[["Update error message"]]
    1brhauigps(("EVAL")) --> xebw2nujq5[["Node"]]
    t6hyz30ejn(("EVAL")) --> rfwgqmb87x[["Resend recovery code"]]
    mcc4xn7khm(("EVAL")) --> ux2xzdhk0a[["Does User Have Existing Password"]]
    1brhauigps(("EVAL")) --> p7gnqv4r4t[["Set New Password"]]
    n0ympwqzwl(("EVAL")) --> ycc8uizvh4[["User Cancelled"]]
    9o0jtjpq4i(("Evaluator")) --> gm535zgls3[["Passwords Do Not Match Error"]]
    4mpcqubv22(("EVAL")) --> tfdqp94azq[["OTP Resent Message"]]
    bl9wn96q7z(("EVAL")) --> ao6h6cnxrq[["Node"]]
    rtv1hwltfy[["Split By Users Selection"]] --> bl9wn96q7z(("EVAL"))
    mkork4kg94(("Evaluator")) --> km7ojt5kyt[["Return Success Response"]]
    c6tyb3dxi1(("EVAL")) --> jb2xut5506[["Display Success Message"]]
    mcc4xn7khm(("EVAL")) --> ixpij6bdtq[["No User Found Error"]]
    jb2xut5506[["Display Success Message"]] --> wy1q3vva1r(("EVAL"))
    klrsk927mu[["Forgot Password Form"]] --> c52w1izn8f(("EVAL"))
    fecpsdg3u3(("EVAL")) --> 16hlhgpr5h[["Verify Passwords Match"]]
    eph6l2tfnr(("EVAL")) --> fzf96tttyw[["User Cancelled"]]
    u0kjt3cxvi(("EVAL")) --> br93gz6bmz[["Return Error Response"]]
    xd56mfv9sc[["NOP UI Page"]] --> n9k3edxufj(("EVAL"))
    n9k3edxufj(("EVAL")) --> klrsk927mu[["Forgot Password Form"]]
    b9635u4i3w(("EVAL")) --> klrsk927mu[["Forgot Password Form"]]
    rtv1hwltfy[["Split By Users Selection"]] --> fecpsdg3u3(("EVAL"))
    k0gh9sf1l8(("EVAL")) --> 0jvt7xvej2[["Lookup User"]]
    ux2xzdhk0a[["Does User Have Existing Password"]] --> eph6l2tfnr(("EVAL"))
    dvr3wi8hib[["Split By Users Selection"]] --> e6u7p021mj(("EVAL"))
    dvr3wi8hib[["Split By Users Selection"]] --> v28wjjz61p(("EVAL"))
    eph6l2tfnr(("EVAL")) --> ujwd58v2j5[["Send Recovery Code"]]
    o88xkrpbve[["Forgot Password Form"]] --> b9635u4i3w(("EVAL"))
    ujwd58v2j5[["Send Recovery Code"]] --> n0ympwqzwl(("EVAL"))
    rfwgqmb87x[["Resend recovery code"]] --> 4mpcqubv22(("EVAL"))
    c52w1izn8f(("EVAL")) --> dvr3wi8hib[["Split By Users Selection"]]
    0jvt7xvej2[["Lookup User"]] --> mcc4xn7khm(("EVAL"))
    o8lq26j99n[["Error"]] --> u0kjt3cxvi(("EVAL"))
    j3hvs9dks4[["Success"]] --> mkork4kg94(("Evaluator"))
    e6u7p021mj(("EVAL")) --> hu2l38mo64[["User Cancelled"]]
    rtv1hwltfy[["Split By Users Selection"]] --> t6hyz30ejn(("EVAL"))
    4mpcqubv22(("EVAL")) --> vp9pfw2l9i[["User Cancelled"]]
    wy1q3vva1r(("EVAL")) --> sili5r3wur[["Go to Sign On Success"]]
    n9tgrbpiz4(("EVAL")) --> rtv1hwltfy[["Split By Users Selection"]]
    p7gnqv4r4t[["Set New Password"]] --> c6tyb3dxi1(("EVAL"))
    16hlhgpr5h[["Verify Passwords Match"]] --> 9o0jtjpq4i(("Evaluator"))
    kj7e51zikv(("EVAL")) --> jx18l5yjj0[["Invalid password"]]
    xkvo347q5m(("EVAL")) --> 3pbs4ekm6u[["Is Validation Limit Reached?"]]
    v4rlsooi5t[["Increment Validation Attempt"]] --> xkvo347q5m(("EVAL"))
    9o0jtjpq4i(("Evaluator")) --> v4rlsooi5t[["Increment Validation Attempt"]]
    5vhs0j1lcd[["Update error message"]] --> kj7e51zikv(("EVAL"))
    xj97e6huu4[["Check for KNOWN DEVICE"]] --> lonpqbsfiu(("EVAL"))
    zpg6zu1p21(("EVAL")) --> m71wjatj9v[["Invoke PingOne Protect subflow"]]
    m71wjatj9v[["Invoke PingOne Protect subflow"]] --> pz7469or4k(("Evaluator"))
    pz7469or4k(("Evaluator")) --> 5mvyk1j6oz[["Get Values from PingOne Protect analysis"]]
    pz7469or4k(("Evaluator")) --> akl8h5d22x[["Get Values from PingOne Protect analysis"]]
    5mvyk1j6oz[["Get Values from PingOne Protect analysis"]] --> c69lo2tfh8(("EVAL"))
    lonpqbsfiu(("EVAL")) --> o4xxassgqz[["Risk Score from PingOne Protect"]]
    o4xxassgqz[["Risk Score from PingOne Protect"]] --> f4he7cr9jf(("EVAL"))
    f4he7cr9jf(("EVAL")) --> llvrblwi3q[["Return to calling node"]]
    o4xxassgqz[["Risk Score from PingOne Protect"]] --> tr6ask2nn2(("EVAL"))
    tr6ask2nn2(("EVAL")) --> 3b5q91z8tx[["Return to calling node"]]
    o4xxassgqz[["Risk Score from PingOne Protect"]] --> 4tfnhsx2bw(("EVAL"))
    mkork4kg94(("Evaluator")) --> zmdygh0diw[["Check if RiskID is empty"]]
    akl8h5d22x[["Get Values from PingOne Protect analysis"]] --> 8fh7taswpw(("EVAL"))
    v28wjjz61p(("EVAL")) --> 0wx52cpso1[["Node"]]
    0gubix0onw(("EVAL")) --> mxiurb5xux[["Send email for threat detected"]]
    ymg2y1p8tf(("EVAL")) --> 8eguhqxqpn[["Node"]]
    0wx52cpso1[["Node"]] --> k0gh9sf1l8(("EVAL"))
    4tfnhsx2bw(("EVAL")) --> rsu5s043qp[["Node"]]
    x1gd8ktif6(("Evaluator")) --> hhileu4ydz[["Update Risk Evaluation - SUCCESS"]]


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
 


## Subflows
| Label | Capatability Name | Node ID | Node Title | Version ID |                                                                                                                                                             
|----------------------------------|-----------------|-----------------|-----------------|-----------------|
| [CIAM-Passwordless-Protect-Threat-Detection-Subflow](../CIAMPasswordlessProtectThreatDetectionSubflow/index.md) | startSubFlow | [m71wjatj9v](./nodes/m71wjatj9v.md) | Invoke PingOne Protect subflow | -1 | 
 