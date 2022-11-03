## Build Information
```
Kernel: ThunderStorm Kernel
Device: Realme Unified 7/6/6i/N20Pro/N30
Type: Stable
Compiler: Neutron Clang 16
Build Number: TS2.3
```
## Changelog
**TS2.3-MGlru**
* Revert mediatek bpf changes
* Disable slmk
* mglru backports(multi generational lru)
* implemented UKSM(ultra kernel samepage merging)
* Introduced cpu_input_boost driver(you can access via /sys/module/cpu_input_boost/parameters)
* cib: boost on power key
* Upstreamed to 4.14.296
* Disable MTKPTPOD (it's for dynamic voltage control)
* set initial TCP window size to 64K (speed improvement)
* Tcp_congestion: Switched to bbr
* Introduce ThunderQuake Engine
* switched to azure clang 15 (bcs of some environment issues i had to switch from neutron clang 16 neutron clang will be back in next update)
* Imported r36p0 gpu from begonia
* Added drivedroid support

**TS2.2**
* Upstreamed to 292
* Switched to simple low memory killer(slmk)
* Silenced few logs
* Switched to Neutron clang 16
* Disable MTK sched enhancement
* Affine GPU IRQs to big cluster CPUS

**TS2.1-hotfix**
* Fix Ipv6 Tethering

**TS2.1**
* Upstreamed To 286
* zsmalloc backports
* mm/vmscan.c: swappiness set to 45
* Introduce kernelspace battery saver mode
* disabled few debuggings
* silenced few logspams
* cpumask: Add cpumasks for big and LITTLE CPU clusters
* fpc1022: Affine IRQs to big CPU
* touchscreen: affine touchscreen to big cpu
* wakelock: Add a timeout to wakelocks globally
* unix backports
* time: Disable timer migration
* sched: Reduce latency for better responsiveness
* Switch To step_wise Thermal Governor
* Enable HW_RANDOM
