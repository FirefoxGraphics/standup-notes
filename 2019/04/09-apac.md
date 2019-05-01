tnikkel
-reviews
-figured out an different imglib intermittent (a real bug)
-RDL android backed out, fixed an (existing) problem with transaction ids and mozafterpaints
-RDL landed and stuck

jbonisteel
  * BEHOLD, the WR roadmap: https://github.com/orgs/FirefoxGraphics/projects/1
  * Also APZ: https://github.com/orgs/FirefoxGraphics/projects/2
  * Goals for the week:
    * Interview plan and score card for the role we have posted (was supposed to do that last week but failed)
    * Continue trying out the github projects thing for tracking
    * Sort out timing for next stakeholder signoff meeting we are supposed to have for WR
    * Plan a team retrospective 

gw
 * Fix for assert in WR when Fission is enabled - https://bugzilla.mozilla.org/show_bug.cgi?id=1542696
 * Investigate text clipping bug - https://bugzilla.mozilla.org/show_bug.cgi?id=1529992
 * Sketched out a rough plan for the picture caching improvements from work week.
 * Reduce use of world_content_transform - https://bugzilla.mozilla.org/show_bug.cgi?id=1542972
 * Next:
    * Change root coordinate system of plane-splitting.
    * Make use of external scroll offset during interning.
    * Start on core part of picture caching improvements.

sotaro
  * Freeze by WebGL update on android(Bug 1529870): Addressed
  * Black flash during starting rendering in GeckoView(Bug 1541145): Addressed
  * Fallback to compositor rendering during disabling WebRender on android(Bug 1533296): Wroking for the bug
  * Browser unresponsive when not all windows are displayed on Wayland(Bug 1515448): Checked-in
  * Looked into GeckoView and created some diagrams
    * https://github.com/sotaroikeda/firefox-diagrams/blob/master/mobile/mobile_GeckoSession_68.pdf
    * https://github.com/sotaroikeda/firefox-diagrams/blob/master/mobile/mobile_GeckoProcessManager_68.pdf
    * https://github.com/sotaroikeda/firefox-diagrams/blob/master/mobile/mobile_SurfaceAllocatorService_68.pdf
    * https://github.com/sotaroikeda/firefox-diagrams/blob/master/mobile/mobile_CodecProxy_68.pdf

jgilbert
  * Debugging why my ASAN builds don't run properly
  * WebGL remoting pieces
  * angle update later this week
  * Going to try to implement multiview for WebGL/FxR
