gw:
  * Picture caching work related to dirty rects:
      * Improve how tile clipping works with picture caching - https://phabricator.services.mozilla.com/D44618.
          * Fixed some android zoom bugs.
          * Fixed handling of some picture caching edge cases.
      * Refactor tile dependency comparisons - https://phabricator.services.mozilla.com/D44771.
          * Makes it possible to split / merge an existing primitive dependency list.
      * Add a quadtree for tracking dirty rects in picture cache tiles - https://phabricator.services.mozilla.com/D45287.
          * Merges / splits adaptively to reduce CPU overhead where parts of tiles aren't changing.
      * Fix a video playback regression on Linux / Mac - https://phabricator.services.mozilla.com/D45734.
      * Various test expectation updates on tier2 platforms:
          * https://phabricator.services.mozilla.com/D45735
          * https://phabricator.services.mozilla.com/D45736
          * https://phabricator.services.mozilla.com/D45737
          * https://phabricator.services.mozilla.com/D45795
  * Picture caching work related to enabling multiple slices:
      * Add type-safe polygon anchor to plane-split crate - https://phabricator.services.mozilla.com/D45628.
      * Refactor primitive instance storage into clusters - https://phabricator.services.mozilla.com/D45636.
      * Support annotating primitives with semantic flags - https://phabricator.services.mozilla.com/D45970.
  * Various reviews
  * Investigated CSS Adrianne test not picture caching on Mac.
      * Scroll bars are handled differently on Mac, which is tripped up existing picture cache logic. Fix in progress.
  * NEXT:
      * Try to sort out Berlin travel.
      * Expose dirty rects (for non-scrolling cases) so that Sotaro can experiment with partial present.
      * Continue landing patches to enable multiple slices, which will also handle:
          * Current slow picture caching path on sites with full-size fixed position background image.
          * Mac picture caching invalidation due to scrollbars.
          * Caching of UI slice.
      * Start experimenting and working with Sotaro + Dan on integrating with DirectComposite.

tnikkel
  * reftest fission, got pushing the child layer trees to the parent working! working through a few intermittents left with that. then just need to do the same for flushRendering.
  * reviews
  * apz leak intermittent, trying even more to reproduce, failing (bug 1567448)


sotaro
  * Use DirectComposition for video on Window( Bug 1460499)
    * Mainly did preparation works
    * Start to implement Windows specific part
  * Remove wr::WrExternalImageId(Bug 1581307): Waiting for a review
  * Long weekend

jgilbert
  * WebGL remoting object lifetimes/js wrappers
  * WebGL and WebGPU F2Fs
  * ResizeObserver discussions

kris
  * Completed implementation of logger, just need to improve enabling/disabling (preference is annoying)
  * Trying to get an overview of images vs blob images vs external images
  * Trying to make sense of the many full screen render targets (20+) on some sites
  * Reviewing hackerrank tests for intern positions
  * 
