# OOTB - Device Management - Main Flow

### Flow Diagram
```mermaid
flowchart LR
    4os42modvj(("EVAL")) --> pks46w5ks6[["Filter Unusable Devices"]]
    pks46w5ks6[["Filter Unusable Devices"]] --> 4wqs0nbs1v(("EVAL"))
    xz5zj0bo0z[["Device Registration Result"]] --> lu3t9lz7j(("EVAL"))
    pthery4nru[["NOP UI Page"]] --> 1lngxsfyuk(("EVAL"))
    61gkn04fvn[["Register Device"]] --> gmbeads147(("EVAL"))
    vbk955oxjg(("EVAL")) --> 8sttri4np9[["Check If Device Removal Warning Is Needed"]]
    8sttri4np9[["Check If Device Removal Warning Is Needed"]] --> 4os42modvj(("EVAL"))
    efiecys0xw(("EVAL")) --> 7rwri5u6ra[["Get User Info"]]
    at5tmglpow[["Error"]] --> 6rcgg8opng(("EVAL"))
    4wqs0nbs1v(("EVAL")) --> kdfb05yf1m[["Display User Devices"]]
    lu3t9lz7j(("EVAL")) --> 3qniq7ika1[["Teleport"]]
    fwpzd4lh0q(("EVAL")) --> eevgv227kt[["Teleport"]]
    j6pgj7seov[["MFA Form Selection"]] --> 2x2le9q98(("EVAL"))
    hhnj8v9hed(("EVAL")) --> m0gjea9ddr[["Return Success Response"]]
    2x2le9q98(("EVAL")) --> up4jkblnks[["Enable MFA for user"]]
    r8nxemp506(("Evaluator")) --> 6p1jps948p[["Teleport"]]
    up4jkblnks[["Enable MFA for user"]] --> r8nxemp506(("Evaluator"))
    3jsczqq7hm(("Evaluator")) --> bpuhlgwdhe[["Teleport"]]
    rxrwt223m5(("EVAL")) --> rsj0knmukp[["Check If MFA Is enabled?"]]
    17n6cajfer(("Evaluator")) --> odx7hiwkjx[["Teleport"]]
    o5huuauebn(("EVAL")) --> u04j1zkybt[["Teleport"]]
    xz5zj0bo0z[["Device Registration Result"]] --> xytgoh995y(("EVAL"))
    rsj0knmukp[["Check If MFA Is enabled?"]] --> 3jsczqq7hm(("Evaluator"))
    1lngxsfyuk(("EVAL")) --> d915blmeth[["Device Registration"]]
    dpv60nrlu4(("EVAL")) --> powjrjqmwn[["Delete Device"]]
    ebzcromrpm[["Selected Device"]] --> to6mgd2tyh(("EVAL"))
    to6mgd2tyh(("EVAL")) --> j4l954l5hz[["Selected Device Screen"]]
    cb42qgfnjd(("EVAL")) --> 43e7ccsg4e[["Teleport"]]
    kh69z64byb(("EVAL")) --> zvpx8o3npf[["Teleport"]]
    d915blmeth[["Device Registration"]] --> 17n6cajfer(("Evaluator"))
    gz9gke603k[["User Selection"]] --> q3ibsmt4qr(("EVAL"))
    5mes9ynjey(("EVAL")) --> 4i8hh3qp83[["Get User Devices"]]
    zmy34kmwpn(("Evaluator")) --> 7ujaohyyg9[["Teleport"]]
    9pekqghawg[["Device Selection"]] --> 5mes9ynjey(("EVAL"))
    q3ibsmt4qr(("EVAL")) --> 5p3ahp4peh[["Teleport"]]
    kdfb05yf1m[["Display User Devices"]] --> 0jgff1lx32(("EVAL"))
    6rcgg8opng(("EVAL")) --> fzdgjjow89[["Error Screen"]]
    921411zeq1(("EVAL")) --> 6nafzw7by5[["Teleport"]]
    fzdgjjow89[["Error Screen"]] --> miwpvke4ky(("EVAL"))
    sjedcfzfgi(("EVAL")) --> lxdqcv1aa7[["Check If User Can Add New Device"]]
    4i8hh3qp83[["Get User Devices"]] --> sjedcfzfgi(("EVAL"))
    gz9gke603k[["User Selection"]] --> kh69z64byb(("EVAL"))
    0jgff1lx32(("EVAL")) --> gz9gke603k[["User Selection"]]
    c6dxhfi5rb(("EVAL")) --> 45rd8ajb4g[["Teleport"]]
    gz9gke603k[["User Selection"]] --> ako0e9ds26(("EVAL"))
    ako0e9ds26(("EVAL")) --> 5b5ckjqcix[["Get Device Info"]]
    5b5ckjqcix[["Get Device Info"]] --> 088nn24g3r(("EVAL"))
    088nn24g3r(("EVAL")) --> zekirrx0pv[["Teleport"]]
    vp8o2mc12q[["Selected Device Screen Selection"]] --> dpv60nrlu4(("EVAL"))
    v9xx0rido4[["Set Device As Default"]] --> c6dxhfi5rb(("EVAL"))
    vp8o2mc12q[["Selected Device Screen Selection"]] --> fvt3dt1sk1(("EVAL"))
    c6dxhfi5rb(("EVAL")) --> vlfgac0ix0[["Teleport"]]
    0mbvscfh8v(("EVAL")) --> mr62wpbo3z[["Update Device Name"]]
    mr62wpbo3z[["Update Device Name"]] --> cb42qgfnjd(("EVAL"))
    cb42qgfnjd(("EVAL")) --> wmy2hwaazd[["Teleport"]]
    vp8o2mc12q[["Selected Device Screen Selection"]] --> 0mbvscfh8v(("EVAL"))
    921411zeq1(("EVAL")) --> qcqgec2dmb[["Teleport"]]
    j4l954l5hz[["Selected Device Screen"]] --> 2tif2w7s85(("EVAL"))
    2tif2w7s85(("EVAL")) --> vp8o2mc12q[["Selected Device Screen Selection"]]
    xytgoh995y(("EVAL")) --> erir79d26y[["Teleport"]]
    gmbeads147(("EVAL")) --> pthery4nru[["NOP UI Page"]]
    fvt3dt1sk1(("EVAL")) --> v9xx0rido4[["Set Device As Default"]]
    powjrjqmwn[["Delete Device"]] --> 921411zeq1(("EVAL"))
    3jsczqq7hm(("Evaluator")) --> o925yy0p7r[["MFA Form"]]
    vp8o2mc12q[["Selected Device Screen Selection"]] --> o5huuauebn(("EVAL"))
    gz9gke603k[["User Selection"]] --> fwpzd4lh0q(("EVAL"))
    j6pgj7seov[["MFA Form Selection"]] --> e9gg1lr1db(("EVAL"))
    e9gg1lr1db(("EVAL")) --> b3jh5zpngp[["Teleport"]]
    sjedcfzfgi(("EVAL")) --> srhu2uexj1[["Teleport"]]
    lxdqcv1aa7[["Check If User Can Add New Device"]] --> vbk955oxjg(("EVAL"))
    7rwri5u6ra[["Get User Info"]] --> rxrwt223m5(("EVAL"))
    rxrwt223m5(("EVAL")) --> ls0q7pxpla[["Teleport"]]
    o925yy0p7r[["MFA Form"]] --> qy6uai4d4r(("EVAL"))
    qy6uai4d4r(("EVAL")) --> j6pgj7seov[["MFA Form Selection"]]
    2dvdm35xe5[["Success"]] --> hhnj8v9hed(("EVAL"))
    r8nxemp506(("Evaluator")) --> ev94io1fpf[["Teleport"]]
    m0gjea9ddr[["Return Success Response"]] --> zmy34kmwpn(("Evaluator"))
    17n6cajfer(("Evaluator")) --> xz5zj0bo0z[["Device Registration Result"]]
    xz5zj0bo0z[["Device Registration Result"]] --> wxyu359jnv(("EVAL"))
    wxyu359jnv(("EVAL")) --> 9jl5ynfchd[["Teleport"]]
    umf4ie39n[["Set Flow Variables"]] --> efiecys0xw(("EVAL"))
    miwpvke4ky(("EVAL")) --> yaorwpte52[["Send Response"]]


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
 


## Variables
| Variable | Value | Context | Display Name | Field Type | Min | Max | Mutable | Type |                                                                                                                                                                
|----------------------------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| ciam_companyName##SK##company | Ping Identity | company |  | string | 0 | 2000 | false | property | 
 | ciam_emailOtpEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_fidoPasskeyEnabled##SK##company | false | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_logoStyle##SK##company | width: 65px; height: 65px; | company | CSS style for company logo | string | 0 | 2000 | true | property | 
 | ciam_logoUrl##SK##company | https://assets.pingone.com/ux/ui-library/5.0.2/images/logo-pingidentity.png | company | URL of company logo | string | 0 | 2000 | true | property | 
 | ciam_smsOtpEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 


## Subflows
| Label | Capatability Name | Node ID | Node Title | Version ID |                                                                                                                                                             
|----------------------------------|-----------------|-----------------|-----------------|-----------------|
| [OOTB - Device Registration - Subflow - 1](../OOTBDeviceRegistrationSubflow1/index.md) | startUiSubFlow | [d915blmeth](./nodes/d915blmeth.md) | Device Registration | -1 | 
 