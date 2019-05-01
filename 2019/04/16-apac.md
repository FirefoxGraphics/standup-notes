gw
 * Bug fixes for 67:
    * Plane splitting with large scale - https://phabricator.services.mozilla.com/D27462
    * Crash on large borders - https://phabricator.services.mozilla.com/D27189
 * Picture caching work:
     * Reduce world_content_transform use - https://phabricator.services.mozilla.com/D26651
     * [WIP] Patch to enable external_scroll_offset - (nearly ready!)
 * Misc:
     * Fix OOP iframe crash in Fission mode - https://phabricator.services.mozilla.com/D26611
     * Various reviews
 * Next:
     * Investigate resizing regression for 67 - https://bugzilla.mozilla.org/show_bug.cgi?id=1543356
     * Finish up and land external_scroll_offset patch.
     * Start on the core picture caching improvements work.
     * Public holidays here on 19th, 22nd and 25th.

sotaro
  * SurfaceTexture handling on WR
    * Working:video frames as a texture on WebGL does not work(Bug 1544642)
    * Fixed(Bug 1543846, Bug 1543616, Bug 1507078)
  * Regression:blank window upon startup on a specific device(Bug 1544074): Fixed by partial backing out.
  * Move NotifyWebRenderError() to CompositorManagerParent(Bug 1543560):Fixed


jbonisteel:
  * FYI - spent some time on Friday working on the WR wiki, including making some burnup charts/tables for tracking bugs: https://wiki.mozilla.org/Platform/GFX/WebRender_Planning
  * Goals for the week:
    * Finish up a few more things I want to do on the wiki
    * Support the Fission/Rendering scoping efforts
    * Keep eye on WR stuff
    * Also heads up:
      * I am out all day Wednesday at a conference (email or Slack will be fastest way to contact me)
      * Friday is a holiday in Canada (and I think EU/Australia?)

tnikkel
  * icon channel can spin the event loop (bug 1530190)
    * moving the offending api call to background thread makes it fail, trying to figure out why
  * picking up where i left off on parent rdl next. 3 or 4 bugs blocking that
    * a try server failure (have patch)
    * clicking in tab bar in windows fails sometimes
    * multiple glass item warning
    * maybe a scrolling perf issue?

jgilbert
  * webgl remoting ongoing
  * ANGLE update still in progress
    * Had to fix some bugs upsream
  * Writing a proposal for webgpu for data upload and download
  * triaging untriaged webgl component bugs
    * Where "triaged" means "has a priority"
