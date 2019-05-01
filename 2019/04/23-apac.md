gw
 (unable to attend today, apologies!)
 * Various reviews and discussions (primarily clipping, android perf).
 * Fixes / workarounds for 67 bugs that came up:
     * Visual resizing glitch - https://phabricator.services.mozilla.com/D27978
     * Plane splitting crash - https://phabricator.services.mozilla.com/D27462
 * Landed external scroll offsets work + fix a regression from it:
     * https://phabricator.services.mozilla.com/D27856
     * https://phabricator.services.mozilla.com/D28443
 * Next:
     * Start to use the external scroll offset work in existing picture caching code.
     * Continue work on the core picture caching changes.

sotaro
  * SurfaceTexture handling on WR(Bug 1544642, Bug 1544703,Bug 1543621)
  * Crash bugs(Bug 1546192, Bug 1545980)
  * NotifyWebRenderError() notification regression on Windows(Bug 1546298)

tnikkel
  * finally figured out the icon channel bug, bug 1530190
  * starting parent RDL debugging
  * need to finish patch for intermittent failure bug 1377457

