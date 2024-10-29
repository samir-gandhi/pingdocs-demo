# CIAM-Passwordless-Protect-Registration-Authentication-Account-Recovery-Main Flow

### Flow Diagram
```mermaid
flowchart LR
    i21ma1l9mn(("EVAL")) --> muyh5iinqk["Node"]
    mkz8u9xtjp(("EVAL")) --> dv7x4k323t["Password Sign On Page"]
    0cmw42tqse(("EVAL")) --> bcrh9zpo2j["Read all MFA devices"]
    hun8tkpynt["Check if Risk ID is Empty"] --> 7186msgx2b(("Evaluator"))
    1gv745vu9f(("EVAL")) --> 5tz0a2yt0y["Check if MFA Size is 0"]
    7186msgx2b(("Evaluator")) --> fqw47ezfd4["Update risk evaluation with SUCCESS"]
    0cdm5xwnl3["Check if Risk ID is Empty"] --> oep2ke136(("Evaluator"))
    sdz87dk9h3(("EVAL")) --> hun8tkpynt["Check if Risk ID is Empty"]
    2ixdpv74ih(("EVAL")) --> 0cdm5xwnl3["Check if Risk ID is Empty"]
    ybma422b3i(("EVAL")) --> 3dpidmgj6g["Node"]
    8a3rp16jhq["Find user and error out if user not found"] --> ybma422b3i(("EVAL"))
    eq6oq9q1ag["Find user in PingOne"] --> 71uz2oxfw9(("Evaluator"))
    5gz6jcxdng(("Evaluator")) --> ptslfr1den["Check if user can authenticate"]
    rmx6s73ihv["Passwordless Sign On Page"] --> 59qszmzgg5(("EVAL"))
    71uz2oxfw9(("Evaluator")) --> r7ddjgug4y["Check if user is enabled."]
    ph08u6bgi1(("Evaluator")) --> hcdhp9ww20["Proceed with this user"]
    dv7x4k323t["Password Sign On Page"] --> gersdqsi8h(("Evaluator"))
    ptslfr1den["Check if user can authenticate"] --> dfcr1art1l(("Evaluator"))
    dfcr1art1l(("Evaluator")) --> j23r4buol6["Error message for user authentication."]
    4rjs3llu20["Set Industry Variables"] --> 340awenest(("EVAL"))
    sdz87dk9h3(("EVAL")) --> 5770fvct63["Check Flow Method"]
    2ixdpv74ih(("EVAL")) --> m8unn93k58["Error Message Screen"]
    m8unn93k58["Error Message Screen"] --> bkuqv7wdoo(("EVAL"))
    gm6xl62pf3["Check Flow Method"] --> yjz1weh9xh(("EVAL"))
    cl9ugbu07r["Return Error"] --> 2ixdpv74ih(("EVAL"))
    jv8lvv5w4x(("EVAL")) --> jimu9wsyls["Find User"]
    5770fvct63["Check Flow Method"] --> eum65le218(("EVAL"))
    asnrb9403q["Keep authMethods As Is"] --> njmld8889h(("EVAL"))
    qdea3v0byw(("EVAL")) --> oca826nc0b["Send Response"]
    yjz1weh9xh(("EVAL")) --> yr9tytff7["Redirect With Error Response"]
    j7vnuet5bk["Set Flow Constants"] --> 3lgnmx50te(("EVAL"))
    bkuqv7wdoo(("EVAL")) --> gm6xl62pf3["Check Flow Method"]
    cppsibbyhy["Password Sign On Page Button Pressed"] --> 8epxzybfo(("EVAL"))
    jimu9wsyls["Find User"] --> jio5trsqxr(("EVAL"))
    eum65le218(("EVAL")) --> zlublpnvlp["Redirect With Success Response"]
    5770fvct63["Check Flow Method"] --> jv8lvv5w4x(("EVAL"))
    jio5trsqxr(("EVAL")) --> 0e7xqfqq2e["Return With Success Response"]
    wcask7tfhv(("EVAL")) --> z34hsrcd98["CIAM - Account Recovery "]
    m2zwktv18x(("EVAL")) --> drg4lvxpjw["Node"]
    ins74ygtvc["Check Session"] --> fqkfitsm9p(("EVAL"))
    fqkfitsm9p(("EVAL")) --> w16j6hvh6d["Check For Valid Session"]
    zkdpy8oqb5(("EVAL")) --> 5g1u9k5fi3["Is Remember Me Checked"]
    cppsibbyhy["Password Sign On Page Button Pressed"] --> n5vpbff54(("EVAL"))
    hp2eob8gy8(("Evaluator")) --> rtjwqkq5ng["Node"]
    aeek6nl8wj(("EVAL")) --> yt7rz448i7["Node"]
    85rxatuk44(("EVAL")) --> qc1wiq047b["NOP UI Page"]
    g1w1cltra3["CIAM - Account Registration "] --> hzmdf4b1w6(("Evaluator"))
    60dszexpy6(("Evaluator")) --> 6961q0o277["Split By Subflow&#39;s Result"]
    qc1wiq047b["NOP UI Page"] --> 83g36u9ohr(("EVAL"))
    83g36u9ohr(("EVAL")) --> sbudfzsp5m["Change Password"]
    sbudfzsp5m["Change Password"] --> ug3m1588jl(("Evaluator"))
    ug3m1588jl(("Evaluator")) --> y1g5lzp3md["Did Subflow Return Success"]
    8b7afymuxh(("EVAL")) --> wdhgxaxnfa["Node"]
    ug3m1588jl(("Evaluator")) --> synvhooann["Node"]
    8b7afymuxh(("EVAL")) --> se0w7zdrd7["Reset Password Success Message"]
    y1g5lzp3md["Did Subflow Return Success"] --> 8b7afymuxh(("EVAL"))
    cao68g3gyc(("EVAL")) --> e0fk3mmhht["Send Verification Code"]
    zkdpy8oqb5(("EVAL")) --> r60mrklkuw["Node"]
    n2c0bh5gsg(("EVAL")) --> c3x77vuo10["NOP UI Page"]
    ozb119ee81(("EVAL")) --> m8opeg6ilr["Verify Email"]
    hp2eob8gy8(("Evaluator")) --> e01o5o4i77["Has User Cancelled Auth"]
    c3x77vuo10["NOP UI Page"] --> 76t9hosyif(("EVAL"))
    pmzg2ixr1g(("EVAL")) --> 90yph4ra19["Node"]
    flmowbcu44(("EVAL")) --> aeev9gqagj["Node"]
    w9egwegsnj(("EVAL")) --> cqktdyqncg["Split By Subflow&#39;s Result"]
    gqbh7qw6qa(("EVAL")) --> 614hjulpdj["Node"]
    nb3y5kcx2q(("EVAL")) --> ze4pz75nx["Node"]
    b275pagysx["Is Account Locked?"] --> scxeegwacj(("EVAL"))
    c9kmm14iq0(("EVAL")) --> b275pagysx["Is Account Locked?"]
    yr66uwy0ma(("EVAL")) --> 0fezdflrz4["Go to Sign On Success"]
    76t9hosyif(("EVAL")) --> frkr1a0u82["Check Agreement"]
    scxeegwacj(("EVAL")) --> 8b6kcm9yz6["Password Check Failure Error"]
    hzmdf4b1w6(("Evaluator")) --> wxocgg04qz["Node"]
    1qqopmsxn1["Split By Subflow&#39;s Result"] --> tcx0nm2t9o(("EVAL"))
    1qqopmsxn1["Split By Subflow&#39;s Result"] --> so58xwowjn(("EVAL"))
    tcx0nm2t9o(("EVAL")) --> 096blcsiod["Node"]
    so58xwowjn(("EVAL")) --> qo3pwj5p12["Node"]
    qbf8b4sda4(("EVAL")) --> 7y41qu33vz["CIAM - Account Registration"]
    hzmdf4b1w6(("Evaluator")) --> 1qqopmsxn1["Split By Subflow&#39;s Result"]
    n5vpbff54(("EVAL")) --> h0rcajanl2["Node"]
    lbhyjujyjv(("Evaluator")) --> vztjuyevpz["Check If No Existing Session Token"]
    d5jso3qit5(("EVAL")) --> g1w1cltra3["CIAM - Account Registration "]
    cppsibbyhy["Password Sign On Page Button Pressed"] --> d5jso3qit5(("EVAL"))
    2nlbum4ywj["Delete Session"] --> m2zwktv18x(("EVAL"))
    m2zwktv18x(("EVAL")) --> hk1hymxs4y["Node"]
    qn65h94yqq(("EVAL")) --> hk1hymxs4y["Node"]
    vztjuyevpz["Check If No Existing Session Token"] --> qn65h94yqq(("EVAL"))
    qn65h94yqq(("EVAL")) --> 2nlbum4ywj["Delete Session"]
    zlublpnvlp["Redirect With Success Response"] --> o74snj74sy(("Evaluator"))
    3lgnmx50te(("EVAL")) --> byomx9u9ci["Set Flow Variables"]
    oiauhhhv4k["Split By Subflow&#39;s Result"] --> aw3ce1sq70(("EVAL"))
    21l7s55n2w(("EVAL")) --> oiauhhhv4k["Split By Subflow&#39;s Result"]
    aw3ce1sq70(("EVAL")) --> nhs3ybbdgg["Node"]
    60dszexpy6(("Evaluator")) --> xmdntu2a5o["Node"]
    3dpidmgj6g["Node"] --> 3e86t7q5xg(("EVAL"))
    ri35kah4nr(("EVAL")) --> as1tfleqv7["Node"]
    6961q0o277["Split By Subflow&#39;s Result"] --> vwq8svkesj(("EVAL"))
    6x0m1t11oh["Passwordless Sign On Page Button Pressed"] --> ri35kah4nr(("EVAL"))
    mkz8u9xtjp(("EVAL")) --> rmx6s73ihv["Passwordless Sign On Page"]
    rc315a9uh1(("EVAL")) --> 5b7wgayb4e["CIAM - Account Recovery "]
    oiauhhhv4k["Split By Subflow&#39;s Result"] --> o5vjpzh7bq(("EVAL"))
    o5vjpzh7bq(("EVAL")) --> bv4f2hdy6o["Node"]
    1nt8111fdv(("EVAL")) --> 2ernrgqxzb["Lookup User"]
    6x0m1t11oh["Passwordless Sign On Page Button Pressed"] --> qbf8b4sda4(("EVAL"))
    se0w7zdrd7["Reset Password Success Message"] --> liu3llworn(("EVAL"))
    59qszmzgg5(("EVAL")) --> 6x0m1t11oh["Passwordless Sign On Page Button Pressed"]
    oiy97ee3bv(("EVAL")) --> vlngo6a8gl["Node"]
    powvchr4kr["Reset Password"] --> 85rxatuk44(("EVAL"))
    r01x04oq1y(("Evaluator")) --> mmqiyn4q46["Verification Not Required"]
    liu3llworn(("EVAL")) --> gj8d9gmnwj["Go to Sign On Success"]
    e0fk3mmhht["Send Verification Code"] --> ozb119ee81(("EVAL"))
    mmqiyn4q46["Verification Not Required"] --> cao68g3gyc(("EVAL"))
    6x0m1t11oh["Passwordless Sign On Page Button Pressed"] --> 907z7uvt6v(("EVAL"))
    5gz6jcxdng(("Evaluator")) --> bt6lzhdb0v["Error Message for disabled user."]
    w9egwegsnj(("EVAL")) --> e1w127ll95["Node"]
    njmld8889h(("EVAL")) --> upanxjpo9i["Node"]
    infm8ry8j9(("EVAL")) --> upanxjpo9i["Node"]
    kpq6uykwvz["Add rememberMe To authMethods"] --> infm8ry8j9(("EVAL"))
    5g1u9k5fi3["Is Remember Me Checked"] --> rgae4w87f5(("Evaluator"))
    ph08u6bgi1(("Evaluator")) --> ou1gi7wq5d["Error message for Non Active user"]
    7y41qu33vz["CIAM - Account Registration"] --> 60dszexpy6(("Evaluator"))
    cqktdyqncg["Split By Subflow&#39;s Result"] --> pmzg2ixr1g(("EVAL"))
    4ncwrpsqgn["Check account status"] --> ph08u6bgi1(("Evaluator"))
    21l7s55n2w(("EVAL")) --> x5v48y5oma["Node"]
    cao68g3gyc(("EVAL")) --> 5g1u9k5fi3["Is Remember Me Checked"]
    rstodi2zw1["Password Authentication"] --> bilu0ighwr(("EVAL"))
    rqsigpn591(("EVAL")) --> xfg1fliupl["Node"]
    fm7p6z4lgt(("EVAL")) --> 4ncwrpsqgn["Check account status"]
    eht5fkf5yz["CIAM - Device Authentication"] --> hp2eob8gy8(("Evaluator"))
    o74snj74sy(("Evaluator")) --> wuyh51gb1x["Node"]
    c9kmm14iq0(("EVAL")) --> cstwt93s8m["Check Password Status"]
    y7f4468q9f(("EVAL")) --> zoqe5yn0jc["No User Found Error"]
    6x0m1t11oh["Passwordless Sign On Page Button Pressed"] --> wcask7tfhv(("EVAL"))
    bcrh9zpo2j["Read all MFA devices"] --> 1gv745vu9f(("EVAL"))
    8epxzybfo(("EVAL")) --> rmx6s73ihv["Passwordless Sign On Page"]
    6x0m1t11oh["Passwordless Sign On Page Button Pressed"] --> gqbh7qw6qa(("EVAL"))
    w16j6hvh6d["Check For Valid Session"] --> lbhyjujyjv(("Evaluator"))
    cppsibbyhy["Password Sign On Page Button Pressed"] --> rc315a9uh1(("EVAL"))
    m8opeg6ilr["Verify Email"] --> zkdpy8oqb5(("EVAL"))
    r01x04oq1y(("Evaluator")) --> shrf93ss72["Node"]
    imnmdfh12z(("EVAL")) --> ed4e0aipzr["Go to Reset Password"]
    vwq8svkesj(("EVAL")) --> 6p48mt9nzd["Node"]
    gersdqsi8h(("Evaluator")) --> cppsibbyhy["Password Sign On Page Button Pressed"]
    8fovn3syu3["Is Passwordless Required?"] --> mkz8u9xtjp(("EVAL"))
    cstwt93s8m["Check Password Status"] --> rqsigpn591(("EVAL"))
    6961q0o277["Split By Subflow&#39;s Result"] --> aeek6nl8wj(("EVAL"))
    f0p9tnng3j(("EVAL")) --> 8fovn3syu3["Is Passwordless Required?"]
    us1sbucx0m["Validate Password"] --> c9kmm14iq0(("EVAL"))
    scxeegwacj(("EVAL")) --> a5vlldmzi6["Node"]
    nbcsfwxqvp(("EVAL")) --> c8p1c19w99["Go to Reset Password"]
    cstwt93s8m["Check Password Status"] --> imnmdfh12z(("EVAL"))
    y7f4468q9f(("EVAL")) --> us1sbucx0m["Validate Password"]
    bilu0ighwr(("EVAL")) --> t09lk8opxa["User Lookup"]
    71uz2oxfw9(("Evaluator")) --> fdo3dhvrb8["Error Message for user not found."]
    nb3y5kcx2q(("EVAL")) --> whgnox29ew["Node"]
    frkr1a0u82["Check Agreement"] --> r01x04oq1y(("Evaluator"))
    rgae4w87f5(("Evaluator")) --> kpq6uykwvz["Add rememberMe To authMethods"]
    t09lk8opxa["User Lookup"] --> y7f4468q9f(("EVAL"))
    cqktdyqncg["Split By Subflow&#39;s Result"] --> flmowbcu44(("EVAL"))
    rgae4w87f5(("Evaluator")) --> asnrb9403q["Keep authMethods As Is"]
    gm6xl62pf3["Check Flow Method"] --> qdea3v0byw(("EVAL"))
    e01o5o4i77["Has User Cancelled Auth"] --> nb3y5kcx2q(("EVAL"))
    el9cmscetd["First Screen"] --> f0p9tnng3j(("EVAL"))
    z34hsrcd98["CIAM - Account Recovery "] --> 21l7s55n2w(("EVAL"))
    cppsibbyhy["Password Sign On Page Button Pressed"] --> ncdawmfdmo(("EVAL"))
    5b7wgayb4e["CIAM - Account Recovery "] --> w9egwegsnj(("EVAL"))
    cstwt93s8m["Check Password Status"] --> nbcsfwxqvp(("EVAL"))
    59qszmzgg5(("EVAL")) --> h4ssqha2ei["Node"]
    1r9qfce4ko["Authentication Complete"] --> n2c0bh5gsg(("EVAL"))
    x8uq3h1ccd["Return Success"] --> sdz87dk9h3(("EVAL"))
    byomx9u9ci["Set Flow Variables"] --> 2t8o7qakxh(("EVAL"))
    2t8o7qakxh(("EVAL")) --> 4rjs3llu20["Set Industry Variables"]
    907z7uvt6v(("EVAL")) --> wuhst17m2s["Node"]
    71chk8uoyb(("EVAL")) --> eht5fkf5yz["CIAM - Device Authentication"]
    r7ddjgug4y["Check if user is enabled."] --> 5gz6jcxdng(("Evaluator"))
    wuhst17m2s["Node"] --> 1nt8111fdv(("EVAL"))
    nyw41b5mjr["Check User"] --> iui85ujva3(("EVAL"))
    iui85ujva3(("EVAL")) --> eq6oq9q1ag["Find user in PingOne"]
    2ernrgqxzb["Lookup User"] --> 71chk8uoyb(("EVAL"))
    gersdqsi8h(("Evaluator")) --> mcnyjde0zd["Node"]
    dfcr1art1l(("Evaluator")) --> v64gvzmcyy["Check if MFA is enabled to this user."]
    v64gvzmcyy["Check if MFA is enabled to this user."] --> fm7p6z4lgt(("EVAL"))
    fm7p6z4lgt(("EVAL")) --> rs2jbqnsry["Check if MFA is Enabled."]
    ncdawmfdmo(("EVAL")) --> 8a3rp16jhq["Find user and error out if user not found"]
    3e86t7q5xg(("EVAL")) --> 3kgzmkm8gy["Check if  user is enabled."]
    3kgzmkm8gy["Check if  user is enabled."] --> vconl69bto(("EVAL"))
    vconl69bto(("EVAL")) --> p6hcn5iy7g["Node"]
    vconl69bto(("EVAL")) --> x15qahvbpw["Error Message for disabled user."]
    opojvoak73(("Evaluator")) --> fr9xup4p3z["Create Device"]
    3e3ddhe5la(("EVAL")) --> 79cmhtu9fy["Prompt For OTP"]
    oiy97ee3bv(("EVAL")) --> 79qzr2aabs["Configure email notification to send an email for new device added."]
    5863kwjvsw["Activate Device"] --> oiy97ee3bv(("EVAL"))
    fr9xup4p3z["Create Device"] --> 3e3ddhe5la(("EVAL"))
    wb4u3n0g7a(("Evaluator")) --> 5863kwjvsw["Activate Device"]
    79cmhtu9fy["Prompt For OTP"] --> wb4u3n0g7a(("Evaluator"))
    d2ltnk9gkn["Notify user on disabling the account for threat detection."] --> 1v3t743uow(("EVAL"))
    qmpie4zfny["Check if Known Device"] --> gaj3ygo1j4(("EVAL"))
    dt7mj4nem1(("EVAL")) --> kleitqcid7["Node"]
    1v3t743uow(("EVAL")) --> yzoki16xti["Disable user"]
    oep2ke136(("Evaluator")) --> 1fdy8se6nx["Update risk evaluation with FAILURE"]
    qvyge7omps(("EVAL")) --> d2ltnk9gkn["Notify user on disabling the account for threat detection."]
    0eroz3r95x(("EVAL")) --> uekzlj66vx["Risk Score from PingOne Protect"]
    dr1asu53u6["Get Values from PingOne Protect analysis"] --> qvyge7omps(("EVAL"))
    mg0lkb9ayl["PingOne Notifications"] --> 0eroz3r95x(("EVAL"))
    y2yl45morr(("EVAL")) --> flt9ewj1a9["Find user via userID"]
    opojvoak73(("Evaluator")) --> ml14k5xdb5["Return"]
    o0ebgiurvi(("EVAL")) --> qmpie4zfny["Check if Known Device"]
    h2wapsopzt["PingOne Protect Analysis"] --> y2yl45morr(("EVAL"))
    flt9ewj1a9["Find user via userID"] --> k3qn24f8pv(("EVAL"))
    gaj3ygo1j4(("EVAL")) --> mg0lkb9ayl["PingOne Notifications"]
    79qzr2aabs["Configure email notification to send an email for new device added."] --> 7nmwxj5w0p(("Evaluator"))
    5tz0a2yt0y["Check if MFA Size is 0"] --> opojvoak73(("Evaluator"))
    80hktgiwnm(("EVAL")) --> 8bimk6mxz4["Node"]
    7nmwxj5w0p(("Evaluator")) --> ml14k5xdb5["Return"]
    k3qn24f8pv(("EVAL")) --> mt49dyk6zx["Invoke PingOne Protect subflow"]
    mt49dyk6zx["Invoke PingOne Protect subflow"] --> w5t7jozp5a(("Evaluator"))
    w5t7jozp5a(("Evaluator")) --> gahfykd5pd["Get Values from PingOne Protect analysis"]
    w5t7jozp5a(("Evaluator")) --> dr1asu53u6["Get Values from PingOne Protect analysis"]
    gahfykd5pd["Get Values from PingOne Protect analysis"] --> o0ebgiurvi(("EVAL"))
    gaj3ygo1j4(("EVAL")) --> uekzlj66vx["Risk Score from PingOne Protect"]
    uekzlj66vx["Risk Score from PingOne Protect"] --> oc2cqsl41l(("EVAL"))
    oc2cqsl41l(("EVAL")) --> uwl9fwuq4d["return"]
    uekzlj66vx["Risk Score from PingOne Protect"] --> 0cmw42tqse(("EVAL"))
    yzoki16xti["Disable user"] --> dt7mj4nem1(("EVAL"))
    uekzlj66vx["Risk Score from PingOne Protect"] --> 80hktgiwnm(("EVAL"))
    340awenest(("EVAL")) --> 3qrmnag6il["Node"]
    muyh5iinqk["Node"] --> yr66uwy0ma(("EVAL"))
    lbhyjujyjv(("Evaluator")) --> qimhttv2jm["Initiate Sk-risk"]
    qimhttv2jm["Initiate Sk-risk"] --> i21ma1l9mn(("EVAL"))
    ybma422b3i(("EVAL")) --> yfv4l5oqrn["User Not Found Error"]
    71chk8uoyb(("EVAL")) --> n55ilztdeo["User Not Found Error"]
    0e7xqfqq2e["Return With Success Response"] --> 69tmgilhek(("Evaluator"))
    69tmgilhek(("Evaluator")) --> 3s1kipk6u3["Node"]

    click i21ma1l9mn "vscode://file/./nodes/i21ma1l9mn.md" _parent
    click muyh5iinqk "vscode://file/./nodes/muyh5iinqk.md" _parent
    click mkz8u9xtjp "vscode://file/./nodes/mkz8u9xtjp.md" _parent
    click dv7x4k323t "vscode://file/./nodes/dv7x4k323t.md" _parent
    click 0cmw42tqse "vscode://file/./nodes/0cmw42tqse.md" _parent
    click bcrh9zpo2j "vscode://file/./nodes/bcrh9zpo2j.md" _parent
    click hun8tkpynt "vscode://file/./nodes/hun8tkpynt.md" _parent
    click 7186msgx2b "vscode://file/./nodes/7186msgx2b.md" _parent
    click 1gv745vu9f "vscode://file/./nodes/1gv745vu9f.md" _parent
    click 5tz0a2yt0y "vscode://file/./nodes/5tz0a2yt0y.md" _parent
    click 7186msgx2b "vscode://file/./nodes/7186msgx2b.md" _parent
    click fqw47ezfd4 "vscode://file/./nodes/fqw47ezfd4.md" _parent
    click 0cdm5xwnl3 "vscode://file/./nodes/0cdm5xwnl3.md" _parent
    click oep2ke136 "vscode://file/./nodes/oep2ke136.md" _parent
    click sdz87dk9h3 "vscode://file/./nodes/sdz87dk9h3.md" _parent
    click hun8tkpynt "vscode://file/./nodes/hun8tkpynt.md" _parent
    click 2ixdpv74ih "vscode://file/./nodes/2ixdpv74ih.md" _parent
    click 0cdm5xwnl3 "vscode://file/./nodes/0cdm5xwnl3.md" _parent
    click ybma422b3i "vscode://file/./nodes/ybma422b3i.md" _parent
    click 3dpidmgj6g "vscode://file/./nodes/3dpidmgj6g.md" _parent
    click 8a3rp16jhq "vscode://file/./nodes/8a3rp16jhq.md" _parent
    click ybma422b3i "vscode://file/./nodes/ybma422b3i.md" _parent
    click eq6oq9q1ag "vscode://file/./nodes/eq6oq9q1ag.md" _parent
    click 71uz2oxfw9 "vscode://file/./nodes/71uz2oxfw9.md" _parent
    click 5gz6jcxdng "vscode://file/./nodes/5gz6jcxdng.md" _parent
    click ptslfr1den "vscode://file/./nodes/ptslfr1den.md" _parent
    click rmx6s73ihv "vscode://file/./nodes/rmx6s73ihv.md" _parent
    click 59qszmzgg5 "vscode://file/./nodes/59qszmzgg5.md" _parent
    click 71uz2oxfw9 "vscode://file/./nodes/71uz2oxfw9.md" _parent
    click r7ddjgug4y "vscode://file/./nodes/r7ddjgug4y.md" _parent
    click ph08u6bgi1 "vscode://file/./nodes/ph08u6bgi1.md" _parent
    click hcdhp9ww20 "vscode://file/./nodes/hcdhp9ww20.md" _parent
    click dv7x4k323t "vscode://file/./nodes/dv7x4k323t.md" _parent
    click gersdqsi8h "vscode://file/./nodes/gersdqsi8h.md" _parent
    click ptslfr1den "vscode://file/./nodes/ptslfr1den.md" _parent
    click dfcr1art1l "vscode://file/./nodes/dfcr1art1l.md" _parent
    click dfcr1art1l "vscode://file/./nodes/dfcr1art1l.md" _parent
    click j23r4buol6 "vscode://file/./nodes/j23r4buol6.md" _parent
    click 4rjs3llu20 "vscode://file/./nodes/4rjs3llu20.md" _parent
    click 340awenest "vscode://file/./nodes/340awenest.md" _parent
    click sdz87dk9h3 "vscode://file/./nodes/sdz87dk9h3.md" _parent
    click 5770fvct63 "vscode://file/./nodes/5770fvct63.md" _parent
    click 2ixdpv74ih "vscode://file/./nodes/2ixdpv74ih.md" _parent
    click m8unn93k58 "vscode://file/./nodes/m8unn93k58.md" _parent
    click m8unn93k58 "vscode://file/./nodes/m8unn93k58.md" _parent
    click bkuqv7wdoo "vscode://file/./nodes/bkuqv7wdoo.md" _parent
    click gm6xl62pf3 "vscode://file/./nodes/gm6xl62pf3.md" _parent
    click yjz1weh9xh "vscode://file/./nodes/yjz1weh9xh.md" _parent
    click cl9ugbu07r "vscode://file/./nodes/cl9ugbu07r.md" _parent
    click 2ixdpv74ih "vscode://file/./nodes/2ixdpv74ih.md" _parent
    click jv8lvv5w4x "vscode://file/./nodes/jv8lvv5w4x.md" _parent
    click jimu9wsyls "vscode://file/./nodes/jimu9wsyls.md" _parent
    click 5770fvct63 "vscode://file/./nodes/5770fvct63.md" _parent
    click eum65le218 "vscode://file/./nodes/eum65le218.md" _parent
    click asnrb9403q "vscode://file/./nodes/asnrb9403q.md" _parent
    click njmld8889h "vscode://file/./nodes/njmld8889h.md" _parent
    click qdea3v0byw "vscode://file/./nodes/qdea3v0byw.md" _parent
    click oca826nc0b "vscode://file/./nodes/oca826nc0b.md" _parent
    click yjz1weh9xh "vscode://file/./nodes/yjz1weh9xh.md" _parent
    click yr9tytff7 "vscode://file/./nodes/yr9tytff7.md" _parent
    click j7vnuet5bk "vscode://file/./nodes/j7vnuet5bk.md" _parent
    click 3lgnmx50te "vscode://file/./nodes/3lgnmx50te.md" _parent
    click bkuqv7wdoo "vscode://file/./nodes/bkuqv7wdoo.md" _parent
    click gm6xl62pf3 "vscode://file/./nodes/gm6xl62pf3.md" _parent
    click cppsibbyhy "vscode://file/./nodes/cppsibbyhy.md" _parent
    click 8epxzybfo "vscode://file/./nodes/8epxzybfo.md" _parent
    click jimu9wsyls "vscode://file/./nodes/jimu9wsyls.md" _parent
    click jio5trsqxr "vscode://file/./nodes/jio5trsqxr.md" _parent
    click eum65le218 "vscode://file/./nodes/eum65le218.md" _parent
    click zlublpnvlp "vscode://file/./nodes/zlublpnvlp.md" _parent
    click 5770fvct63 "vscode://file/./nodes/5770fvct63.md" _parent
    click jv8lvv5w4x "vscode://file/./nodes/jv8lvv5w4x.md" _parent
    click jio5trsqxr "vscode://file/./nodes/jio5trsqxr.md" _parent
    click 0e7xqfqq2e "vscode://file/./nodes/0e7xqfqq2e.md" _parent
    click wcask7tfhv "vscode://file/./nodes/wcask7tfhv.md" _parent
    click z34hsrcd98 "vscode://file/./nodes/z34hsrcd98.md" _parent
    click m2zwktv18x "vscode://file/./nodes/m2zwktv18x.md" _parent
    click drg4lvxpjw "vscode://file/./nodes/drg4lvxpjw.md" _parent
    click ins74ygtvc "vscode://file/./nodes/ins74ygtvc.md" _parent
    click fqkfitsm9p "vscode://file/./nodes/fqkfitsm9p.md" _parent
    click fqkfitsm9p "vscode://file/./nodes/fqkfitsm9p.md" _parent
    click w16j6hvh6d "vscode://file/./nodes/w16j6hvh6d.md" _parent
    click zkdpy8oqb5 "vscode://file/./nodes/zkdpy8oqb5.md" _parent
    click 5g1u9k5fi3 "vscode://file/./nodes/5g1u9k5fi3.md" _parent
    click cppsibbyhy "vscode://file/./nodes/cppsibbyhy.md" _parent
    click n5vpbff54 "vscode://file/./nodes/n5vpbff54.md" _parent
    click hp2eob8gy8 "vscode://file/./nodes/hp2eob8gy8.md" _parent
    click rtjwqkq5ng "vscode://file/./nodes/rtjwqkq5ng.md" _parent
    click aeek6nl8wj "vscode://file/./nodes/aeek6nl8wj.md" _parent
    click yt7rz448i7 "vscode://file/./nodes/yt7rz448i7.md" _parent
    click 85rxatuk44 "vscode://file/./nodes/85rxatuk44.md" _parent
    click qc1wiq047b "vscode://file/./nodes/qc1wiq047b.md" _parent
    click g1w1cltra3 "vscode://file/./nodes/g1w1cltra3.md" _parent
    click hzmdf4b1w6 "vscode://file/./nodes/hzmdf4b1w6.md" _parent
    click 60dszexpy6 "vscode://file/./nodes/60dszexpy6.md" _parent
    click 6961q0o277 "vscode://file/./nodes/6961q0o277.md" _parent
    click qc1wiq047b "vscode://file/./nodes/qc1wiq047b.md" _parent
    click 83g36u9ohr "vscode://file/./nodes/83g36u9ohr.md" _parent
    click 83g36u9ohr "vscode://file/./nodes/83g36u9ohr.md" _parent
    click sbudfzsp5m "vscode://file/./nodes/sbudfzsp5m.md" _parent
    click sbudfzsp5m "vscode://file/./nodes/sbudfzsp5m.md" _parent
    click ug3m1588jl "vscode://file/./nodes/ug3m1588jl.md" _parent
    click ug3m1588jl "vscode://file/./nodes/ug3m1588jl.md" _parent
    click y1g5lzp3md "vscode://file/./nodes/y1g5lzp3md.md" _parent
    click 8b7afymuxh "vscode://file/./nodes/8b7afymuxh.md" _parent
    click wdhgxaxnfa "vscode://file/./nodes/wdhgxaxnfa.md" _parent
    click ug3m1588jl "vscode://file/./nodes/ug3m1588jl.md" _parent
    click synvhooann "vscode://file/./nodes/synvhooann.md" _parent
    click 8b7afymuxh "vscode://file/./nodes/8b7afymuxh.md" _parent
    click se0w7zdrd7 "vscode://file/./nodes/se0w7zdrd7.md" _parent
    click y1g5lzp3md "vscode://file/./nodes/y1g5lzp3md.md" _parent
    click 8b7afymuxh "vscode://file/./nodes/8b7afymuxh.md" _parent
    click cao68g3gyc "vscode://file/./nodes/cao68g3gyc.md" _parent
    click e0fk3mmhht "vscode://file/./nodes/e0fk3mmhht.md" _parent
    click zkdpy8oqb5 "vscode://file/./nodes/zkdpy8oqb5.md" _parent
    click r60mrklkuw "vscode://file/./nodes/r60mrklkuw.md" _parent
    click n2c0bh5gsg "vscode://file/./nodes/n2c0bh5gsg.md" _parent
    click c3x77vuo10 "vscode://file/./nodes/c3x77vuo10.md" _parent
    click ozb119ee81 "vscode://file/./nodes/ozb119ee81.md" _parent
    click m8opeg6ilr "vscode://file/./nodes/m8opeg6ilr.md" _parent
    click hp2eob8gy8 "vscode://file/./nodes/hp2eob8gy8.md" _parent
    click e01o5o4i77 "vscode://file/./nodes/e01o5o4i77.md" _parent
    click c3x77vuo10 "vscode://file/./nodes/c3x77vuo10.md" _parent
    click 76t9hosyif "vscode://file/./nodes/76t9hosyif.md" _parent
    click pmzg2ixr1g "vscode://file/./nodes/pmzg2ixr1g.md" _parent
    click 90yph4ra19 "vscode://file/./nodes/90yph4ra19.md" _parent
    click flmowbcu44 "vscode://file/./nodes/flmowbcu44.md" _parent
    click aeev9gqagj "vscode://file/./nodes/aeev9gqagj.md" _parent
    click w9egwegsnj "vscode://file/./nodes/w9egwegsnj.md" _parent
    click cqktdyqncg "vscode://file/./nodes/cqktdyqncg.md" _parent
    click gqbh7qw6qa "vscode://file/./nodes/gqbh7qw6qa.md" _parent
    click 614hjulpdj "vscode://file/./nodes/614hjulpdj.md" _parent
    click nb3y5kcx2q "vscode://file/./nodes/nb3y5kcx2q.md" _parent
    click ze4pz75nx "vscode://file/./nodes/ze4pz75nx.md" _parent
    click b275pagysx "vscode://file/./nodes/b275pagysx.md" _parent
    click scxeegwacj "vscode://file/./nodes/scxeegwacj.md" _parent
    click c9kmm14iq0 "vscode://file/./nodes/c9kmm14iq0.md" _parent
    click b275pagysx "vscode://file/./nodes/b275pagysx.md" _parent
    click yr66uwy0ma "vscode://file/./nodes/yr66uwy0ma.md" _parent
    click 0fezdflrz4 "vscode://file/./nodes/0fezdflrz4.md" _parent
    click 76t9hosyif "vscode://file/./nodes/76t9hosyif.md" _parent
    click frkr1a0u82 "vscode://file/./nodes/frkr1a0u82.md" _parent
    click scxeegwacj "vscode://file/./nodes/scxeegwacj.md" _parent
    click 8b6kcm9yz6 "vscode://file/./nodes/8b6kcm9yz6.md" _parent
    click hzmdf4b1w6 "vscode://file/./nodes/hzmdf4b1w6.md" _parent
    click wxocgg04qz "vscode://file/./nodes/wxocgg04qz.md" _parent
    click 1qqopmsxn1 "vscode://file/./nodes/1qqopmsxn1.md" _parent
    click tcx0nm2t9o "vscode://file/./nodes/tcx0nm2t9o.md" _parent
    click 1qqopmsxn1 "vscode://file/./nodes/1qqopmsxn1.md" _parent
    click so58xwowjn "vscode://file/./nodes/so58xwowjn.md" _parent
    click tcx0nm2t9o "vscode://file/./nodes/tcx0nm2t9o.md" _parent
    click 096blcsiod "vscode://file/./nodes/096blcsiod.md" _parent
    click so58xwowjn "vscode://file/./nodes/so58xwowjn.md" _parent
    click qo3pwj5p12 "vscode://file/./nodes/qo3pwj5p12.md" _parent
    click qbf8b4sda4 "vscode://file/./nodes/qbf8b4sda4.md" _parent
    click 7y41qu33vz "vscode://file/./nodes/7y41qu33vz.md" _parent
    click hzmdf4b1w6 "vscode://file/./nodes/hzmdf4b1w6.md" _parent
    click 1qqopmsxn1 "vscode://file/./nodes/1qqopmsxn1.md" _parent
    click n5vpbff54 "vscode://file/./nodes/n5vpbff54.md" _parent
    click h0rcajanl2 "vscode://file/./nodes/h0rcajanl2.md" _parent
    click lbhyjujyjv "vscode://file/./nodes/lbhyjujyjv.md" _parent
    click vztjuyevpz "vscode://file/./nodes/vztjuyevpz.md" _parent
    click d5jso3qit5 "vscode://file/./nodes/d5jso3qit5.md" _parent
    click g1w1cltra3 "vscode://file/./nodes/g1w1cltra3.md" _parent
    click cppsibbyhy "vscode://file/./nodes/cppsibbyhy.md" _parent
    click d5jso3qit5 "vscode://file/./nodes/d5jso3qit5.md" _parent
    click 2nlbum4ywj "vscode://file/./nodes/2nlbum4ywj.md" _parent
    click m2zwktv18x "vscode://file/./nodes/m2zwktv18x.md" _parent
    click m2zwktv18x "vscode://file/./nodes/m2zwktv18x.md" _parent
    click hk1hymxs4y "vscode://file/./nodes/hk1hymxs4y.md" _parent
    click qn65h94yqq "vscode://file/./nodes/qn65h94yqq.md" _parent
    click hk1hymxs4y "vscode://file/./nodes/hk1hymxs4y.md" _parent
    click vztjuyevpz "vscode://file/./nodes/vztjuyevpz.md" _parent
    click qn65h94yqq "vscode://file/./nodes/qn65h94yqq.md" _parent
    click qn65h94yqq "vscode://file/./nodes/qn65h94yqq.md" _parent
    click 2nlbum4ywj "vscode://file/./nodes/2nlbum4ywj.md" _parent
    click zlublpnvlp "vscode://file/./nodes/zlublpnvlp.md" _parent
    click o74snj74sy "vscode://file/./nodes/o74snj74sy.md" _parent
    click 3lgnmx50te "vscode://file/./nodes/3lgnmx50te.md" _parent
    click byomx9u9ci "vscode://file/./nodes/byomx9u9ci.md" _parent
    click oiauhhhv4k "vscode://file/./nodes/oiauhhhv4k.md" _parent
    click aw3ce1sq70 "vscode://file/./nodes/aw3ce1sq70.md" _parent
    click 21l7s55n2w "vscode://file/./nodes/21l7s55n2w.md" _parent
    click oiauhhhv4k "vscode://file/./nodes/oiauhhhv4k.md" _parent
    click aw3ce1sq70 "vscode://file/./nodes/aw3ce1sq70.md" _parent
    click nhs3ybbdgg "vscode://file/./nodes/nhs3ybbdgg.md" _parent
    click 60dszexpy6 "vscode://file/./nodes/60dszexpy6.md" _parent
    click xmdntu2a5o "vscode://file/./nodes/xmdntu2a5o.md" _parent
    click 3dpidmgj6g "vscode://file/./nodes/3dpidmgj6g.md" _parent
    click 3e86t7q5xg "vscode://file/./nodes/3e86t7q5xg.md" _parent
    click ri35kah4nr "vscode://file/./nodes/ri35kah4nr.md" _parent
    click as1tfleqv7 "vscode://file/./nodes/as1tfleqv7.md" _parent
    click 6961q0o277 "vscode://file/./nodes/6961q0o277.md" _parent
    click vwq8svkesj "vscode://file/./nodes/vwq8svkesj.md" _parent
    click 6x0m1t11oh "vscode://file/./nodes/6x0m1t11oh.md" _parent
    click ri35kah4nr "vscode://file/./nodes/ri35kah4nr.md" _parent
    click mkz8u9xtjp "vscode://file/./nodes/mkz8u9xtjp.md" _parent
    click rmx6s73ihv "vscode://file/./nodes/rmx6s73ihv.md" _parent
    click rc315a9uh1 "vscode://file/./nodes/rc315a9uh1.md" _parent
    click 5b7wgayb4e "vscode://file/./nodes/5b7wgayb4e.md" _parent
    click oiauhhhv4k "vscode://file/./nodes/oiauhhhv4k.md" _parent
    click o5vjpzh7bq "vscode://file/./nodes/o5vjpzh7bq.md" _parent
    click o5vjpzh7bq "vscode://file/./nodes/o5vjpzh7bq.md" _parent
    click bv4f2hdy6o "vscode://file/./nodes/bv4f2hdy6o.md" _parent
    click 1nt8111fdv "vscode://file/./nodes/1nt8111fdv.md" _parent
    click 2ernrgqxzb "vscode://file/./nodes/2ernrgqxzb.md" _parent
    click 6x0m1t11oh "vscode://file/./nodes/6x0m1t11oh.md" _parent
    click qbf8b4sda4 "vscode://file/./nodes/qbf8b4sda4.md" _parent
    click se0w7zdrd7 "vscode://file/./nodes/se0w7zdrd7.md" _parent
    click liu3llworn "vscode://file/./nodes/liu3llworn.md" _parent
    click 59qszmzgg5 "vscode://file/./nodes/59qszmzgg5.md" _parent
    click 6x0m1t11oh "vscode://file/./nodes/6x0m1t11oh.md" _parent
    click oiy97ee3bv "vscode://file/./nodes/oiy97ee3bv.md" _parent
    click vlngo6a8gl "vscode://file/./nodes/vlngo6a8gl.md" _parent
    click powvchr4kr "vscode://file/./nodes/powvchr4kr.md" _parent
    click 85rxatuk44 "vscode://file/./nodes/85rxatuk44.md" _parent
    click r01x04oq1y "vscode://file/./nodes/r01x04oq1y.md" _parent
    click mmqiyn4q46 "vscode://file/./nodes/mmqiyn4q46.md" _parent
    click liu3llworn "vscode://file/./nodes/liu3llworn.md" _parent
    click gj8d9gmnwj "vscode://file/./nodes/gj8d9gmnwj.md" _parent
    click e0fk3mmhht "vscode://file/./nodes/e0fk3mmhht.md" _parent
    click ozb119ee81 "vscode://file/./nodes/ozb119ee81.md" _parent
    click mmqiyn4q46 "vscode://file/./nodes/mmqiyn4q46.md" _parent
    click cao68g3gyc "vscode://file/./nodes/cao68g3gyc.md" _parent
    click 6x0m1t11oh "vscode://file/./nodes/6x0m1t11oh.md" _parent
    click 907z7uvt6v "vscode://file/./nodes/907z7uvt6v.md" _parent
    click 5gz6jcxdng "vscode://file/./nodes/5gz6jcxdng.md" _parent
    click bt6lzhdb0v "vscode://file/./nodes/bt6lzhdb0v.md" _parent
    click w9egwegsnj "vscode://file/./nodes/w9egwegsnj.md" _parent
    click e1w127ll95 "vscode://file/./nodes/e1w127ll95.md" _parent
    click njmld8889h "vscode://file/./nodes/njmld8889h.md" _parent
    click upanxjpo9i "vscode://file/./nodes/upanxjpo9i.md" _parent
    click infm8ry8j9 "vscode://file/./nodes/infm8ry8j9.md" _parent
    click upanxjpo9i "vscode://file/./nodes/upanxjpo9i.md" _parent
    click kpq6uykwvz "vscode://file/./nodes/kpq6uykwvz.md" _parent
    click infm8ry8j9 "vscode://file/./nodes/infm8ry8j9.md" _parent
    click 5g1u9k5fi3 "vscode://file/./nodes/5g1u9k5fi3.md" _parent
    click rgae4w87f5 "vscode://file/./nodes/rgae4w87f5.md" _parent
    click ph08u6bgi1 "vscode://file/./nodes/ph08u6bgi1.md" _parent
    click ou1gi7wq5d "vscode://file/./nodes/ou1gi7wq5d.md" _parent
    click 7y41qu33vz "vscode://file/./nodes/7y41qu33vz.md" _parent
    click 60dszexpy6 "vscode://file/./nodes/60dszexpy6.md" _parent
    click cqktdyqncg "vscode://file/./nodes/cqktdyqncg.md" _parent
    click pmzg2ixr1g "vscode://file/./nodes/pmzg2ixr1g.md" _parent
    click 4ncwrpsqgn "vscode://file/./nodes/4ncwrpsqgn.md" _parent
    click ph08u6bgi1 "vscode://file/./nodes/ph08u6bgi1.md" _parent
    click 21l7s55n2w "vscode://file/./nodes/21l7s55n2w.md" _parent
    click x5v48y5oma "vscode://file/./nodes/x5v48y5oma.md" _parent
    click cao68g3gyc "vscode://file/./nodes/cao68g3gyc.md" _parent
    click 5g1u9k5fi3 "vscode://file/./nodes/5g1u9k5fi3.md" _parent
    click rstodi2zw1 "vscode://file/./nodes/rstodi2zw1.md" _parent
    click bilu0ighwr "vscode://file/./nodes/bilu0ighwr.md" _parent
    click rqsigpn591 "vscode://file/./nodes/rqsigpn591.md" _parent
    click xfg1fliupl "vscode://file/./nodes/xfg1fliupl.md" _parent
    click fm7p6z4lgt "vscode://file/./nodes/fm7p6z4lgt.md" _parent
    click 4ncwrpsqgn "vscode://file/./nodes/4ncwrpsqgn.md" _parent
    click eht5fkf5yz "vscode://file/./nodes/eht5fkf5yz.md" _parent
    click hp2eob8gy8 "vscode://file/./nodes/hp2eob8gy8.md" _parent
    click o74snj74sy "vscode://file/./nodes/o74snj74sy.md" _parent
    click wuyh51gb1x "vscode://file/./nodes/wuyh51gb1x.md" _parent
    click c9kmm14iq0 "vscode://file/./nodes/c9kmm14iq0.md" _parent
    click cstwt93s8m "vscode://file/./nodes/cstwt93s8m.md" _parent
    click y7f4468q9f "vscode://file/./nodes/y7f4468q9f.md" _parent
    click zoqe5yn0jc "vscode://file/./nodes/zoqe5yn0jc.md" _parent
    click 6x0m1t11oh "vscode://file/./nodes/6x0m1t11oh.md" _parent
    click wcask7tfhv "vscode://file/./nodes/wcask7tfhv.md" _parent
    click bcrh9zpo2j "vscode://file/./nodes/bcrh9zpo2j.md" _parent
    click 1gv745vu9f "vscode://file/./nodes/1gv745vu9f.md" _parent
    click 8epxzybfo "vscode://file/./nodes/8epxzybfo.md" _parent
    click rmx6s73ihv "vscode://file/./nodes/rmx6s73ihv.md" _parent
    click 6x0m1t11oh "vscode://file/./nodes/6x0m1t11oh.md" _parent
    click gqbh7qw6qa "vscode://file/./nodes/gqbh7qw6qa.md" _parent
    click w16j6hvh6d "vscode://file/./nodes/w16j6hvh6d.md" _parent
    click lbhyjujyjv "vscode://file/./nodes/lbhyjujyjv.md" _parent
    click cppsibbyhy "vscode://file/./nodes/cppsibbyhy.md" _parent
    click rc315a9uh1 "vscode://file/./nodes/rc315a9uh1.md" _parent
    click m8opeg6ilr "vscode://file/./nodes/m8opeg6ilr.md" _parent
    click zkdpy8oqb5 "vscode://file/./nodes/zkdpy8oqb5.md" _parent
    click r01x04oq1y "vscode://file/./nodes/r01x04oq1y.md" _parent
    click shrf93ss72 "vscode://file/./nodes/shrf93ss72.md" _parent
    click imnmdfh12z "vscode://file/./nodes/imnmdfh12z.md" _parent
    click ed4e0aipzr "vscode://file/./nodes/ed4e0aipzr.md" _parent
    click vwq8svkesj "vscode://file/./nodes/vwq8svkesj.md" _parent
    click 6p48mt9nzd "vscode://file/./nodes/6p48mt9nzd.md" _parent
    click gersdqsi8h "vscode://file/./nodes/gersdqsi8h.md" _parent
    click cppsibbyhy "vscode://file/./nodes/cppsibbyhy.md" _parent
    click 8fovn3syu3 "vscode://file/./nodes/8fovn3syu3.md" _parent
    click mkz8u9xtjp "vscode://file/./nodes/mkz8u9xtjp.md" _parent
    click cstwt93s8m "vscode://file/./nodes/cstwt93s8m.md" _parent
    click rqsigpn591 "vscode://file/./nodes/rqsigpn591.md" _parent
    click 6961q0o277 "vscode://file/./nodes/6961q0o277.md" _parent
    click aeek6nl8wj "vscode://file/./nodes/aeek6nl8wj.md" _parent
    click f0p9tnng3j "vscode://file/./nodes/f0p9tnng3j.md" _parent
    click 8fovn3syu3 "vscode://file/./nodes/8fovn3syu3.md" _parent
    click us1sbucx0m "vscode://file/./nodes/us1sbucx0m.md" _parent
    click c9kmm14iq0 "vscode://file/./nodes/c9kmm14iq0.md" _parent
    click scxeegwacj "vscode://file/./nodes/scxeegwacj.md" _parent
    click a5vlldmzi6 "vscode://file/./nodes/a5vlldmzi6.md" _parent
    click nbcsfwxqvp "vscode://file/./nodes/nbcsfwxqvp.md" _parent
    click c8p1c19w99 "vscode://file/./nodes/c8p1c19w99.md" _parent
    click cstwt93s8m "vscode://file/./nodes/cstwt93s8m.md" _parent
    click imnmdfh12z "vscode://file/./nodes/imnmdfh12z.md" _parent
    click y7f4468q9f "vscode://file/./nodes/y7f4468q9f.md" _parent
    click us1sbucx0m "vscode://file/./nodes/us1sbucx0m.md" _parent
    click bilu0ighwr "vscode://file/./nodes/bilu0ighwr.md" _parent
    click t09lk8opxa "vscode://file/./nodes/t09lk8opxa.md" _parent
    click 71uz2oxfw9 "vscode://file/./nodes/71uz2oxfw9.md" _parent
    click fdo3dhvrb8 "vscode://file/./nodes/fdo3dhvrb8.md" _parent
    click nb3y5kcx2q "vscode://file/./nodes/nb3y5kcx2q.md" _parent
    click whgnox29ew "vscode://file/./nodes/whgnox29ew.md" _parent
    click frkr1a0u82 "vscode://file/./nodes/frkr1a0u82.md" _parent
    click r01x04oq1y "vscode://file/./nodes/r01x04oq1y.md" _parent
    click rgae4w87f5 "vscode://file/./nodes/rgae4w87f5.md" _parent
    click kpq6uykwvz "vscode://file/./nodes/kpq6uykwvz.md" _parent
    click t09lk8opxa "vscode://file/./nodes/t09lk8opxa.md" _parent
    click y7f4468q9f "vscode://file/./nodes/y7f4468q9f.md" _parent
    click cqktdyqncg "vscode://file/./nodes/cqktdyqncg.md" _parent
    click flmowbcu44 "vscode://file/./nodes/flmowbcu44.md" _parent
    click rgae4w87f5 "vscode://file/./nodes/rgae4w87f5.md" _parent
    click asnrb9403q "vscode://file/./nodes/asnrb9403q.md" _parent
    click gm6xl62pf3 "vscode://file/./nodes/gm6xl62pf3.md" _parent
    click qdea3v0byw "vscode://file/./nodes/qdea3v0byw.md" _parent
    click e01o5o4i77 "vscode://file/./nodes/e01o5o4i77.md" _parent
    click nb3y5kcx2q "vscode://file/./nodes/nb3y5kcx2q.md" _parent
    click el9cmscetd "vscode://file/./nodes/el9cmscetd.md" _parent
    click f0p9tnng3j "vscode://file/./nodes/f0p9tnng3j.md" _parent
    click z34hsrcd98 "vscode://file/./nodes/z34hsrcd98.md" _parent
    click 21l7s55n2w "vscode://file/./nodes/21l7s55n2w.md" _parent
    click cppsibbyhy "vscode://file/./nodes/cppsibbyhy.md" _parent
    click ncdawmfdmo "vscode://file/./nodes/ncdawmfdmo.md" _parent
    click 5b7wgayb4e "vscode://file/./nodes/5b7wgayb4e.md" _parent
    click w9egwegsnj "vscode://file/./nodes/w9egwegsnj.md" _parent
    click cstwt93s8m "vscode://file/./nodes/cstwt93s8m.md" _parent
    click nbcsfwxqvp "vscode://file/./nodes/nbcsfwxqvp.md" _parent
    click 59qszmzgg5 "vscode://file/./nodes/59qszmzgg5.md" _parent
    click h4ssqha2ei "vscode://file/./nodes/h4ssqha2ei.md" _parent
    click 1r9qfce4ko "vscode://file/./nodes/1r9qfce4ko.md" _parent
    click n2c0bh5gsg "vscode://file/./nodes/n2c0bh5gsg.md" _parent
    click x8uq3h1ccd "vscode://file/./nodes/x8uq3h1ccd.md" _parent
    click sdz87dk9h3 "vscode://file/./nodes/sdz87dk9h3.md" _parent
    click byomx9u9ci "vscode://file/./nodes/byomx9u9ci.md" _parent
    click 2t8o7qakxh "vscode://file/./nodes/2t8o7qakxh.md" _parent
    click 2t8o7qakxh "vscode://file/./nodes/2t8o7qakxh.md" _parent
    click 4rjs3llu20 "vscode://file/./nodes/4rjs3llu20.md" _parent
    click 907z7uvt6v "vscode://file/./nodes/907z7uvt6v.md" _parent
    click wuhst17m2s "vscode://file/./nodes/wuhst17m2s.md" _parent
    click 71chk8uoyb "vscode://file/./nodes/71chk8uoyb.md" _parent
    click eht5fkf5yz "vscode://file/./nodes/eht5fkf5yz.md" _parent
    click r7ddjgug4y "vscode://file/./nodes/r7ddjgug4y.md" _parent
    click 5gz6jcxdng "vscode://file/./nodes/5gz6jcxdng.md" _parent
    click wuhst17m2s "vscode://file/./nodes/wuhst17m2s.md" _parent
    click 1nt8111fdv "vscode://file/./nodes/1nt8111fdv.md" _parent
    click nyw41b5mjr "vscode://file/./nodes/nyw41b5mjr.md" _parent
    click iui85ujva3 "vscode://file/./nodes/iui85ujva3.md" _parent
    click iui85ujva3 "vscode://file/./nodes/iui85ujva3.md" _parent
    click eq6oq9q1ag "vscode://file/./nodes/eq6oq9q1ag.md" _parent
    click 2ernrgqxzb "vscode://file/./nodes/2ernrgqxzb.md" _parent
    click 71chk8uoyb "vscode://file/./nodes/71chk8uoyb.md" _parent
    click gersdqsi8h "vscode://file/./nodes/gersdqsi8h.md" _parent
    click mcnyjde0zd "vscode://file/./nodes/mcnyjde0zd.md" _parent
    click dfcr1art1l "vscode://file/./nodes/dfcr1art1l.md" _parent
    click v64gvzmcyy "vscode://file/./nodes/v64gvzmcyy.md" _parent
    click v64gvzmcyy "vscode://file/./nodes/v64gvzmcyy.md" _parent
    click fm7p6z4lgt "vscode://file/./nodes/fm7p6z4lgt.md" _parent
    click fm7p6z4lgt "vscode://file/./nodes/fm7p6z4lgt.md" _parent
    click rs2jbqnsry "vscode://file/./nodes/rs2jbqnsry.md" _parent
    click ncdawmfdmo "vscode://file/./nodes/ncdawmfdmo.md" _parent
    click 8a3rp16jhq "vscode://file/./nodes/8a3rp16jhq.md" _parent
    click 3e86t7q5xg "vscode://file/./nodes/3e86t7q5xg.md" _parent
    click 3kgzmkm8gy "vscode://file/./nodes/3kgzmkm8gy.md" _parent
    click 3kgzmkm8gy "vscode://file/./nodes/3kgzmkm8gy.md" _parent
    click vconl69bto "vscode://file/./nodes/vconl69bto.md" _parent
    click vconl69bto "vscode://file/./nodes/vconl69bto.md" _parent
    click p6hcn5iy7g "vscode://file/./nodes/p6hcn5iy7g.md" _parent
    click vconl69bto "vscode://file/./nodes/vconl69bto.md" _parent
    click x15qahvbpw "vscode://file/./nodes/x15qahvbpw.md" _parent
    click opojvoak73 "vscode://file/./nodes/opojvoak73.md" _parent
    click fr9xup4p3z "vscode://file/./nodes/fr9xup4p3z.md" _parent
    click 3e3ddhe5la "vscode://file/./nodes/3e3ddhe5la.md" _parent
    click 79cmhtu9fy "vscode://file/./nodes/79cmhtu9fy.md" _parent
    click oiy97ee3bv "vscode://file/./nodes/oiy97ee3bv.md" _parent
    click 79qzr2aabs "vscode://file/./nodes/79qzr2aabs.md" _parent
    click 5863kwjvsw "vscode://file/./nodes/5863kwjvsw.md" _parent
    click oiy97ee3bv "vscode://file/./nodes/oiy97ee3bv.md" _parent
    click fr9xup4p3z "vscode://file/./nodes/fr9xup4p3z.md" _parent
    click 3e3ddhe5la "vscode://file/./nodes/3e3ddhe5la.md" _parent
    click wb4u3n0g7a "vscode://file/./nodes/wb4u3n0g7a.md" _parent
    click 5863kwjvsw "vscode://file/./nodes/5863kwjvsw.md" _parent
    click 79cmhtu9fy "vscode://file/./nodes/79cmhtu9fy.md" _parent
    click wb4u3n0g7a "vscode://file/./nodes/wb4u3n0g7a.md" _parent
    click d2ltnk9gkn "vscode://file/./nodes/d2ltnk9gkn.md" _parent
    click 1v3t743uow "vscode://file/./nodes/1v3t743uow.md" _parent
    click qmpie4zfny "vscode://file/./nodes/qmpie4zfny.md" _parent
    click gaj3ygo1j4 "vscode://file/./nodes/gaj3ygo1j4.md" _parent
    click dt7mj4nem1 "vscode://file/./nodes/dt7mj4nem1.md" _parent
    click kleitqcid7 "vscode://file/./nodes/kleitqcid7.md" _parent
    click 1v3t743uow "vscode://file/./nodes/1v3t743uow.md" _parent
    click yzoki16xti "vscode://file/./nodes/yzoki16xti.md" _parent
    click oep2ke136 "vscode://file/./nodes/oep2ke136.md" _parent
    click 1fdy8se6nx "vscode://file/./nodes/1fdy8se6nx.md" _parent
    click qvyge7omps "vscode://file/./nodes/qvyge7omps.md" _parent
    click d2ltnk9gkn "vscode://file/./nodes/d2ltnk9gkn.md" _parent
    click 0eroz3r95x "vscode://file/./nodes/0eroz3r95x.md" _parent
    click uekzlj66vx "vscode://file/./nodes/uekzlj66vx.md" _parent
    click dr1asu53u6 "vscode://file/./nodes/dr1asu53u6.md" _parent
    click qvyge7omps "vscode://file/./nodes/qvyge7omps.md" _parent
    click mg0lkb9ayl "vscode://file/./nodes/mg0lkb9ayl.md" _parent
    click 0eroz3r95x "vscode://file/./nodes/0eroz3r95x.md" _parent
    click y2yl45morr "vscode://file/./nodes/y2yl45morr.md" _parent
    click flt9ewj1a9 "vscode://file/./nodes/flt9ewj1a9.md" _parent
    click opojvoak73 "vscode://file/./nodes/opojvoak73.md" _parent
    click ml14k5xdb5 "vscode://file/./nodes/ml14k5xdb5.md" _parent
    click o0ebgiurvi "vscode://file/./nodes/o0ebgiurvi.md" _parent
    click qmpie4zfny "vscode://file/./nodes/qmpie4zfny.md" _parent
    click h2wapsopzt "vscode://file/./nodes/h2wapsopzt.md" _parent
    click y2yl45morr "vscode://file/./nodes/y2yl45morr.md" _parent
    click flt9ewj1a9 "vscode://file/./nodes/flt9ewj1a9.md" _parent
    click k3qn24f8pv "vscode://file/./nodes/k3qn24f8pv.md" _parent
    click gaj3ygo1j4 "vscode://file/./nodes/gaj3ygo1j4.md" _parent
    click mg0lkb9ayl "vscode://file/./nodes/mg0lkb9ayl.md" _parent
    click 79qzr2aabs "vscode://file/./nodes/79qzr2aabs.md" _parent
    click 7nmwxj5w0p "vscode://file/./nodes/7nmwxj5w0p.md" _parent
    click 5tz0a2yt0y "vscode://file/./nodes/5tz0a2yt0y.md" _parent
    click opojvoak73 "vscode://file/./nodes/opojvoak73.md" _parent
    click 80hktgiwnm "vscode://file/./nodes/80hktgiwnm.md" _parent
    click 8bimk6mxz4 "vscode://file/./nodes/8bimk6mxz4.md" _parent
    click 7nmwxj5w0p "vscode://file/./nodes/7nmwxj5w0p.md" _parent
    click ml14k5xdb5 "vscode://file/./nodes/ml14k5xdb5.md" _parent
    click k3qn24f8pv "vscode://file/./nodes/k3qn24f8pv.md" _parent
    click mt49dyk6zx "vscode://file/./nodes/mt49dyk6zx.md" _parent
    click mt49dyk6zx "vscode://file/./nodes/mt49dyk6zx.md" _parent
    click w5t7jozp5a "vscode://file/./nodes/w5t7jozp5a.md" _parent
    click w5t7jozp5a "vscode://file/./nodes/w5t7jozp5a.md" _parent
    click gahfykd5pd "vscode://file/./nodes/gahfykd5pd.md" _parent
    click w5t7jozp5a "vscode://file/./nodes/w5t7jozp5a.md" _parent
    click dr1asu53u6 "vscode://file/./nodes/dr1asu53u6.md" _parent
    click gahfykd5pd "vscode://file/./nodes/gahfykd5pd.md" _parent
    click o0ebgiurvi "vscode://file/./nodes/o0ebgiurvi.md" _parent
    click gaj3ygo1j4 "vscode://file/./nodes/gaj3ygo1j4.md" _parent
    click uekzlj66vx "vscode://file/./nodes/uekzlj66vx.md" _parent
    click uekzlj66vx "vscode://file/./nodes/uekzlj66vx.md" _parent
    click oc2cqsl41l "vscode://file/./nodes/oc2cqsl41l.md" _parent
    click oc2cqsl41l "vscode://file/./nodes/oc2cqsl41l.md" _parent
    click uwl9fwuq4d "vscode://file/./nodes/uwl9fwuq4d.md" _parent
    click uekzlj66vx "vscode://file/./nodes/uekzlj66vx.md" _parent
    click 0cmw42tqse "vscode://file/./nodes/0cmw42tqse.md" _parent
    click yzoki16xti "vscode://file/./nodes/yzoki16xti.md" _parent
    click dt7mj4nem1 "vscode://file/./nodes/dt7mj4nem1.md" _parent
    click uekzlj66vx "vscode://file/./nodes/uekzlj66vx.md" _parent
    click 80hktgiwnm "vscode://file/./nodes/80hktgiwnm.md" _parent
    click 340awenest "vscode://file/./nodes/340awenest.md" _parent
    click 3qrmnag6il "vscode://file/./nodes/3qrmnag6il.md" _parent
    click muyh5iinqk "vscode://file/./nodes/muyh5iinqk.md" _parent
    click yr66uwy0ma "vscode://file/./nodes/yr66uwy0ma.md" _parent
    click lbhyjujyjv "vscode://file/./nodes/lbhyjujyjv.md" _parent
    click qimhttv2jm "vscode://file/./nodes/qimhttv2jm.md" _parent
    click qimhttv2jm "vscode://file/./nodes/qimhttv2jm.md" _parent
    click i21ma1l9mn "vscode://file/./nodes/i21ma1l9mn.md" _parent
    click ybma422b3i "vscode://file/./nodes/ybma422b3i.md" _parent
    click yfv4l5oqrn "vscode://file/./nodes/yfv4l5oqrn.md" _parent
    click 71chk8uoyb "vscode://file/./nodes/71chk8uoyb.md" _parent
    click n55ilztdeo "vscode://file/./nodes/n55ilztdeo.md" _parent
    click 0e7xqfqq2e "vscode://file/./nodes/0e7xqfqq2e.md" _parent
    click 69tmgilhek "vscode://file/./nodes/69tmgilhek.md" _parent
    click 69tmgilhek "vscode://file/./nodes/69tmgilhek.md" _parent
    click 3s1kipk6u3 "vscode://file/./nodes/3s1kipk6u3.md" _parent
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
| agreementId##SK##flowInstance | 29d5d681-93ee-4590-abdc-7d7cd94aa85c | flowInstance |  | string | 0 | 2000 | true | property | 
 | ciam_accountRecoveryEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_agreementEnabled##SK##company | false | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_appleEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_authMethod##SK##flowInstance |  | flowInstance |  | string | 0 | 2000 | true | property | 
 | ciam_companyName##SK##company | Ping Identity | company |  | string | 0 | 2000 | false | property | 
 | ciam_emailOtpEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_facebookEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_fidoPasskeyEnabled##SK##company | false | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_googleEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_logoStyle##SK##company | width: 65px; height: 65px; | company | CSS style for company logo | string | 0 | 2000 | true | property | 
 | ciam_logoUrl##SK##company | https://assets.pingone.com/ux/ui-library/5.0.2/images/logo-pingidentity.png | company | URL of company logo | string | 0 | 2000 | true | property | 
 | ciam_magicLinkEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 | ciam_passwordlessRequired##SK##company | false | company |  | boolean | 0 | 2000 | false | property | 
 | ciam_protectDeviceStatus##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne protect flow | string | 0 | 2000 | true | property | 
 | ciam_protectPredictor##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne Protect flows. | string | 0 | 2000 | true | property | 
 | ciam_protectRiskID##SK##flowInstance |  | flowInstance | This variable is used by CIAM Passwordless with pingone protect flows. | string | 0 | 2000 | true | property | 
 | ciam_protectRiskLevel##SK##flowInstance |  | flowInstance | Used by CIAM Passwordless and PingOne protect flows | string | 0 | 2000 | true | property | 
 | ciam_protectriskPolicyId##SK##flowInstance |  | flowInstance | This PingOne Protect Risk Policy ID will be passed by default. | string | 0 | 2000 | true | property | 
 | ciam_sessionLengthInMinute##SK##company | 5 | company |  | number | 0 | 2000 | false | property | 
 | ciam_smsOtpEnabled##SK##company | true | company |  | boolean | 0 | 2000 | true | property | 
 

### Custom CSS
~> Note: Custom CSS is applied to every node in the flow

```css
.companyLogo {
    /* Ping Logo  */
    content: url("https://assets.pingone.com/ux/ui-library/5.0.2/images/logo-pingidentity.png");
    width: 65px;
    height: 65px;
}
```
