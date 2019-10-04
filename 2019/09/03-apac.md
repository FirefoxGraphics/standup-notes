gw
 * Going around in circles trying to get picture caching enabled on multiple slices (still). The patches are reasonably
    simple, however I have run into 3-4 issues causing test failures. They are existing and/or unrelated issues, that get
    exposed when multiple content slices are enabled. Usually I can work around these by making WR changes, but some
    of these may require changes to how Gecko supplies the DL to WR. I have a good understanding of the problems now,
    but still unsure of the "right" solution, so planning to investigate some of the Gecko-side code today and come
    up with a plan to get these resolved.
