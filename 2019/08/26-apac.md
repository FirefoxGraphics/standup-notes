jbonisteel:
  * Last week's goals: 
    * work on Q4 OKRs
      * Reasonable draft in place: https://docs.google.com/document/d/1lvGFjGR1ub0xkIaMQ6x7R4UNj151rBz84Zrq123y9MY/edit 
    * gather more feedback from team/stakeholders about 2020 planning
  * This week:
    * Finish headcount doc for product
    * Finally have consensus that Focus can use GV Nightly, push that along so we can enable WR
    * Finish updating the WR roadmap
    * Q4 planning - will want to do that around mid/later September, put together a plan to do that 'remotely'


sotaro
  * Use DirectComposition for WebGL on Window (Bug 1546823)
    * It seems better to use "Partial Invalidation on Windows(Bug 1575159)" instead of this bug.
    * ID3D11DeviceContext::CopyResource and ID3D11DeviceContext::CopySubresourceRegiocould not copy data from WebGL's D3D11Texture2D to SwapBuffer's D3D11Texture2D even when format and size were same.
    * mstange are going to use picture cache tile as native overlay on mac. But it could not be used on Windows. Partial invalidation seems better.
    * I am going to test data copy and color conversion for video. Chromium uses overly only for video.
  * reviews
  * triage
  * Assertion failure in WebRenderImageHost(Bug 1557858): addressed

tnikkel
  * reftest fission - finally have some useful messages being passed to all the relevant processes
  * fixed up a mistake in svg component transfer filters in webrender (bug 1575119)
  * investigating a failure with marionette reftest harness when moving to new fission compatible api (bug 1574935)
  * looking into another ChooseScale wr bug regression (bug 1553571)
