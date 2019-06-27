https://public.etherpad-mozilla.org/p/GFXWhistler19plans

jbonisteel
Goals for this week:
  * help prioritize anything that may come up for WR
  * get organized for intern svg filter project
  * check up on doc splitting progress 
  * start thinking about onboarding  

sotaro
  * Remove WrExternalImageBufferType(Bug 1554091)
    * Use wr::ExternalImageType directly at ffi.
    * Pass wr::ExternalImageType by value at ffi caused a crash on non-Window platform. Stack seemed to be broken.
    * Pass wr::ExternalImageType by reference at ffi could bypass the crash
  * Don't trigger composites on out-of-viewport texture updates(Bug 1531898)
    * Gong to start review. Waiting Bug 1554091 fix.
    * Waiting Bug 1554091 fix
  * Document based partial present(Bug 1550029)
    * Still have a flicker problem.
    * It seems that we need to clipe rendering update
  * av1 video playback does not use fast path on Windows(Bug 1552734): Landed to m-c
  * DirectComposition based document compositor(Bug 1479786) : Started to work

tnikkel
  * finally landed icon channel bug (bug 1530190)
  * landed a fix for parent rdl (bug 1552104)
  * need to rework patch for glass item handling (Windows effect) for parent rdl (bug 1554373)
next
  * issue where two documents use the same image forces us to revalidate when we shouldnt because of imgcache limitations keeps coming up (bug 1553923), there is probably a quick fix we can do to fix 95% of the problem
  * parent rdl potential perf regression investigation

gw
  * Various reviews
  * Mostly focused on picture caching work.
    * Running now in Gecko with some glitches and a couple missing features.
    * Hoping to work on those today / tomorrow.
    * Will be aiming to land some smaller parts of those as isolated work while starting to work through any try run issues.
    
