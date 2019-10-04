jbonisteel
  * Document from Andreas about how web platform features get prioritized/into Gecko
    * https://docs.google.com/document/d/1DwcfM1chcrGqiJz5tMnfu5oj8Kfeey7dMU0Yq_wxHps/edit 
  * Team H2 Goals
    * https://docs.google.com/spreadsheets/d/10s3243kIzyrT_uLIxzfhJXcmhZYUl7JtN5XGXH6mLis/edit#gid=249668108
  * Goals for the week:
    * Work on Q4 OKRs
    * Gather more feedback from team/stakeholders about 2020 planning
      * Very rough draft doc so far: https://docs.google.com/document/d/1gNHDu-fKhDKw7sLNSrkIQNMnIKv9U16x9kE4795ZrPQ/edit

gw
 - Working towards multi-resolution tiles:
     - https://phabricator.services.mozilla.com/D42473
     - https://phabricator.services.mozilla.com/D42274
     - Both reviewed - fixing up some comments / test failures and getting them landed.
 - Continued some investigations on various driver (?) related bugs on my list.
 - NEXT: Enable picture caching on content + UI slices once the patches above land, see what happens.
 - NEXT: Various picture caching related things I can start on, not totally sure of ordering yet:
        - Enable on multiple content slices (some subpx aa work to do first).
        - Prototype integration with OS compositor (CA / DC).
        - Fix up some cases where picture caching invalidates way too much (high dpi, mobile).
        - Investigate cases where invalidation is happening much more than it seems like it should.

tnikkel
  * reftest fission - getting basic JSWindowActors working in reftest harness
  * img.decode bug 1572360 - pondering how to fix it and stay within spec

sotaro
  * Flickering (Win10 (1903)/Intel HD Graphics 530 + 620) (Bug 1556634)
    * MSFT planning a fix to address this issue
    * Confirmed that Windows insider program(with Fast Ring). But it was for 20H1
    * We do not know yet if the problem is addressed soon by MSFT.
  * Assertion failure at WebRenderImageHost(Bug 1557858):created a patch

jgilbert
  * Ported python2 scripts to python3
  * Wrote up how-to-update ANGLE doc: https://hackmd.io/pWC4XBaHTYGG16a0P3tKgg
    * Will be onboarding miko into updating ANGLE
    * Targeting an ANGLE update in v70
  * Rebasing WebGL remoting branch on central
    * Move-only args for ipdl constructors doesn't seem to be supported anymore, oops!
  * Looking into TensorFlow.js in Worker support without OffscreenCanvas

kris
  * onboarding
  * expenses submitted
  * Looking at how mochitests decide whether to run with webrender or not
