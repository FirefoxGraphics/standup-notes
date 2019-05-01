Tuesday Feb 19th - APAC/PST Weekly Sync - Notes!

sotaro
  * Enabled WebRenderTextureHostWrapper for canvas
    * Improved glterrain on windows10-64-qr better than on windows10-64.
  * Wroked for security bugs.
  * Worked for wayland with WebRender bugs

gw
 * Investigations related to snapping and local scale / animations - fix is https://phabricator.services.mozilla.com/D20276
 * Found Win/ANGLE seems much slower at picture cache blits - planning to investigate further.
 * Discussions with kats + matt about scroll offsets, normalizing coords. This may simplify picture caching a lot.
 * Profiling + optimization ideas for low-end integrated gfx + 4k.

tnikkel
* reviews
* cleaning up component transfer webrender patches for review after interning overhaul

