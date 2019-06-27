tnikkel
  * finally figured out root cause of bug 1556687. flooding main thread with paints in an edge case our existing paint throttling doesn't catch
  * next: fix firstpaint (bug 1556568)
  * think on parent rdl regression caused by bug 1534549
  * hopefully write a relatively quick fix that 85% solves bug 919113

jgilbert
  * How do we keep WebGL from keeping the dGPU active on Mac?
    * 

sotaro
  * Fallback from WebRender to Compositor on andorid(Bug 1533296):Fixed
  * Don't trigger composites on out-of-viewport texture updates: Going to ask review.
  * Fixed crash bugs(Bug 1546192, Bug 1547760)
  * Triage
  * Documentation work related to changing contract in Japan
