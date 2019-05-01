jbonisteel:
  * Core Objectives for the week:
    * Work on revising Q2 OKRs - some priorities are still being discussed but want to iterate on the wording of my draft so far
    * Finish and share WR triage notes
    * Start revising agenda for work week: please think about anything specific you want to see happen, I'll be talking about this in our 1:1s
      * On that note - if you have not booked travel yet please do so or contact me if you have any questions

gw:
    * Fixed a hit testing bug (1531170). Also refactored and optimized hit testing at the same time.
    * Landed a gradient fast path (1533236). Much faster for the majority of encountered gradients.
    * Investigating profiling on Android.
        * Streamline
        * Mali profiler
        * RenderDoc
        * GAPID
    * Profiling performance on espn.com on mobile.
      * Next: Have ~5 possible fixes / solutions - need to do a bit more profiling, then will start to prototype / implement these.
    * Reviews

sotaro
  * WebGL performance regression with webrender(Bug 1531294): checked-in
    * heavy over production happened during webgl
  * Working for enabling shared gl on android(Bug 1532929)
  * Working for android surface texture handling(Bug 1529870)
  * Fixed frequent empty window with WebRender on wayland
  * Fixed misc bugs

tnikkel
  * RDL android
    * one crash that I'm not sure if RDL or not, can never reproduce when I have a build with crashreporter enabled
    * talked with botond about timing wrt containerless
  * shader compiler fix for component transfer
  * our png code or libpng bug investigating
  * next: continue to make sure RDL android is ready for after merge, fix that png bug

jgilbert:
  * Firefox is now WebGL 1.0.3-compliant!
  * Webgl remoting ongoing, aiming to start landing patches early 68
  * sec bugs! (Ever passed a uint64_t to malloc on 32bit??)
  * Next:
    * Investigate WEBGL_multiview for 68
    * Prep ANGLE update for 68
  * Also, I have a distcc-like running on Windows now! :D
