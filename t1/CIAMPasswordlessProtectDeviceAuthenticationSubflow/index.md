# CIAM-Passwordless-Protect-Device-Authentication-Subflow

### Flow Diagram
```mermaid
flowchart LR
    mtaqacdw1m(("Evaluator")) --> 8jrbqcts2g["Create MFA Device"]
    hk00gx2f95(("EVAL")) --> onogvjusk6["Prompt For OTP"]
    qw4n733f3t(("EVAL")) --> li0d8slgjx["Send email for new device"]
    7jufzmg1rk["Activate MFA Device"] --> qw4n733f3t(("EVAL"))
    8jrbqcts2g["Create MFA Device"] --> hk00gx2f95(("EVAL"))
    kho2rpwvb7(("Evaluator")) --> 7jufzmg1rk["Activate MFA Device"]
    onogvjusk6["Prompt For OTP"] --> kho2rpwvb7(("Evaluator"))
    78i0a08xfl["Send email for threat detection"] --> iz5nper189(("EVAL"))
    gsmghrxxoy["Check for KNOWN DEVICE"] --> nl0cxyid0x(("EVAL"))
    99q38lg97t(("EVAL")) --> sqdggkol0g["Node"]
    iloobtovwh(("EVAL")) --> dxowhkk5n5["Check if Risk Policy ID is empty"]
    iz5nper189(("EVAL")) --> 7hwtzuxjwc["Disable user"]
    n69ynlsgag(("EVAL")) --> nf4hv96sui["Check MFA devices size"]
    cb4rka2li0(("EVAL")) --> 78i0a08xfl["Send email for threat detection"]
    x8ainlbr6x(("EVAL")) --> ndm5er34sv["Risk Score from PingOne Protect"]
    j6salon8z4["Get Values from PingOne Protect analysis"] --> cb4rka2li0(("EVAL"))
    ahjplbui3q["PingOne Notifications"] --> x8ainlbr6x(("EVAL"))
    pt24r4nafa(("EVAL")) --> 3y03qc0kxe["Find user details"]
    mtaqacdw1m(("Evaluator")) --> 5231692i67["Return to calling node."]
    4oyc5l9npk(("EVAL")) --> 737gi6ip3e["Node"]
    u22hch23vs(("EVAL")) --> gsmghrxxoy["Check for KNOWN DEVICE"]
    zfpuewwuhl["PingOne Protect Analysis"] --> pt24r4nafa(("EVAL"))
    3y03qc0kxe["Find user details"] --> qxdd8mlll5(("EVAL"))
    nl0cxyid0x(("EVAL")) --> ahjplbui3q["PingOne Notifications"]
    li0d8slgjx["Send email for new device"] --> e3httj56zd(("EVAL"))
    737gi6ip3e["Node"] --> 9vk797lpxx(("EVAL"))
    nf4hv96sui["Check MFA devices size"] --> mtaqacdw1m(("Evaluator"))
    1cbcpbc5no(("EVAL")) --> 4psx471uwp["Authentication Required"]
    h8dtvwld36(("EVAL")) --> 76reddil11["Node"]
    r0hto2xun7["Present OTP Form"] --> l5z3ngnhjv(("EVAL"))
    1gtc5d0awz(("EVAL")) --> kok73n8hkt["to otp"]
    4psx471uwp["Authentication Required"] --> 1gtc5d0awz(("EVAL"))
    qurffyxc2d["Split by user selection "] --> gsw5wwtm7t(("EVAL"))
    en7y953x31["Get authMethod Value"] --> 0w6twuixxq(("EVAL"))
    fzjj3nuh7m(("EVAL")) --> dxsjn36392["Node"]
    mt9kvt7hnn(("EVAL")) --> fgc8woctfo["Validate Passcode"]
    qurffyxc2d["Split by user selection "] --> 00j11fkhbx(("EVAL"))
    fzjj3nuh7m(("EVAL")) --> uz6hhdt9gv["OTP Resent Message"]
    zxfluj3oxa["OTP"] --> b0csz8cgnl(("EVAL"))
    qurffyxc2d["Split by user selection "] --> ig2ndq8bf2(("EVAL"))
    00j11fkhbx(("EVAL")) --> beakf43h8t["Node"]
    gsw5wwtm7t(("EVAL")) --> r6lnkuy0yh["Transform Passcode To Lowercase"]
    ig2ndq8bf2(("EVAL")) --> m1e0cw0ygl["Resend OTP"]
    m1e0cw0ygl["Resend OTP"] --> fzjj3nuh7m(("EVAL"))
    r6lnkuy0yh["Transform Passcode To Lowercase"] --> mt9kvt7hnn(("EVAL"))
    hdc8oa72ci["Is invalidOTP Error"] --> 8h5tjkrug9(("EVAL"))
    v97rmwpban(("EVAL")) --> 5pixttpidw["Invalid Passcode Error"]
    gntsn38l9s["CIAM - Magic Link Authentication"] --> 51zazld6jz(("EVAL"))
    5uyrxkfgza(("EVAL")) --> tidk1pmqix["Return Success Response"]
    8h5tjkrug9(("EVAL")) --> mmojm56jlj["Node"]
    uoyh9kzwil["Device Selection"] --> bhgtvbjvu1(("EVAL"))
    se271xaurx(("EVAL")) --> uwfrx6s60u["Node"]
    vr1msssq3l(("EVAL")) --> wpbqyomp7z["Node"]
    wa07p8s7qm["Not Magic Link?"] --> vr1msssq3l(("EVAL"))
    vul5k2q2dw(("EVAL")) --> te0bcdks99["Magic Link Authentication"]
    wa07p8s7qm["Not Magic Link?"] --> vul5k2q2dw(("EVAL"))
    imhudhsy1w(("EVAL")) --> e717up82dy["Device Selected By The User"]
    wa07p8s7qm["Not Magic Link?"] --> imhudhsy1w(("EVAL"))
    j8lmuiytzs["Is MFA Enabled?"] --> bf9jlbogz1(("EVAL"))
    bhgtvbjvu1(("EVAL")) --> 1qtib8s0uu["Select Authentication Device"]
    0sua91hqk7(("EVAL")) --> 10oaokas61["Start MFA Authentication"]
    845xzgf4bk(("EVAL")) --> ulsqznx6ut["Is Constraint Violation Error"]
    51zazld6jz(("EVAL")) --> 5gs9h0ar04["Node"]
    3a77bpgwom(("EVAL")) --> y7f8x8dkw2["Node"]
    zfsjjfa5h6["Present FIDO2 Form "] --> 9pb86bg0qi(("EVAL"))
    wf0h6fo6h8["Split By User&#39;s Selection"] --> ay2mm4z4xe(("EVAL"))
    ulsqznx6ut["Is Constraint Violation Error"] --> fu06ckn12l(("EVAL"))
    fj8w62y4z3["Assert FIDO Device Authentication"] --> 845xzgf4bk(("EVAL"))
    fu06ckn12l(("EVAL")) --> y8pxpynfle["Invalid Device Error"]
    7vrrd3uuhm(("EVAL")) --> en7y953x31["Get authMethod Value"]
    1lam7h7jbc["Split By Subflow&#39;s Result"] --> 9fzm9oj8fd(("EVAL"))
    qsu3efxcsp(("EVAL")) --> 1lam7h7jbc["Split By Subflow&#39;s Result"]
    6yu5p2iz3r(("EVAL")) --> ms19ql02hi["Get MFA Status"]
    en7y953x31["Get authMethod Value"] --> 0w6twuixxq(("EVAL"))
    t6p5s6t603["Get WebAuthn Browser Compatibility"] --> 4oyc5l9npk(("EVAL"))
    10uwd1ccc4["Filter Unusable Devices"] --> se271xaurx(("EVAL"))
    wzzac3ucto["Create Masked Devices"] --> 6yu5p2iz3r(("EVAL"))
    fd7o3icva4(("EVAL")) --> j8lmuiytzs["Is MFA Enabled?"]
    ms19ql02hi["Get MFA Status"] --> fd7o3icva4(("EVAL"))
    3nn0mw8jkt(("EVAL")) --> 61c9e2dt59["Node"]
    51zazld6jz(("EVAL")) --> nvxwg0vum3["Node"]
    9fzm9oj8fd(("EVAL")) --> lgn9kliiqj["Node"]
    b0csz8cgnl(("EVAL")) --> fq7l0s8w2s["Mask Device"]
    1lam7h7jbc["Split By Subflow&#39;s Result"] --> lylme68jbw(("EVAL"))
    0w6twuixxq(("EVAL")) --> 5sb0db3vb0["Node"]
    7vpjww2ek2["FIDO2"] --> t04dles3gs(("EVAL"))
    9vk797lpxx(("EVAL")) --> 10uwd1ccc4["Filter Unusable Devices"]
    wf0h6fo6h8["Split By User&#39;s Selection"] --> 3nn0mw8jkt(("EVAL"))
    k46n95w9eo["Success "] --> 5uyrxkfgza(("EVAL"))
    hdc8oa72ci["Is invalidOTP Error"] --> v97rmwpban(("EVAL"))
    7vrrd3uuhm(("EVAL")) --> hdc8oa72ci["Is invalidOTP Error"]
    fgc8woctfo["Validate Passcode"] --> 7vrrd3uuhm(("EVAL"))
    zbhvblc83s["Authentication Method Selection"] --> ybwxgols9w(("EVAL"))
    4psx471uwp["Authentication Required"] --> h8dtvwld36(("EVAL"))
    ybwxgols9w(("EVAL")) --> 9zctbmveoc["Enrich Device Details"]
    iloobtovwh(("EVAL")) --> dwhgyxkavz["Error Error Response"]
    qsu3efxcsp(("EVAL")) --> muund54c7j["Node"]
    6p4frzqpp1["Get Origin"] --> sk7vd2o3r7(("EVAL"))
    845xzgf4bk(("EVAL")) --> dp43hy7h76["Get authMethod Value"]
    5v1i2f1az4(("EVAL")) --> cbapcifpyy["Node"]
    nydopq0ve3(("EVAL")) --> qzuk2c4cdb["Node"]
    nydopq0ve3(("EVAL")) --> t6p5s6t603["Get WebAuthn Browser Compatibility"]
    fq7l0s8w2s["Mask Device"] --> bdjeulfdki(("EVAL"))
    jd87iaho99["Error"] --> iloobtovwh(("EVAL"))
    7vz1yqkdqo(("Evaluator")) --> gntsn38l9s["CIAM - Magic Link Authentication"]
    bdjeulfdki(("EVAL")) --> r0hto2xun7["Present OTP Form"]
    9m5a2f4emp["Get User&#39;s Existing Devices"] --> nydopq0ve3(("EVAL"))
    dp43hy7h76["Get authMethod Value"] --> zep1ojf98g(("EVAL"))
    czzrbt1dsb["Magic Link Enabled"] --> 7vz1yqkdqo(("Evaluator"))
    ulsqznx6ut["Is Constraint Violation Error"] --> 3a77bpgwom(("EVAL"))
    ay2mm4z4xe(("EVAL")) --> fj8w62y4z3["Assert FIDO Device Authentication"]
    0sua91hqk7(("EVAL")) --> czzrbt1dsb["Magic Link Enabled"]
    sk7vd2o3r7(("EVAL")) --> 9m5a2f4emp["Get User&#39;s Existing Devices"]
    lylme68jbw(("EVAL")) --> fkkub10ukt["Node"]
    zep1ojf98g(("EVAL")) --> 9f0dokmcu9["Node"]
    10oaokas61["Start MFA Authentication"] --> 4l39ap532m(("Evaluator"))
    47qta86y95(("EVAL")) --> x0jx5r2pyd["Node"]
    frh74jp1jg["Only One Usable Device"] --> ydyrhm9fkz(("EVAL"))
    47qta86y95(("EVAL")) --> wphj1fy8ri["Node"]
    b01n00fwkm["Continue MFA With Only Device"] --> 47qta86y95(("EVAL"))
    7vz1yqkdqo(("Evaluator")) --> 2uhj1oobbe["Node"]
    4l39ap532m(("Evaluator")) --> icy7kw57ll["Authentication Prompt"]
    icy7kw57ll["Authentication Prompt"] --> v0t14r4lv2(("EVAL"))
    v0t14r4lv2(("EVAL")) --> frh74jp1jg["Only One Usable Device"]
    4l39ap532m(("Evaluator")) --> t4cuk82upd["Node"]
    icy7kw57ll["Authentication Prompt"] --> wj5284rjb8(("EVAL"))
    wj5284rjb8(("EVAL")) --> l7i5qjffz1["Node"]
    icy7kw57ll["Authentication Prompt"] --> vw8zbuzgod(("EVAL"))
    vw8zbuzgod(("EVAL")) --> j55n69o5i7["Node"]
    ydyrhm9fkz(("EVAL")) --> a58tdqlgfb["Node"]
    t04dles3gs(("EVAL")) --> zfsjjfa5h6["Present FIDO2 Form "]
    5v1i2f1az4(("EVAL")) --> 4vf8sqyl70["Node"]
    9pb86bg0qi(("EVAL")) --> wf0h6fo6h8["Split By User&#39;s Selection"]
    1qtib8s0uu["Select Authentication Device"] --> iagfrg0an6(("EVAL"))
    e717up82dy["Device Selected By The User"] --> 5v1i2f1az4(("EVAL"))
    bf9jlbogz1(("EVAL")) --> 2n3az4vori["User Has Active Devices"]
    iagfrg0an6(("EVAL")) --> wa07p8s7qm["Not Magic Link?"]
    bf9jlbogz1(("EVAL")) --> czzrbt1dsb["Magic Link Enabled"]
    2n3az4vori["User Has Active Devices"] --> 0sua91hqk7(("EVAL"))
    te0bcdks99["Magic Link Authentication"] --> qsu3efxcsp(("EVAL"))
    ydyrhm9fkz(("EVAL")) --> xsm25p5qf7["Magic Link Enabled"]
    xsm25p5qf7["Magic Link Enabled"] --> ayodtok1lb(("EVAL"))
    ayodtok1lb(("EVAL")) --> x9k0uusly8["Node"]
    ayodtok1lb(("EVAL")) --> b01n00fwkm["Continue MFA With Only Device"]
    9zctbmveoc["Enrich Device Details"] --> 1cbcpbc5no(("EVAL"))
    l5z3ngnhjv(("EVAL")) --> qurffyxc2d["Split by user selection "]
    se271xaurx(("EVAL")) --> wzzac3ucto["Create Masked Devices"]
    sk3dza5671(("EVAL")) --> di86a7q7j0["Node"]
    e3httj56zd(("EVAL")) --> 5231692i67["Return to calling node."]
    qxdd8mlll5(("EVAL")) --> u9ab712lfx["Invoke PingOne Protect subflow"]
    u9ab712lfx["Invoke PingOne Protect subflow"] --> vexxoicu6a(("Evaluator"))
    vexxoicu6a(("Evaluator")) --> 3s5kidc2wc["Get Values from PingOne Protect analysis"]
    vexxoicu6a(("Evaluator")) --> j6salon8z4["Get Values from PingOne Protect analysis"]
    3s5kidc2wc["Get Values from PingOne Protect analysis"] --> u22hch23vs(("EVAL"))
    nl0cxyid0x(("EVAL")) --> ndm5er34sv["Risk Score from PingOne Protect"]
    ndm5er34sv["Risk Score from PingOne Protect"] --> 4n12f0orqv(("EVAL"))
    4n12f0orqv(("EVAL")) --> d2uumx5mpk["Return to calling node"]
    ndm5er34sv["Risk Score from PingOne Protect"] --> n69ynlsgag(("EVAL"))
    7hwtzuxjwc["Disable user"] --> 99q38lg97t(("EVAL"))
    ndm5er34sv["Risk Score from PingOne Protect"] --> sk3dza5671(("EVAL"))
    kgxiu8h9i5(("EVAL")) --> 9w2fwmdjtp["PingOne Protect Risk ID is Empty/NULL"]
    qw4n733f3t(("EVAL")) --> sj6aezm25b["Node"]
    dxowhkk5n5["Check if Risk Policy ID is empty"] --> kgxiu8h9i5(("EVAL"))
    kgxiu8h9i5(("EVAL")) --> p3914imkz7["Update Risk Evaluation - FAILURE"]
    5uyrxkfgza(("EVAL")) --> wi6hu0ai62["Check if Risk Policy ID is empty"]
    wi6hu0ai62["Check if Risk Policy ID is empty"] --> 33jpsgsdxv(("EVAL"))
    33jpsgsdxv(("EVAL")) --> ilu6o9n2x7["Update Risk Evaluation - SUCCESS"]
    33jpsgsdxv(("EVAL")) --> 33kryo3flh["PingOne Protect Risk ID is Empty/NULL"]
    fd7o3icva4(("EVAL")) --> 9q9zj5ndao["Node"]

    click mtaqacdw1m "vscode://file/./nodes/mtaqacdw1m.md" _parent
    click 8jrbqcts2g "vscode://file/./nodes/8jrbqcts2g.md" _parent
    click hk00gx2f95 "vscode://file/./nodes/hk00gx2f95.md" _parent
    click onogvjusk6 "vscode://file/./nodes/onogvjusk6.md" _parent
    click qw4n733f3t "vscode://file/./nodes/qw4n733f3t.md" _parent
    click li0d8slgjx "vscode://file/./nodes/li0d8slgjx.md" _parent
    click 7jufzmg1rk "vscode://file/./nodes/7jufzmg1rk.md" _parent
    click qw4n733f3t "vscode://file/./nodes/qw4n733f3t.md" _parent
    click 8jrbqcts2g "vscode://file/./nodes/8jrbqcts2g.md" _parent
    click hk00gx2f95 "vscode://file/./nodes/hk00gx2f95.md" _parent
    click kho2rpwvb7 "vscode://file/./nodes/kho2rpwvb7.md" _parent
    click 7jufzmg1rk "vscode://file/./nodes/7jufzmg1rk.md" _parent
    click onogvjusk6 "vscode://file/./nodes/onogvjusk6.md" _parent
    click kho2rpwvb7 "vscode://file/./nodes/kho2rpwvb7.md" _parent
    click 78i0a08xfl "vscode://file/./nodes/78i0a08xfl.md" _parent
    click iz5nper189 "vscode://file/./nodes/iz5nper189.md" _parent
    click gsmghrxxoy "vscode://file/./nodes/gsmghrxxoy.md" _parent
    click nl0cxyid0x "vscode://file/./nodes/nl0cxyid0x.md" _parent
    click 99q38lg97t "vscode://file/./nodes/99q38lg97t.md" _parent
    click sqdggkol0g "vscode://file/./nodes/sqdggkol0g.md" _parent
    click iloobtovwh "vscode://file/./nodes/iloobtovwh.md" _parent
    click dxowhkk5n5 "vscode://file/./nodes/dxowhkk5n5.md" _parent
    click iz5nper189 "vscode://file/./nodes/iz5nper189.md" _parent
    click 7hwtzuxjwc "vscode://file/./nodes/7hwtzuxjwc.md" _parent
    click n69ynlsgag "vscode://file/./nodes/n69ynlsgag.md" _parent
    click nf4hv96sui "vscode://file/./nodes/nf4hv96sui.md" _parent
    click cb4rka2li0 "vscode://file/./nodes/cb4rka2li0.md" _parent
    click 78i0a08xfl "vscode://file/./nodes/78i0a08xfl.md" _parent
    click x8ainlbr6x "vscode://file/./nodes/x8ainlbr6x.md" _parent
    click ndm5er34sv "vscode://file/./nodes/ndm5er34sv.md" _parent
    click j6salon8z4 "vscode://file/./nodes/j6salon8z4.md" _parent
    click cb4rka2li0 "vscode://file/./nodes/cb4rka2li0.md" _parent
    click ahjplbui3q "vscode://file/./nodes/ahjplbui3q.md" _parent
    click x8ainlbr6x "vscode://file/./nodes/x8ainlbr6x.md" _parent
    click pt24r4nafa "vscode://file/./nodes/pt24r4nafa.md" _parent
    click 3y03qc0kxe "vscode://file/./nodes/3y03qc0kxe.md" _parent
    click mtaqacdw1m "vscode://file/./nodes/mtaqacdw1m.md" _parent
    click 5231692i67 "vscode://file/./nodes/5231692i67.md" _parent
    click 4oyc5l9npk "vscode://file/./nodes/4oyc5l9npk.md" _parent
    click 737gi6ip3e "vscode://file/./nodes/737gi6ip3e.md" _parent
    click u22hch23vs "vscode://file/./nodes/u22hch23vs.md" _parent
    click gsmghrxxoy "vscode://file/./nodes/gsmghrxxoy.md" _parent
    click zfpuewwuhl "vscode://file/./nodes/zfpuewwuhl.md" _parent
    click pt24r4nafa "vscode://file/./nodes/pt24r4nafa.md" _parent
    click 3y03qc0kxe "vscode://file/./nodes/3y03qc0kxe.md" _parent
    click qxdd8mlll5 "vscode://file/./nodes/qxdd8mlll5.md" _parent
    click nl0cxyid0x "vscode://file/./nodes/nl0cxyid0x.md" _parent
    click ahjplbui3q "vscode://file/./nodes/ahjplbui3q.md" _parent
    click li0d8slgjx "vscode://file/./nodes/li0d8slgjx.md" _parent
    click e3httj56zd "vscode://file/./nodes/e3httj56zd.md" _parent
    click 737gi6ip3e "vscode://file/./nodes/737gi6ip3e.md" _parent
    click 9vk797lpxx "vscode://file/./nodes/9vk797lpxx.md" _parent
    click nf4hv96sui "vscode://file/./nodes/nf4hv96sui.md" _parent
    click mtaqacdw1m "vscode://file/./nodes/mtaqacdw1m.md" _parent
    click 1cbcpbc5no "vscode://file/./nodes/1cbcpbc5no.md" _parent
    click 4psx471uwp "vscode://file/./nodes/4psx471uwp.md" _parent
    click h8dtvwld36 "vscode://file/./nodes/h8dtvwld36.md" _parent
    click 76reddil11 "vscode://file/./nodes/76reddil11.md" _parent
    click r0hto2xun7 "vscode://file/./nodes/r0hto2xun7.md" _parent
    click l5z3ngnhjv "vscode://file/./nodes/l5z3ngnhjv.md" _parent
    click 1gtc5d0awz "vscode://file/./nodes/1gtc5d0awz.md" _parent
    click kok73n8hkt "vscode://file/./nodes/kok73n8hkt.md" _parent
    click 4psx471uwp "vscode://file/./nodes/4psx471uwp.md" _parent
    click 1gtc5d0awz "vscode://file/./nodes/1gtc5d0awz.md" _parent
    click qurffyxc2d "vscode://file/./nodes/qurffyxc2d.md" _parent
    click gsw5wwtm7t "vscode://file/./nodes/gsw5wwtm7t.md" _parent
    click en7y953x31 "vscode://file/./nodes/en7y953x31.md" _parent
    click 0w6twuixxq "vscode://file/./nodes/0w6twuixxq.md" _parent
    click fzjj3nuh7m "vscode://file/./nodes/fzjj3nuh7m.md" _parent
    click dxsjn36392 "vscode://file/./nodes/dxsjn36392.md" _parent
    click mt9kvt7hnn "vscode://file/./nodes/mt9kvt7hnn.md" _parent
    click fgc8woctfo "vscode://file/./nodes/fgc8woctfo.md" _parent
    click qurffyxc2d "vscode://file/./nodes/qurffyxc2d.md" _parent
    click 00j11fkhbx "vscode://file/./nodes/00j11fkhbx.md" _parent
    click fzjj3nuh7m "vscode://file/./nodes/fzjj3nuh7m.md" _parent
    click uz6hhdt9gv "vscode://file/./nodes/uz6hhdt9gv.md" _parent
    click zxfluj3oxa "vscode://file/./nodes/zxfluj3oxa.md" _parent
    click b0csz8cgnl "vscode://file/./nodes/b0csz8cgnl.md" _parent
    click qurffyxc2d "vscode://file/./nodes/qurffyxc2d.md" _parent
    click ig2ndq8bf2 "vscode://file/./nodes/ig2ndq8bf2.md" _parent
    click 00j11fkhbx "vscode://file/./nodes/00j11fkhbx.md" _parent
    click beakf43h8t "vscode://file/./nodes/beakf43h8t.md" _parent
    click gsw5wwtm7t "vscode://file/./nodes/gsw5wwtm7t.md" _parent
    click r6lnkuy0yh "vscode://file/./nodes/r6lnkuy0yh.md" _parent
    click ig2ndq8bf2 "vscode://file/./nodes/ig2ndq8bf2.md" _parent
    click m1e0cw0ygl "vscode://file/./nodes/m1e0cw0ygl.md" _parent
    click m1e0cw0ygl "vscode://file/./nodes/m1e0cw0ygl.md" _parent
    click fzjj3nuh7m "vscode://file/./nodes/fzjj3nuh7m.md" _parent
    click r6lnkuy0yh "vscode://file/./nodes/r6lnkuy0yh.md" _parent
    click mt9kvt7hnn "vscode://file/./nodes/mt9kvt7hnn.md" _parent
    click hdc8oa72ci "vscode://file/./nodes/hdc8oa72ci.md" _parent
    click 8h5tjkrug9 "vscode://file/./nodes/8h5tjkrug9.md" _parent
    click v97rmwpban "vscode://file/./nodes/v97rmwpban.md" _parent
    click 5pixttpidw "vscode://file/./nodes/5pixttpidw.md" _parent
    click gntsn38l9s "vscode://file/./nodes/gntsn38l9s.md" _parent
    click 51zazld6jz "vscode://file/./nodes/51zazld6jz.md" _parent
    click 5uyrxkfgza "vscode://file/./nodes/5uyrxkfgza.md" _parent
    click tidk1pmqix "vscode://file/./nodes/tidk1pmqix.md" _parent
    click 8h5tjkrug9 "vscode://file/./nodes/8h5tjkrug9.md" _parent
    click mmojm56jlj "vscode://file/./nodes/mmojm56jlj.md" _parent
    click uoyh9kzwil "vscode://file/./nodes/uoyh9kzwil.md" _parent
    click bhgtvbjvu1 "vscode://file/./nodes/bhgtvbjvu1.md" _parent
    click se271xaurx "vscode://file/./nodes/se271xaurx.md" _parent
    click uwfrx6s60u "vscode://file/./nodes/uwfrx6s60u.md" _parent
    click vr1msssq3l "vscode://file/./nodes/vr1msssq3l.md" _parent
    click wpbqyomp7z "vscode://file/./nodes/wpbqyomp7z.md" _parent
    click wa07p8s7qm "vscode://file/./nodes/wa07p8s7qm.md" _parent
    click vr1msssq3l "vscode://file/./nodes/vr1msssq3l.md" _parent
    click vul5k2q2dw "vscode://file/./nodes/vul5k2q2dw.md" _parent
    click te0bcdks99 "vscode://file/./nodes/te0bcdks99.md" _parent
    click wa07p8s7qm "vscode://file/./nodes/wa07p8s7qm.md" _parent
    click vul5k2q2dw "vscode://file/./nodes/vul5k2q2dw.md" _parent
    click imhudhsy1w "vscode://file/./nodes/imhudhsy1w.md" _parent
    click e717up82dy "vscode://file/./nodes/e717up82dy.md" _parent
    click wa07p8s7qm "vscode://file/./nodes/wa07p8s7qm.md" _parent
    click imhudhsy1w "vscode://file/./nodes/imhudhsy1w.md" _parent
    click j8lmuiytzs "vscode://file/./nodes/j8lmuiytzs.md" _parent
    click bf9jlbogz1 "vscode://file/./nodes/bf9jlbogz1.md" _parent
    click bhgtvbjvu1 "vscode://file/./nodes/bhgtvbjvu1.md" _parent
    click 1qtib8s0uu "vscode://file/./nodes/1qtib8s0uu.md" _parent
    click 0sua91hqk7 "vscode://file/./nodes/0sua91hqk7.md" _parent
    click 10oaokas61 "vscode://file/./nodes/10oaokas61.md" _parent
    click 845xzgf4bk "vscode://file/./nodes/845xzgf4bk.md" _parent
    click ulsqznx6ut "vscode://file/./nodes/ulsqznx6ut.md" _parent
    click 51zazld6jz "vscode://file/./nodes/51zazld6jz.md" _parent
    click 5gs9h0ar04 "vscode://file/./nodes/5gs9h0ar04.md" _parent
    click 3a77bpgwom "vscode://file/./nodes/3a77bpgwom.md" _parent
    click y7f8x8dkw2 "vscode://file/./nodes/y7f8x8dkw2.md" _parent
    click zfsjjfa5h6 "vscode://file/./nodes/zfsjjfa5h6.md" _parent
    click 9pb86bg0qi "vscode://file/./nodes/9pb86bg0qi.md" _parent
    click wf0h6fo6h8 "vscode://file/./nodes/wf0h6fo6h8.md" _parent
    click ay2mm4z4xe "vscode://file/./nodes/ay2mm4z4xe.md" _parent
    click ulsqznx6ut "vscode://file/./nodes/ulsqznx6ut.md" _parent
    click fu06ckn12l "vscode://file/./nodes/fu06ckn12l.md" _parent
    click fj8w62y4z3 "vscode://file/./nodes/fj8w62y4z3.md" _parent
    click 845xzgf4bk "vscode://file/./nodes/845xzgf4bk.md" _parent
    click fu06ckn12l "vscode://file/./nodes/fu06ckn12l.md" _parent
    click y8pxpynfle "vscode://file/./nodes/y8pxpynfle.md" _parent
    click 7vrrd3uuhm "vscode://file/./nodes/7vrrd3uuhm.md" _parent
    click en7y953x31 "vscode://file/./nodes/en7y953x31.md" _parent
    click 1lam7h7jbc "vscode://file/./nodes/1lam7h7jbc.md" _parent
    click 9fzm9oj8fd "vscode://file/./nodes/9fzm9oj8fd.md" _parent
    click qsu3efxcsp "vscode://file/./nodes/qsu3efxcsp.md" _parent
    click 1lam7h7jbc "vscode://file/./nodes/1lam7h7jbc.md" _parent
    click 6yu5p2iz3r "vscode://file/./nodes/6yu5p2iz3r.md" _parent
    click ms19ql02hi "vscode://file/./nodes/ms19ql02hi.md" _parent
    click en7y953x31 "vscode://file/./nodes/en7y953x31.md" _parent
    click 0w6twuixxq "vscode://file/./nodes/0w6twuixxq.md" _parent
    click t6p5s6t603 "vscode://file/./nodes/t6p5s6t603.md" _parent
    click 4oyc5l9npk "vscode://file/./nodes/4oyc5l9npk.md" _parent
    click 10uwd1ccc4 "vscode://file/./nodes/10uwd1ccc4.md" _parent
    click se271xaurx "vscode://file/./nodes/se271xaurx.md" _parent
    click wzzac3ucto "vscode://file/./nodes/wzzac3ucto.md" _parent
    click 6yu5p2iz3r "vscode://file/./nodes/6yu5p2iz3r.md" _parent
    click fd7o3icva4 "vscode://file/./nodes/fd7o3icva4.md" _parent
    click j8lmuiytzs "vscode://file/./nodes/j8lmuiytzs.md" _parent
    click ms19ql02hi "vscode://file/./nodes/ms19ql02hi.md" _parent
    click fd7o3icva4 "vscode://file/./nodes/fd7o3icva4.md" _parent
    click 3nn0mw8jkt "vscode://file/./nodes/3nn0mw8jkt.md" _parent
    click 61c9e2dt59 "vscode://file/./nodes/61c9e2dt59.md" _parent
    click 51zazld6jz "vscode://file/./nodes/51zazld6jz.md" _parent
    click nvxwg0vum3 "vscode://file/./nodes/nvxwg0vum3.md" _parent
    click 9fzm9oj8fd "vscode://file/./nodes/9fzm9oj8fd.md" _parent
    click lgn9kliiqj "vscode://file/./nodes/lgn9kliiqj.md" _parent
    click b0csz8cgnl "vscode://file/./nodes/b0csz8cgnl.md" _parent
    click fq7l0s8w2s "vscode://file/./nodes/fq7l0s8w2s.md" _parent
    click 1lam7h7jbc "vscode://file/./nodes/1lam7h7jbc.md" _parent
    click lylme68jbw "vscode://file/./nodes/lylme68jbw.md" _parent
    click 0w6twuixxq "vscode://file/./nodes/0w6twuixxq.md" _parent
    click 5sb0db3vb0 "vscode://file/./nodes/5sb0db3vb0.md" _parent
    click 7vpjww2ek2 "vscode://file/./nodes/7vpjww2ek2.md" _parent
    click t04dles3gs "vscode://file/./nodes/t04dles3gs.md" _parent
    click 9vk797lpxx "vscode://file/./nodes/9vk797lpxx.md" _parent
    click 10uwd1ccc4 "vscode://file/./nodes/10uwd1ccc4.md" _parent
    click wf0h6fo6h8 "vscode://file/./nodes/wf0h6fo6h8.md" _parent
    click 3nn0mw8jkt "vscode://file/./nodes/3nn0mw8jkt.md" _parent
    click k46n95w9eo "vscode://file/./nodes/k46n95w9eo.md" _parent
    click 5uyrxkfgza "vscode://file/./nodes/5uyrxkfgza.md" _parent
    click hdc8oa72ci "vscode://file/./nodes/hdc8oa72ci.md" _parent
    click v97rmwpban "vscode://file/./nodes/v97rmwpban.md" _parent
    click 7vrrd3uuhm "vscode://file/./nodes/7vrrd3uuhm.md" _parent
    click hdc8oa72ci "vscode://file/./nodes/hdc8oa72ci.md" _parent
    click fgc8woctfo "vscode://file/./nodes/fgc8woctfo.md" _parent
    click 7vrrd3uuhm "vscode://file/./nodes/7vrrd3uuhm.md" _parent
    click zbhvblc83s "vscode://file/./nodes/zbhvblc83s.md" _parent
    click ybwxgols9w "vscode://file/./nodes/ybwxgols9w.md" _parent
    click 4psx471uwp "vscode://file/./nodes/4psx471uwp.md" _parent
    click h8dtvwld36 "vscode://file/./nodes/h8dtvwld36.md" _parent
    click ybwxgols9w "vscode://file/./nodes/ybwxgols9w.md" _parent
    click 9zctbmveoc "vscode://file/./nodes/9zctbmveoc.md" _parent
    click iloobtovwh "vscode://file/./nodes/iloobtovwh.md" _parent
    click dwhgyxkavz "vscode://file/./nodes/dwhgyxkavz.md" _parent
    click qsu3efxcsp "vscode://file/./nodes/qsu3efxcsp.md" _parent
    click muund54c7j "vscode://file/./nodes/muund54c7j.md" _parent
    click 6p4frzqpp1 "vscode://file/./nodes/6p4frzqpp1.md" _parent
    click sk7vd2o3r7 "vscode://file/./nodes/sk7vd2o3r7.md" _parent
    click 845xzgf4bk "vscode://file/./nodes/845xzgf4bk.md" _parent
    click dp43hy7h76 "vscode://file/./nodes/dp43hy7h76.md" _parent
    click 5v1i2f1az4 "vscode://file/./nodes/5v1i2f1az4.md" _parent
    click cbapcifpyy "vscode://file/./nodes/cbapcifpyy.md" _parent
    click nydopq0ve3 "vscode://file/./nodes/nydopq0ve3.md" _parent
    click qzuk2c4cdb "vscode://file/./nodes/qzuk2c4cdb.md" _parent
    click nydopq0ve3 "vscode://file/./nodes/nydopq0ve3.md" _parent
    click t6p5s6t603 "vscode://file/./nodes/t6p5s6t603.md" _parent
    click fq7l0s8w2s "vscode://file/./nodes/fq7l0s8w2s.md" _parent
    click bdjeulfdki "vscode://file/./nodes/bdjeulfdki.md" _parent
    click jd87iaho99 "vscode://file/./nodes/jd87iaho99.md" _parent
    click iloobtovwh "vscode://file/./nodes/iloobtovwh.md" _parent
    click 7vz1yqkdqo "vscode://file/./nodes/7vz1yqkdqo.md" _parent
    click gntsn38l9s "vscode://file/./nodes/gntsn38l9s.md" _parent
    click bdjeulfdki "vscode://file/./nodes/bdjeulfdki.md" _parent
    click r0hto2xun7 "vscode://file/./nodes/r0hto2xun7.md" _parent
    click 9m5a2f4emp "vscode://file/./nodes/9m5a2f4emp.md" _parent
    click nydopq0ve3 "vscode://file/./nodes/nydopq0ve3.md" _parent
    click dp43hy7h76 "vscode://file/./nodes/dp43hy7h76.md" _parent
    click zep1ojf98g "vscode://file/./nodes/zep1ojf98g.md" _parent
    click czzrbt1dsb "vscode://file/./nodes/czzrbt1dsb.md" _parent
    click 7vz1yqkdqo "vscode://file/./nodes/7vz1yqkdqo.md" _parent
    click ulsqznx6ut "vscode://file/./nodes/ulsqznx6ut.md" _parent
    click 3a77bpgwom "vscode://file/./nodes/3a77bpgwom.md" _parent
    click ay2mm4z4xe "vscode://file/./nodes/ay2mm4z4xe.md" _parent
    click fj8w62y4z3 "vscode://file/./nodes/fj8w62y4z3.md" _parent
    click 0sua91hqk7 "vscode://file/./nodes/0sua91hqk7.md" _parent
    click czzrbt1dsb "vscode://file/./nodes/czzrbt1dsb.md" _parent
    click sk7vd2o3r7 "vscode://file/./nodes/sk7vd2o3r7.md" _parent
    click 9m5a2f4emp "vscode://file/./nodes/9m5a2f4emp.md" _parent
    click lylme68jbw "vscode://file/./nodes/lylme68jbw.md" _parent
    click fkkub10ukt "vscode://file/./nodes/fkkub10ukt.md" _parent
    click zep1ojf98g "vscode://file/./nodes/zep1ojf98g.md" _parent
    click 9f0dokmcu9 "vscode://file/./nodes/9f0dokmcu9.md" _parent
    click 10oaokas61 "vscode://file/./nodes/10oaokas61.md" _parent
    click 4l39ap532m "vscode://file/./nodes/4l39ap532m.md" _parent
    click 47qta86y95 "vscode://file/./nodes/47qta86y95.md" _parent
    click x0jx5r2pyd "vscode://file/./nodes/x0jx5r2pyd.md" _parent
    click frh74jp1jg "vscode://file/./nodes/frh74jp1jg.md" _parent
    click ydyrhm9fkz "vscode://file/./nodes/ydyrhm9fkz.md" _parent
    click 47qta86y95 "vscode://file/./nodes/47qta86y95.md" _parent
    click wphj1fy8ri "vscode://file/./nodes/wphj1fy8ri.md" _parent
    click b01n00fwkm "vscode://file/./nodes/b01n00fwkm.md" _parent
    click 47qta86y95 "vscode://file/./nodes/47qta86y95.md" _parent
    click 7vz1yqkdqo "vscode://file/./nodes/7vz1yqkdqo.md" _parent
    click 2uhj1oobbe "vscode://file/./nodes/2uhj1oobbe.md" _parent
    click 4l39ap532m "vscode://file/./nodes/4l39ap532m.md" _parent
    click icy7kw57ll "vscode://file/./nodes/icy7kw57ll.md" _parent
    click icy7kw57ll "vscode://file/./nodes/icy7kw57ll.md" _parent
    click v0t14r4lv2 "vscode://file/./nodes/v0t14r4lv2.md" _parent
    click v0t14r4lv2 "vscode://file/./nodes/v0t14r4lv2.md" _parent
    click frh74jp1jg "vscode://file/./nodes/frh74jp1jg.md" _parent
    click 4l39ap532m "vscode://file/./nodes/4l39ap532m.md" _parent
    click t4cuk82upd "vscode://file/./nodes/t4cuk82upd.md" _parent
    click icy7kw57ll "vscode://file/./nodes/icy7kw57ll.md" _parent
    click wj5284rjb8 "vscode://file/./nodes/wj5284rjb8.md" _parent
    click wj5284rjb8 "vscode://file/./nodes/wj5284rjb8.md" _parent
    click l7i5qjffz1 "vscode://file/./nodes/l7i5qjffz1.md" _parent
    click icy7kw57ll "vscode://file/./nodes/icy7kw57ll.md" _parent
    click vw8zbuzgod "vscode://file/./nodes/vw8zbuzgod.md" _parent
    click vw8zbuzgod "vscode://file/./nodes/vw8zbuzgod.md" _parent
    click j55n69o5i7 "vscode://file/./nodes/j55n69o5i7.md" _parent
    click ydyrhm9fkz "vscode://file/./nodes/ydyrhm9fkz.md" _parent
    click a58tdqlgfb "vscode://file/./nodes/a58tdqlgfb.md" _parent
    click t04dles3gs "vscode://file/./nodes/t04dles3gs.md" _parent
    click zfsjjfa5h6 "vscode://file/./nodes/zfsjjfa5h6.md" _parent
    click 5v1i2f1az4 "vscode://file/./nodes/5v1i2f1az4.md" _parent
    click 4vf8sqyl70 "vscode://file/./nodes/4vf8sqyl70.md" _parent
    click 9pb86bg0qi "vscode://file/./nodes/9pb86bg0qi.md" _parent
    click wf0h6fo6h8 "vscode://file/./nodes/wf0h6fo6h8.md" _parent
    click 1qtib8s0uu "vscode://file/./nodes/1qtib8s0uu.md" _parent
    click iagfrg0an6 "vscode://file/./nodes/iagfrg0an6.md" _parent
    click e717up82dy "vscode://file/./nodes/e717up82dy.md" _parent
    click 5v1i2f1az4 "vscode://file/./nodes/5v1i2f1az4.md" _parent
    click bf9jlbogz1 "vscode://file/./nodes/bf9jlbogz1.md" _parent
    click 2n3az4vori "vscode://file/./nodes/2n3az4vori.md" _parent
    click iagfrg0an6 "vscode://file/./nodes/iagfrg0an6.md" _parent
    click wa07p8s7qm "vscode://file/./nodes/wa07p8s7qm.md" _parent
    click bf9jlbogz1 "vscode://file/./nodes/bf9jlbogz1.md" _parent
    click czzrbt1dsb "vscode://file/./nodes/czzrbt1dsb.md" _parent
    click 2n3az4vori "vscode://file/./nodes/2n3az4vori.md" _parent
    click 0sua91hqk7 "vscode://file/./nodes/0sua91hqk7.md" _parent
    click te0bcdks99 "vscode://file/./nodes/te0bcdks99.md" _parent
    click qsu3efxcsp "vscode://file/./nodes/qsu3efxcsp.md" _parent
    click ydyrhm9fkz "vscode://file/./nodes/ydyrhm9fkz.md" _parent
    click xsm25p5qf7 "vscode://file/./nodes/xsm25p5qf7.md" _parent
    click xsm25p5qf7 "vscode://file/./nodes/xsm25p5qf7.md" _parent
    click ayodtok1lb "vscode://file/./nodes/ayodtok1lb.md" _parent
    click ayodtok1lb "vscode://file/./nodes/ayodtok1lb.md" _parent
    click x9k0uusly8 "vscode://file/./nodes/x9k0uusly8.md" _parent
    click ayodtok1lb "vscode://file/./nodes/ayodtok1lb.md" _parent
    click b01n00fwkm "vscode://file/./nodes/b01n00fwkm.md" _parent
    click 9zctbmveoc "vscode://file/./nodes/9zctbmveoc.md" _parent
    click 1cbcpbc5no "vscode://file/./nodes/1cbcpbc5no.md" _parent
    click l5z3ngnhjv "vscode://file/./nodes/l5z3ngnhjv.md" _parent
    click qurffyxc2d "vscode://file/./nodes/qurffyxc2d.md" _parent
    click se271xaurx "vscode://file/./nodes/se271xaurx.md" _parent
    click wzzac3ucto "vscode://file/./nodes/wzzac3ucto.md" _parent
    click sk3dza5671 "vscode://file/./nodes/sk3dza5671.md" _parent
    click di86a7q7j0 "vscode://file/./nodes/di86a7q7j0.md" _parent
    click e3httj56zd "vscode://file/./nodes/e3httj56zd.md" _parent
    click 5231692i67 "vscode://file/./nodes/5231692i67.md" _parent
    click qxdd8mlll5 "vscode://file/./nodes/qxdd8mlll5.md" _parent
    click u9ab712lfx "vscode://file/./nodes/u9ab712lfx.md" _parent
    click u9ab712lfx "vscode://file/./nodes/u9ab712lfx.md" _parent
    click vexxoicu6a "vscode://file/./nodes/vexxoicu6a.md" _parent
    click vexxoicu6a "vscode://file/./nodes/vexxoicu6a.md" _parent
    click 3s5kidc2wc "vscode://file/./nodes/3s5kidc2wc.md" _parent
    click vexxoicu6a "vscode://file/./nodes/vexxoicu6a.md" _parent
    click j6salon8z4 "vscode://file/./nodes/j6salon8z4.md" _parent
    click 3s5kidc2wc "vscode://file/./nodes/3s5kidc2wc.md" _parent
    click u22hch23vs "vscode://file/./nodes/u22hch23vs.md" _parent
    click nl0cxyid0x "vscode://file/./nodes/nl0cxyid0x.md" _parent
    click ndm5er34sv "vscode://file/./nodes/ndm5er34sv.md" _parent
    click ndm5er34sv "vscode://file/./nodes/ndm5er34sv.md" _parent
    click 4n12f0orqv "vscode://file/./nodes/4n12f0orqv.md" _parent
    click 4n12f0orqv "vscode://file/./nodes/4n12f0orqv.md" _parent
    click d2uumx5mpk "vscode://file/./nodes/d2uumx5mpk.md" _parent
    click ndm5er34sv "vscode://file/./nodes/ndm5er34sv.md" _parent
    click n69ynlsgag "vscode://file/./nodes/n69ynlsgag.md" _parent
    click 7hwtzuxjwc "vscode://file/./nodes/7hwtzuxjwc.md" _parent
    click 99q38lg97t "vscode://file/./nodes/99q38lg97t.md" _parent
    click ndm5er34sv "vscode://file/./nodes/ndm5er34sv.md" _parent
    click sk3dza5671 "vscode://file/./nodes/sk3dza5671.md" _parent
    click kgxiu8h9i5 "vscode://file/./nodes/kgxiu8h9i5.md" _parent
    click 9w2fwmdjtp "vscode://file/./nodes/9w2fwmdjtp.md" _parent
    click qw4n733f3t "vscode://file/./nodes/qw4n733f3t.md" _parent
    click sj6aezm25b "vscode://file/./nodes/sj6aezm25b.md" _parent
    click dxowhkk5n5 "vscode://file/./nodes/dxowhkk5n5.md" _parent
    click kgxiu8h9i5 "vscode://file/./nodes/kgxiu8h9i5.md" _parent
    click kgxiu8h9i5 "vscode://file/./nodes/kgxiu8h9i5.md" _parent
    click p3914imkz7 "vscode://file/./nodes/p3914imkz7.md" _parent
    click 5uyrxkfgza "vscode://file/./nodes/5uyrxkfgza.md" _parent
    click wi6hu0ai62 "vscode://file/./nodes/wi6hu0ai62.md" _parent
    click wi6hu0ai62 "vscode://file/./nodes/wi6hu0ai62.md" _parent
    click 33jpsgsdxv "vscode://file/./nodes/33jpsgsdxv.md" _parent
    click 33jpsgsdxv "vscode://file/./nodes/33jpsgsdxv.md" _parent
    click ilu6o9n2x7 "vscode://file/./nodes/ilu6o9n2x7.md" _parent
    click 33jpsgsdxv "vscode://file/./nodes/33jpsgsdxv.md" _parent
    click 33kryo3flh "vscode://file/./nodes/33kryo3flh.md" _parent
    click fd7o3icva4 "vscode://file/./nodes/fd7o3icva4.md" _parent
    click 9q9zj5ndao "vscode://file/./nodes/9q9zj5ndao.md" _parent
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
