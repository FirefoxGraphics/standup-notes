jbonisteel
  * Last week goals:
    * Keeping an eye on WR bugs, self-assessments/workday admin 
  * This week:
    * Still keeping an eye on WR stuff
      * Am actually doing GFX triage this week
    * Prepping for all hands - planning, Fission stuff

sotaro
  * Alternative player(add-on) for Twitch.tv video sometimes becomes permanently black(Bug 1553969): landed to m-c
  * WebRTC screen sharing preview only works once(Bug 1557105):checked in.
  * Don't trigger composites on out-of-viewport texture updates(Bug 1531898)
    * Updated patch based on IRC discussion
  * Make D3D11TextureData and DXGIYCbCrTextureData alive during host side usage with WebRender(Bug 1556340)
    * landed to m-c
    * But caused regression: Higth memory and CPU usage when playing video in bilibili.co(Bug 1558100)
      * CanvasClient2D::Update() created TextureClient that is not recycled. It seemed to cause the regression
  * Building with --disable-printing is broken(Bug 1537586): landed to m-c

tnikkel
  * windows iconchannel follow up for a regression (bug 1556360)
  * macOS 10.15 beta came out and that caused us to crash like all the time in the mac iconchannel code (bug 1556076)
  * tier 2 test perma fail caused by parent rdl. tons of time dumped into this, not much to show for it yet. (bug 1556687)
  * looked into bug 1554149 a bit, (parent rdl perf improvement), next: continue this

gw
  * Got patches for picture caching uploaded. Working through review comments today and last few reftest failures on windows / android.
  * Working with cbrewster on bits and pieces related to SVG filters.
  * Workday assessments.
  * Next: Try to land picture caching work.
  * Next: Follow up issues / regressions related to picture caching changes.
  
jgilbert:
  * Revendoring ANGLE with a build fix for Solaris :S
  * EXT_blend_float went core in ES3.2, so many Android devices were capable all along!
  * Got Android Studio working on Linux for debugging Fennec on-device.
    * TODO: Update documentation
  * Checking in on what we're missing for WebGL 2.0.0 conformance
    * Not much on Windows
    * Mac needs a BlitFramebuffer workaround for srgb<->linear conversions
  * More anti-moire fact-finding, isolation of possible Chrome bug with non-even canvases on Retina Macs
    * https://github.com/KhronosGroup/WebGL/issues/587#issuecomment-499648875
  * Up next:
    * More remoting!
    * webgpu-rs review onboarding
    * DMD report of ANGLE shader translator objects not tracked by memory tracking, thus invisible to GC! :(
