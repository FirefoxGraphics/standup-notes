Tuesday Feb 26th - APAC/PST Weekly Sync - Notes!

jbonisteel
  * Main objectives for the week:
    * Concrete next steps for WebRender + Android device
    * Work with Jeff to further triage WR P4s a little more clearly and make progress in what a better WR triage process overall should be
    * Also pushing along the bugs QA wanted fixed by March 8th: 1494924, 1495170 , 1453935
    * Make sure I am organized for cultural onboarding next week
    * Quick team update

sotaro
  * Improved Windows Intel PC performance(Bug 1528865).
    * Adding DXGI_USAGE_SHADER_INPUT flag to swap chain addressed bad picture cache performance.
    * scrolling on windows intel pc became smoother
  * Worked for security bugs. Addressed 2 security bugs.
  * Addressed WebRender related intermittent test failures(Bug 1516834, Bug 1529500)
  * Addressed GDK_BACKEND=wayland WebRender bug(Bug 1527804).
  * Started to review document split patches

Thomas
  * WebRender Release Experiments for Fx66/Fx67 remain on track. Closing in on final sign offs.
  * Data Science Peer review to be concluded this week.
  * Experiment QA scheduled for March 6th for Fx66 and May 2nd for Fx67

gw
  * Fix a regression from clip mask optimization (1529378).
  * Handle local scale for glyph rasterization (1491929).
  * Spent time thinking about / prototyping picture caching improvements.
    * WIP on normalizing local primitive / clip coordinates (1530590, 1530518).
    * Picture caching invalidation tests and infrastructure (1530242).
  * Spent quite a bit of time on reviews.
  * Investigating the Intel PC performance problem.

tnikkel
  * never ending component transfer
    * found out there were tests I wasn't running, fixed those
    * found what seems like a shader miscompilation
    * adding the _comment_ to describe the issue caused tests to fail
    * 35 try pushes later landed it
    * after landing it seems to be blamed for an intermittent

jgilbert
  * Exact GL library symbol loading
    * Seems to have caused a startup crash on some android devices (https://bugzilla.mozilla.org/show_bug.cgi?id=1420745)
  * Landed draft-pref-gated support for OES_fbo_render_mipmap
  * 
