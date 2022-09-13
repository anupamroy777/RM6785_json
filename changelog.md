## Build Information
```
Kernel: ThunderStorm Kernel
Device: Realme Unified 7/6/6i/N20Pro/N30
Type: Stable
Compiler: Azure Clang 15
Build Number: TS2.2
```
## Changelog
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
