jbonisteel
  * Shared Q3 OKRs, updated triage schedule, had many conversations about Android
  * Goals for this week:
    * Finish my onboarding docs, which I didn't really get to last week
    * Write proposal for WebRender A/B test we eventually want to do on Android 
    * Kick-off recruitment for new req

gw
 * PTO last week
 * Catching up on email / reviews / bugzilla
 * Next: Continuing work on https://phabricator.services.mozilla.com/D36711 - causes some Talos regressions
 * Next: Build on patch above to support smaller dirty rects / multi-resolution tiles.
 * Next: Try to work out what's going on with:
     https://bugzilla.mozilla.org/show_bug.cgi?id=1566178
     https://bugzilla.mozilla.org/show_bug.cgi?id=1541072#c19
     https://bugzilla.mozilla.org/show_bug.cgi?id=1565473#c3
     (seem to all be related - not sure if they are the same / how easy they are to reproduce etc )
 * Next: More investigation of SwiftShader / llvmpipe etc

tnikkel
  * new parent rdl regressions came in this week
    * browsertime + webrender broken (bug 1565225)
    * reproducible crash (bug 1565922)
    * Windows glass effect glitch (bug 1562184)
  * need to finish up fixing firstpaint telemetry patch
  * triaging

jgilbert
  * WebGL remoting
    * Kill PWebGL on context loss
    * Infer IPC sync/async from return type
  * Potential fix for crash on macOS disconnection of external monitor
  * Todo: Multi-queue proposal for WebGPU
  * Fix blocklisting of GMA4500
    * D3D11 support there is bad, so we were supposed to be on D3D9, but that logic got interrupted in the ANGLE update in Fx60

sotaro
  * Crash with mozilla::ipc::IProtocol::HandleFatalError(Bug 1562616): Analyzed the crash and found a possible cause of the crash.
    * Matt Woodrow addressed the crash.
  * Don't trigger composites on out-of-viewport external image updates(Bug 1564646): Waiting for review
  * Add ImageBorder image key to Tile(Bug 1565463): Merged to m-c
  * Skip WR rendering until window becomes ready to draw on Wayland(Bug 1565785): Review passed
  * Remove ID3D11Device::GetDeviceRemovedReason() call from RenderCompositorANGLE::BeginFrame()(Bug 1563432): Merged to m-c
  * Disable double buffering with compositor when device reset happens(Bug 1562847): Merged to m-c
  * Battery: Don't trigger composites on out-of-viewport native texture image updates(Bug 1531898): Merged to m-c
  * Fallback from WebRender when EGLSurface creation failed in RenderCompositorEGL::BeginFrame()(Bug 1564720):merged to m-c
