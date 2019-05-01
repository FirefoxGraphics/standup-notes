jbonisteel
  * Objectives this week:
    * Some prep work for certain discussions during the work week/planning prep
    * WR experiment went live in 66 yesterday! https://dbc-caf9527b-e073.cloud.databricks.com/#notebook/94118/dashboard/94226/present
    * Also doing another triage week
    * Administrative comment: we are having an "official" team dinner on Tuesday of the work week, just sent around a meeting invite. If you can't make it, no worries, can you let me know by the end of the week? 

sotaro
  * Enable shared gl on android(Bug 1532929): checked-in
  * Enable SurfaceFactory_EGLImage usage with WebRender on android(Bug 1532201): Waiting for review
  * Add handling of single buffer mode android SurfaceTexture(Bug 1529870): Waiting for review
  * Fallback from webrender error to compositor on android(Bug 1533296): Working

gw
Last week:
 - Support fast path clip-out rectangles - https://phabricator.services.mozilla.com/D24666
 - Add experimental pixel local storage render path - https://phabricator.services.mozilla.com/D24124
 - Support segment rendering for (some) pictures - https://phabricator.services.mozilla.com/D24852
 - Prototype PLS clip mask rendering - https://bugzilla.mozilla.org/show_bug.cgi?id=1536358
Next:
 - Continue profiling and fixing mobile issues. Three specific issues I'm focused on:
   - Shader times on some sites, esp. slow clip mask shaders.
   - Stalls on some sites - not GPU time specifically, likely to be hitting a stall in (texture?) updates.
   - Picture caching support on mobile. 

tnikkel
last week
  * rdl on android - a new issue turned up on try server, debugged, think I have a patch
  * imagelib intermittents - debugging, a patch that improved perf causes them
  * parent process rdl, a little debugging, a little more complicated then i thought
next
  * rdl on android - disable a few webplatform tests because they don't support fuzzy yet, hopefully turn on rdl
  * fixing those intermittents is not super easy

jgilbert
  * remoting prefactor ongoing
  * Pushing on angle update dependencies
  * webgpu proposal for buffer upload/downloads
  * Worked with jya to get my color-space conversion calculator matching specs:
    * https://jdashg.github.io/misc/colors/from-coeffs.html
