jbonisteel
  * Last week:
    * Wrote a doc about WR on Android to try and help move that along: https://docs.google.com/document/d/1VcQ5Ecz-2ijcto8TGnvCEUqeMLpgpeVFd2Vzazo_mPI/edit#
    * Bug triaging/worrying/shepherding for WR 69
    * Kick-off recruitment for new req
  * This week:
    * Finish making interview plan
    * Make sure organized for Kris to start
  * Also heads up - I have some PTO coming up. Am off on Friday and only here Monday and Tuesday of next week

gw
 * Investigating a range of visual artifacts, some related to subpixel scrolling / picture caching, some not, e.g:
     * https://bugzilla.mozilla.org/show_bug.cgi?id=1566517
     * https://bugzilla.mozilla.org/show_bug.cgi?id=1566178
     * Fix for some (most / all?) of these bugs is https://phabricator.services.mozilla.com/D38267
 * Fix regression with preserve-3d + background-image - https://bugzilla.mozilla.org/show_bug.cgi?id=1567472
 * Fix picture caching not working on css-adriane - https://bugzilla.mozilla.org/show_bug.cgi?id=1566901
 * Updating some dependencies in WR debugger code.
 * Background work on dirty rects for tiles - https://phabricator.services.mozilla.com/D36711
 * Next: Try to repro / fix Intel glitches on some devices - https://bugzilla.mozilla.org/show_bug.cgi?id=1562462
 * Next: Continue work on multi-resolution / dirty rects for tiles. 

tnikkel
  * Windows 7 glass glitch with parent rdl (bug 1562184), debugged, patch up
  * crash caused by parent rdl, debugged, need to write patch (bug 1565922)
  * fixing first paint patch update to review comments (bug 1556568)

sotaro
  * Flickering selection/text input and jumpy scrolling (Win10 (1903)/Intel HD Graphics 530 + 620)(Bug 1556634):Looking into
  * Don't trigger composites on out-of-viewport image updates(Bug 1564646):Landed
  * Remove WebRenderTextureHostWrapper(Bug 1567816): Landed
  * Crash in [@ std::map<T>::_Try_emplace<T>](Bug 1565255):Landed
  * Re-enable test_videocontrols_onclickplay.html test (Bug 1529171)
  * Skip WR rendering until window becomes ready to draw on Wayland(Bug 1565785):Landed
  * Fix CompositorInitiallyPaused() for Wayland(Bug 1566468): Landed

jgilbert
  * Close to merging refactor for remoting
  * Reviewing per-slice uninitialized texture data tracking
  * Marked MDN status for OffscreenCanvas as "partial" instead of "full"
  * ResizeObserver discussions
  * Webgl multisampled multiview discussions
  * Direct sampling of (YUV?) video textures in WebGL discussion with Ken@Google
