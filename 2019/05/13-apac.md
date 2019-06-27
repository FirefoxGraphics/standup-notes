Jbonisteel
	* Worked on WR blog post quite a bit
	* Attempted starting Q3 OKRs
	* Did more wrangling/discussing work around Android, shipping on more desktop
Goals for this week
	* Probably need to make more progress on Q3 OKRs (for real this time)
	* Finish off the blog post after sharing with vp/cto
	* WR intel wrangling


sotaro
	* Catch up
	* GL security bug: going to aply a review comment.
	* Fixed Intermittent failure(Bug 1536668)
	* Found and looked into  D3D compositor regression(Bug 1549674)
		* bas addressed the bug
	* Found and looked into wayland bug(Bug 1550658)
		* Martin Stránský addressed the bug
	* Did reviews
	* Started to work "Document based partial present"(Bug 1550029)

gw
 * Fix a crash bug in 68 when Gecko supplies non-existent image keys (https://phabricator.services.mozilla.com/D30560)
 * Picture caching improvements:
  * Create render task graph earlier during frame (https://phabricator.services.mozilla.com/D29994)
  * Refactor batch building for multiple batches / targets per picture (https://phabricator.services.mozilla.com/D30330)
 * Review transform flattening, border fix patches.
 * Next:
   * Try to finish up and land multiple batches per picture, which unblocks stage 1/2 of the picture caching work.

tnikkel
	* sick all last week :(
	* the imglib patch that I thought was a perf win, then turned out not to be. Turns out it does improve things after all. smaug told me to try it on speedindex, which only a few people are running locally, it was a win there.
	* debugged/patched bug 1547277, extension popups frequently being blank
	* bug 1530190, icon channel spinning the event loop at bad times, noticed a couple minor issues with existing patch, need to fix, write a test, and land and finally be rid of this bug.
	* looked at RDL telemetry on android. avg case stayed about the same, but matt landed some general RDL improvements a couple weeks after android RDL was enabled and that definitely improved the avg case. The 95% case got ever so slightly worse. Matt had a simple idea to try to avoid that maybe, need to write that patch.
	* hopefully can finally look more into parent rdl once i wrap that stuff up.

jgilbert
	* webgl remoting integration
	* angle sec fixes
	* webgl and webgpu F2F this week
		* Writing webgpu multiqueue proposal for
		* webgl multiview moving forward
			* Should get this on Windows and Android in 69
		* webgl video textures/zero copy discussions
		* webgl non-blocking "parallel" shader linking in Gecko
			* Should get this on Windows (where it's most needed) in 69
		* (mostly webgl) color space discussions: highp/hdr backbuffers
	* webgpu integration into Gecko
