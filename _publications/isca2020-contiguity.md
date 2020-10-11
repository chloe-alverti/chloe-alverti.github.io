---
title: Enhancing and Exploiting Contiguity for Fast Memory Virtualization
collection: publications
---
<p style="color:black;font-size:16px;"> Chloe Alverti, Stratos Psomadakis, Vasileios Karakostas, Jayneel Gandhi, 
Konstantinos Nikas,<br/>Georgios Goumas, and Nectarios Koziris
<br/>Published in <i>47th International Conference on Computer Architecture (ISCA)</i>, 2020 </p>
We propose synergistic software and hardware mechanisms that alleviate the address translation overhead, focusing particularly on virtualized execution.
On the software side, we propose contiguity-aware (CA) paging, a novel physical memory allocation technique that creates larger-than-a-page contiguous mappings while preserving the flexibility of demand paging. 
CA paging applies to the hypervisor and guest OS memory manager independently, as well as to native systems. 
Moreover, CA paging benefits any address translation scheme that leverages contiguous mappings.
On the hardware side, we propose SpOT, a simple micro-architectural mechanism to hide TLB miss latency by exploiting the regularity of large contiguous mappings to predict address translations
in both native and virtualized systems.
We implement and emulate the proposed techniques for the x86-64 architecture in Linux and KVM, and evaluate them across a variety of memory-intensive workloads. Our results show that: (i) CA paging is highly effective at creating vast contiguous mappings,
even when memory is fragmented, and (ii) SpOT exploits the created contiguity and reduces address translation overhead of nested paging from 16.5% to 0.9%.

keywords: virtual memory, virtualization, memory management, contiguous page mappings

[[code]](https://github.com/cslab-ntua/contiguity-isca2020) 
[[pdf]](https://cslab.ece.ntua.gr/~xalverti/papers/isca20_enhancing_and_exploiting_contiguity.pdf) 
[[pptx]](https://cslab.ece.ntua.gr/~xalverti/papers/isca20_enhancing_and_exploiting_contiguity.pptx) 
[[video]](https://www.youtube.com/watch?v=njCazqLIBbc&ab_channel=chloialverti)
