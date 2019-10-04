jbonisteel
Goals for the week:
  * Finish putting together retrospective
  * 2-pager on "wins" we expect from WR on Android
  * Interview more
  * Prep for some q4 planning sessions
  * Heads up: I am out of the office next week M-W for training.

tnikkel
  * leak in apz tests, trying to reproduce locally, failing (bug 1567448)
  * reftest fission stuff, progress being made
  * investigating bug 1579173, turned out to be hitting surface cache limit. resurrected bug 1284651 to increase that.

sotaro
  * Looked into DirectComposition usage on Windows(Bug 1460499,  Bug 1479786,  Bug 1546823, Bug 1550029)
  * DirectComposition sync meeting
    * Put off document splitting for now. It still has problems to address.
    * We need "Partial Invalidation on Windows(Bug 1575159)"
    * Work for video direct composition at first
  * Remove workaround of flickering with intel GPU (Bug 1578605)
    * Fix of flickering was release by MS via Windows update

gw
 - Landing bits and pieces of the dirty rect support for picture caching:
     - https://phabricator.services.mozilla.com/D44771
     - https://phabricator.services.mozilla.com/D44618
     - https://phabricator.services.mozilla.com/D44436
 - Have dirty rects working locally.
  - Have a couple test failures to resolve today.
  - Need to tidy up the patch, then put up for review.
  - Talos shows some nice perf wins from try runs.
  
kris:
    Friday:
    * Addressed comments for bug 1571977 (texture rect reftest), one open discussion point
    * Looked into enabling webrender for drawWindow, requested info from sotaro 
    to see why this is specifically disabled,
    * Monitor RMA
    * Git - windows issues
  Today:
    * Look into other way to create iframe reftest captures using seperate windows
    * Look into adding pixel drawcount metrics for rasterized blob images.
   

jgilbert:
  * webgl remoting
  * webgpu prep for f2f week-after-next
  * miko landed an ANGLE update for 71
  * gpu switching thrashing on google maps
  * Will be updating webgl conformance tests checkout
  * ResizeObserver and device-pixel-box discussions with Google
