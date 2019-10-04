Jbonisteel:
  * Last week:
    * Getting caught up after PTO
    * Starting onboarding doc for Kris, who will join in August
    * Submitted requests for summer interns in 2020!
    * Did some WR triage
  * Goal this week:
    * Finish the rest of the onboarding docs that I have in mind and share for feedback
    * Share Q3 OKRs
    * Update triage schedule

sotaro
  * Don't trigger composites on out-of-viewport native texture image updates(Bug 1531898): About to check in
  * Disable double buffering with compositor when device reset happens(Bug 1562847): About to check in.
  * Hovering/clicking over (seemingly random) stuff causes the whole Nightly window to jump up and down, if the window is maximized(Bug 1525084)
    * Tried to reproduce the problem on several Win10 PCs. But failed to reproduce it.
    * It might be specific to "Intel(R) HD Graphics 530". Bug 1556634 also happens on "Intel(R) HD Graphics 530"
  * Document based partial present(Bug 1550029)
    * Current patch expects to be used with document-spliting. But its implementation was changed.
    * RenderRoot::Popover was added. When it is used, partial update seems not work well.
    * Partial update might be used with picture cache. How to handle resizing window is a problem.

tnikkel
  * fixing firstpaint (bug 1556568), harder to verify then I thought since the old first paint doesn't usually trigger on my machine
  * trying an experimental patch for bug 1556687, where we get around refresh driver throttling by having the paint transaction revoked
  * regression from parent rdl in Windows glass effect (bug 1562184)

jgilbert
  * On dual-gpu Macs, only keep the dGPU on when webgl is active:
    * https://bugzilla.mozilla.org/show_bug.cgi?id=1562812
  * Fixed a perma-orange on Android
    * Lots of follow-ups to re-mark tests after fixing it
  * Reorganized webgl intermittent failure bugs, combining similar ones
    * In particular, combining out of memory bugs:
    * https://bugzilla.mozilla.org/show_bug.cgi?id=1561134
  * Fixed some Mac Mojave WebGL crashes
    * WebGL test jobs are being migrated to Mojave machines
  * Remoting integration
    * Hoping to land preffed-off in v70!
