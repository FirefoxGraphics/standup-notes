Jbonisteel:
  * Friday:
    * Had two interviews for our open req
    * Did a bit of triaging
    * Conversation with svoisen
    * Did my own H2 goals (once my manager approves I will add to shared team doc)
  * Goals for the week:
    * Make sure Kris has a good week in Toronto!
    * Review/approve team's H2 goals

gw
 - Various reviews / meetings / discussions (backdrop-filter, preserve-3d issues, driver bugs).
 - Investigating some hard to repro bugs - not much progress on 1566099, 1565891, 1566178.
 - Meeting with Kris to give a WR overview.
 - Found a Gecko bug causing picture caching issues with non-integer dpi ratios (filed 1572340).
 - Fixed a WR bug causing bad rendering on egencia itineraries - https://phabricator.services.mozilla.com/D41111
    - This exposed an unrelated plane splitting bug - worked with Dzmitry to diagnose and land plane-split update.
    - Got these patches approved and merged to beta.
    - Also fixed some 3d transform bugs on tier2 platforms - https://phabricator.services.mozilla.com/D41493
 - Landed some work towards enabling multiple picture cache slices:
    - https://phabricator.services.mozilla.com/D41342
    - https://phabricator.services.mozilla.com/D40916
 - NEXT:
     - Continue on multiple picture cache slice work.
     - Continue trying to make progress on the hard-to-repro bugs above.
     - Sort out some H2 goals.
     - Public holiday in Brisbane tomorrow (Wednesday) for Ekka day.

tnikkel
  * another img.decode bug (bug 1572360)
  * starting on reftest harness fission work
  * fixing first paint telemetry, review hell, pushing forward slowly
  * img.decode hashtable asserts that I get sometimes, haven't filed bug yet

sotaro
  * Flickering selection/text input and jumpy scrolling (Win10 (1903)/Intel HD Graphics 530 + 620)(Bug 1556634)
    * The poroblem happened also on google chrome by disabling partial swap
    * DXGI_ALPHA_MODE_PREMULTIPLIED usage seems to be relatively low risk patch. But it regress performance in some cases. 
  * Tabs bar is broken when a high contrast theme is activated(Bug 1570879)
    * Compositor window usage caused the problem.
    * When native theme was used, TabsInTitlebar background color was transparent
    * It exposed windows background color
    * When Compositor window usage changed windows background color.
    * TabsInTitlebar needs to render by using explicit color.
    * Component was changed to Theme
  * Canvas redraw doesn't update on screen after made hidden, then visible(Bug 1569724):Merged to m-c
