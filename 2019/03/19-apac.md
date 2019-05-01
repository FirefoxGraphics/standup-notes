jbonisteel
  * Objectives for the week:
    * Work week schedule (I am probably overthinking it a little at this point...)
    * Add Q2 OKRs to our doc https://docs.google.com/spreadsheets/d/1zAoLoqEFUDHmF20Lqy4Y0BI8aQoWizhXXdcpy3ghuZk/edit#gid=0
    * Survive my first week doing GFX triage!
    * Quick update re: Q1 OKRs
    * Also reminder: if you are coming to All Hands, book travel by the 22nd!

gw
 * Done:
     * Profiled performance on Mali devices. Wrote up document and bugs with fixes for these.
     * Started work on making existing picture caching work on mobile - https://phabricator.services.mozilla.com/D23633
     * Experimented with pixel local storage on mobile for clip tasks - promising results so far!
     * Started landing some work related to PLS - https://phabricator.services.mozilla.com/D23271
     * Optimized clip mask rendering for common cases - https://phabricator.services.mozilla.com/D23817
     * Investigated some other options to reduce size of clip mask allocations on mobile.
 * Next:
     * Implement functionality needed to enable PLS rendering path on mobile devices.
     * Add code path for clip masks that make use of PLS.
     * Continue investigating current picture caching issue(s) on mobile.

Sotaro
  * Enable SharedGL on android(Bug 1532929): Waiting for review
  * Re-enable SurfaceFactory_EGLImage usage with WebRender on android(Bug 1532201): Started to work
  * Checked in misc patches
  * Did urgent help

jgilbert
  * webgl remoting work ongoing
  * prepping ANGLE update
    * Likely end of this week, depending on blockers
  * Misc webgl sec-bugs
  * Going to add a web console warning when webgl apps unportably rely on implicitly-activate extensions
  * Burning down stale assigned bugs, needinfos, and unprioritized webgl component bugs

tnikkel
  * enabling RDL in the parent process - debugging/fixing issues with that
