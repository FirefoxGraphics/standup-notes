jbonisteel
  * Goal for the week:
    * Do triage
    * Write OKR status update
    * Draft H2 Goals
  * On PTO Weds-Weds
  * Monday Aug 5th is a holiday in Canada

sotaro
  * Crash in rx::ProgramD3D::load(Bug 1567620): Addressed
    * Obsoleted program binary was loaded
  * Crash in mozilla::layers::AsyncImagePipelineManager::UpdateImageKeys()(Bug 1567737):Addressed
  * Add ClientLayerManager::Initialize()(Bug 1569110):Merged to m-c
    * Clean up initialization code
  * Flash is broken with wmode=gpu and WebRender(Bug 1565980):Looked into
    * Caused by compositor window usage.
    * :jrmuizel addressed the bug
  * Picture-in-Picture flickering (Bug 1557994):Looked into
    * 2 video sink sent video frames to one VideoFrameContainer.
    * :mconley is working for it

gw
 - Stuck in an infinite loop on https://bugzilla.mozilla.org/show_bug.cgi?id=1562462
 - Various reviews
 - Uplifted a couple of fixes to beta
 
 tnikkel
  * bug 1567535/bug 1565542 img.decode() promise never resolving causing google maps to not draw sometimes
  * bug 1568655 crash in imagecachekey null check fix
  * bug 1565922 document viewer crash fix might also fix bug 1561104
  * bug 1562184 windows 7 glass fix for parent rdl
  * fiddled with composition recorder stuff but got nowhere (bug 1566203, bug 1565225, bug 1566915)
 
jgilbert
  * WebGL remoting! (again again)
  * WebGL test perma-orange when adding preceeding guard page to allocations
    * https://bugzilla.mozilla.org/show_bug.cgi?id=1546442
  * Discussions with W3C CSS WG about ResizeObserver and device pixel rects
  * Considering ANGLE update this cycle for 70 (last update was 68)
  * Got some Unity demo/benchmarks from Jukka
    * Landed some minor optimizations (1-2%) to help (VAO mutation revalidation)
    * Asked if they can use VAOs on their WebGL backend ("maybe, we use them (some?) on the es31 backend")
    * Firefox has really inconistent frame times compared to Chrome
      * Firefox has better median times, but worse 90th-percentile spikes every 4-ish frames
      * Smoothness is a goal here, so I'm looking into it a bit
  * Updated the graphics hardware inventory wiki page with my various GPUs and machines
