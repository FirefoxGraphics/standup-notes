gw
 * Get android sdk + mali graphics debugger working.
 * Fixed a number of extra resolve / copy steps on mobile - Bug 1531248
 * Investigating GL profile counters on mobile and experimenting with how we can make them useful.
 * Profiling slow scrolling at 4k on Intel GPUs on bugzilla - https://bugzilla.mozilla.org/show_bug.cgi?id=1530505.
   * Working today on fixing the main issues here.
* Investigations / experiments with world_content_transform / external scroll offsets.
* Get wrench running on android - https://phabricator.services.mozilla.com/D21881
* Investigating android profiling options - looking at gapid and also ds-5 studio.

sotaro
  * Looking into Performance issues on Sketchfab.com with WebRender on(Bug 1531294)
    * Too much gpu task seemed to block D3D11 api for a second.
    * Just using NV fence regressed glterrain a lot.
  * Working for SurfaceTexture usage bugs on android with webrender
  * Fixed Toggling titlebar produces empty window on wayland with WebRender(Bug 1531300)
  * Landed wbgl security bug
  * Fixed misc bugs

tnikkel
  * investigating the state of retained display lists on android
    * seems to be in pretty good state
  * intermittent bug 1306896 - likely just flakey Windows tick count

jgilbert
  * Submitted WebGL 1.0.3 conformance results!
  * WebGL remoting
  * removing size_t usage from webgl
  * asan/sec bugs
  * FYI: Expect next ANGLE update at the beginning of 68
