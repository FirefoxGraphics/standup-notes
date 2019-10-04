gw
 - Mostly working on https://bugzilla.mozilla.org/show_bug.cgi?id=1562462
  - We seem to have a workaround now. Landed in m-c, beta uplift request has been made.
 - Various WR reviews.
 - Some review / discussions of backdrop-filter WIP patches.
 - Rebasing / reworking some of the patches for multi-resolution / dirty regions in picture cache tiles.
 - Testing / investigating https://bugzilla.mozilla.org/show_bug.cgi?id=1566099 and https://bugzilla.mozilla.org/show_bug.cgi?id=1566178

sotaro
  * Investigate a workaroud for Flickering selection/text input(Win10 (1903)/Intel HD Graphics 530 + 620)(Bug 1569881):Investigated another workaround
    * All workarounds regressed performance
  * document splitting: Failed to lock ExternalImage error(Bug 1570593):Addressed
  * Call ScheduleForcedGenerateFrame() in WebRenderBridgeParent::RecvScheduleComposite()(Bug 1571331): Addressed
  * Crash in [@ nsBaseWidget::CreateCompositor](Bug 1569565):Addressed
  * Canvas redraw doesn't update on screen after made hidden, then visible(Bug 1569724): Passed review

gankro
  * trying to reproduce this user's issue with webrender being unusable slow on beta (windows)
