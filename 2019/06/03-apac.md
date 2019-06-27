jbonisteel
  * Friday:
    * A handful of meetings, following up on some sec bugs, talking to Jeff before his leave
  * Goals this week:
    * Keep an eye on WR bugs 
      * This bug is concerning me a bit, seems to not be terribly reproducable so far: https://bugzilla.mozilla.org/show_bug.cgi?id=1556106
        * If others can try reproducing it too - that would be swell
    * Self-assessment 
  * Heads up:
    * I have to take a half-day PTO on Thursday afternoon
    * Technically supposed to be at a conference on Friday, but might change my mind depending on how the week goes

gw
  * (Still) picture caching improvements.
  * Got reftests passing, performance is looking good in most cases.
  * Currently working on tidying up patches, try run(s), and one optimization that should fix the common case that is a bit slow.

sotaro
  * Heavy flickering of WebGL background(Bug 1555544): Addressed on m-c
    * The site is recreating the canvas on every frame.
    * TextureClient needs to be alive until host side opens D3D11Texture2D from handle
  * Make D3D11TextureData and DXGIYCbCrTextureData alive during host side usage with WebRender(Bug 1556340): Waiting for review.
    * It is a possible fix that is similar to Bug 1555544.
  * Don't trigger composites on out-of-viewport texture updates(Bug 1531898): Waiting for review
  * Building with --disable-printing is broken(Bug 1537586): passed review, going to update
  * Looked into chromium's android implementation
    * https://bugzilla.mozilla.org/show_bug.cgi?id=1529629#c2
    * On recent android, AHardwareBuffer could be used as android::GraphicBuffer.
    * Implementation for Android Q already exists.
    * From Android Q, ASurfaceTransaction is going to be added.
    * ASurfaceTransaction_setBuffer() seemed to be used for overlay.
  * Helped Tokyo office relocation

tnikkel
  * handle glass item for parent RDL - several iterations and landed (bug 1554373)
  * firstPaint regression with webrender (bug 1546140)
    * looked at a bunch of invididual telemetry pings to try to figure out what was going on
    * eventually figured out how we measure firstPaint is totally broken, likely no actually regression
  * next: likely look into bug 1554149, hopefully improves perf for parent rdl because there were reports of regressions last time it was enabled

jgilbert
  * Sec bugs!
  * Dynamic indexing of samplers in GLSL on Linux
  * WebGPU PRs/proposals
  * Merging improvements into our WIP remote-webgl branch
  * Onboarding into the webgpu-rs codebase
