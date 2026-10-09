# Prioritizing Maritime Starlink Traffic for Commercial Fishing Vessels

A CSC 466 research project exploring whether smart edge queue management can protect
essential vessel operations on Starlink while allowing crew use the network.

**Live site:** https://rowanhall.github.io/starlink-maritime-prioritization/

**Team:** Jasper McLennan, Rowan Hall 
**Course:** CSC 466, University of Victoria

## The Problem

Commercial fishing vessels increasingly depend on Starlink for both essential operations
and crew welfare. When off-shift crew use high-bandwidth apps (video streaming, cloud
backups), the shared uplink saturates and suffers **bufferbloat** 

This causes latency spikes that can disrupt critical bridge traffic and vessel telematics. 
This causes operators to restrict crew to messaging and light browsing to
avoid interfering with essential ship operations. Having experience in the fishing industry, we
have lived this trade-off firsthand.

## Our Approach

We want to replace that policy with **edge traffic prioritization and Active Queue
Management** (e.g. FQ-CoDel / CAKE, or dynamic rate-limiting) tuned to Starlink's fluctuating
capacity. Our goal is to let queue management automatically protect necessary operational traffic, allowing
crew to use the network without risk.

## Plan

1. **Benchmark & test locally** — measure baseline latency under load and compare queueing/QoS
   policies on a controlled testbed (possibly using UVic's Starlink setup).
2. **Deploy on a real vessel** — run the most promising configuration on an edge
   gateway/router connected to an active vessel terminal and measure real-world improvement
   under crew load.

## This Repository

Static website hosted on GitHub Pages