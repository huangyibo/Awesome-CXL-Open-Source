# Awesome CXL Papers and Open-Source Artifacts
 *Hope that you'd be happy to add a star if you think this list is helpful!*

## Overview

- [Hardware, Architecture, and Characterization](#hardware-architecture-and-characterization)
- [Memory Pooling, Disaggregation, and Virtualization](#memory-pooling-disaggregation-and-virtualization)
- [Tiered-Memory Management and Page Migration](#tiered-memory-management-and-page-migration)
- [Communication Frameworks, Shared Memory, and Common Libraries](#communication-frameworks-shared-memory-and-common-libraries)
- [Machine Learning, Recommendation, and Near-Memory Processing](#machine-learning-recommendation-and-near-memory-processing)
- [Databases, Transactions, and Key-Value Stores](#databases-transactions-and-key-value-stores)
- [Storage, Shared Logs, and CXL SSDs](#storage-shared-logs-and-cxl-ssds)
- [Coherence, Programming Models, and Verification](#coherence-programming-models-and-verification)
- [Security, Reliability, and Failure Recovery](#security-reliability-and-failure-recovery)
- [Simulation and Emulation Infrastructure](#simulation-and-emulation-infrastructure)
- [Supplementary Papers from Other Venues and Workshops](#supplementary-papers-from-other-venues-and-workshops)
- [Related PCIe Interconnect Work](#related-pcie-interconnect-work)
- [Blogs on CXL](#blogs-on-cxl)


## Hardware, Architecture, and Characterization

- Vistara: Making CXL Real—Full Path from ASIC Design and OS Support to Hyperscale Deployment **(ISCA 2026, industry)** --- [paper](https://aisystemcodesign.github.io/papers/isca26/vistara_camera_ready.pdf).
- A Silicon-Proven Unified Low-Latency CXL Controller and Port-Based Routing Switch for Memory-Centric Fabrics **(ISCA 2026, industry)** --- [paper page](https://www.iscaconf.org/isca2026/program/).
- 🔓 Rethinking Compression for CXL Memory Expanders at Hyperscale **(MICRO 2026)** --- [paper page](https://haneulpark.me/pubs/rethinking-compression.html) [github](https://github.com/google-systems-research/cold-memory-model).
- Finding NEMO: Nimble and Expressive Memory Observability **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-li-shihang.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-li_shihang.pdf).
- 🔓 Systematic CXL Memory Characterization and Performance Analysis at Scale **(ASPLOS 2025)** --- [paper](https://huaicheng.github.io/p/asplos25-melody.pdf) [github](https://github.com/MoatLab/Melody) [slides](https://huaicheng.github.io/s/asplos25-melody-slides.pdf).
- 🔓 Understanding and Profiling CXL.mem Using PathFinder **(SIGCOMM 2025)** --- [paper](https://pages.cs.wisc.edu/~mgliu/papers/pathfinder-sigcomm25.pdf) [github](https://github.com/netlab-wisconsin/PathFinder).
- 🔓 CXL-Interplay: Unraveling and Characterizing CXL Interference in Modern Computer Systems **(DAC 2025)** --- [paper](https://www.thu-haslab.org/publication/2025-cxl-interplay/dac2025cxl-interplay.pdf) [github](https://github.com/THU-HAS/CXL-Interplay).
- Demystifying a CXL Type-2 Device: A Heterogeneous Cooperative Computing Perspective **(MICRO 2024)** --- [paper page](https://doi.org/10.1109/MICRO61859.2024.00110).
- 🔓 Exploring Performance and Cost Optimization with ASIC-Based CXL Memory **(EuroSys 2024)** --- [paper page](https://doi.org/10.1145/3627703.3650061) [github](https://github.com/bytedance/eurosys24-artifacts).
- COAXIAL: A CXL-Centric Memory System for Scalable Servers **(SC 2024)** --- [paper](https://faculty.cc.gatech.edu/~adaglis/files/papers/coaxial_sc24.pdf).
- 🔓 Demystifying CXL Memory with Genuine CXL-Ready Systems and Devices **(MICRO 2023)** --- [paper](https://tianyin.github.io/pub/cxl-mem.pdf) [github](https://github.com/ece-fast-lab/cxl_type3_tests).
- DRAM Translation Layer: Software-Transparent DRAM Power Savings for Disaggregated Memory **(ISCA 2023)** --- [paper](https://haneulpark.me/papers/isca23_DTL.pdf).

## Memory Pooling, Disaggregation, and Virtualization

- Break On Through to the Other Side: Pooling Memory Elastically with RamRyder **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-zhou-yanbo.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-zhou_yanbo.pdf).
- Blowfish: Elastic Virtual Machine Memory for Disaggregated Memory **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-zhang-yulong.pdf).
- 🔓 Octopus: Enhancing CXL Memory Pods via Sparse Topology **(NSDI 2026)** --- [paper](https://www.usenix.org/system/files/nsdi26-zhong.pdf) [github](https://github.com/yuhong-zhong/Octopus-CXL-Pod) [slides](https://www.usenix.org/system/files/nsdi26_slides-zhong.pdf).
- FM2: Fast Live VM Migration in CXL Memory Pools **(ATC 2026, accepted)** --- [paper page](https://sigops.org/s/conferences/atc/2026/accepted.html).
- 🔓 Oasis: Pooling PCIe Devices Over CXL to Boost Utilization **(SOSP 2025)** --- [paper](https://www.yuhong-zhong.com/papers/Oasis_SOSP25.pdf) [code—Bitbucket](https://bitbucket.org/yuhong_zhong/oasis) [slides—PPTX](https://www.yuhong-zhong.com/slides/Oasis_SOSP25.pptx).
- DRack: A CXL-Disaggregated Rack Architecture to Boost Inter-Rack Communication **(ATC 2025)** --- [paper](https://www.usenix.org/system/files/atc25-zhang-xu.pdf) [slides](https://www.usenix.org/sites/default/files/conference/protected-files/atc25_slides-zhang_xu.pdf).
- 🔓 Managing Memory Tiers with CXL in Virtualized Environments **(OSDI 2024)** --- [paper](https://www.usenix.org/system/files/osdi24-zhong-yuhong.pdf) [code—Bitbucket](https://bitbucket.org/yuhong_zhong/memstrata/src/master/) [slides](https://www.usenix.org/system/files/osdi24_slides-zhong-yuhong.pdf).
- 🔓 Pond: CXL-Based Memory Pooling Systems for Cloud Platforms **(ASPLOS 2023)** --- [paper](https://huaicheng.github.io/p/asplos23-pond.pdf) [github](https://github.com/MoatLab/Pond) [slides](https://huaicheng.github.io/s/asplos23-pond-slides.pdf).
- Direct Access, High-Performance Memory Disaggregation with DirectCXL **(ATC 2022)** --- [paper](https://www.usenix.org/system/files/atc22-gouk.pdf).

## Tiered-Memory Management and Page Migration

- Tierce: Observability-Driven Tiered Memory Management for Colocated Workloads **(SOSP 2026)** --- [paper](https://huaicheng.github.io/p/sosp26-tierce.pdf) [slides](https://huaicheng.github.io/s/sosp26-tierce-slides.pdf).
- MAC: Metadata Acceleration for Sustainable Performance in Big-Data Systems with CXL DRAM **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-lee.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-lee.pdf).
- Harvesting Sub-Microsecond CXL Memory Stalls with LiteSwitch **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-li-nanqinqin.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-li_nanqinqin.pdf).
- 🔓 ARC: Adaptive Reconfigurable CXL Hotness Monitoring **(MICRO 2026)** --- [paper page](https://www.microarch.org/micro59/program/) [github](https://github.com/ece-fast-lab/MICRO-2026-ARC).
- HYDRA: Hybrid DRAM Caching for Dynamic Complementary Multi-to-One Page Mapping in CXL Tiered Memory **(MICRO 2026)** --- [paper](https://ghuang14.github.io/files/hydra2026micro.pdf).
- 🔓 PACT: A Criticality-First Design for Tiered Memory **(ASPLOS 2026)** --- [paper](https://huaicheng.github.io/p/asplos26-pact.pdf) [github](https://github.com/MoatLab/PACT) [slides](https://huaicheng.github.io/s/asplos26-pact-slides.pdf).
- 🔓 Performance Predictability in Heterogeneous Memory **(ASPLOS 2026)** --- [paper](https://huaicheng.github.io/p/asplos26-camp.pdf) [github](https://github.com/MoatLab/CAMP) [slides](https://huaicheng.github.io/s/asplos26-camp-slides.pdf).
- PIPM: Partial and Incremental Page Migration for Multi-host CXL Disaggregated Shared Memory **(ASPLOS 2026)** --- [paper](https://ghuang14.github.io/files/pipm2026asplos.pdf).
- 🔓 MTTM: Dynamic Fast Memory Partitioning with Bandwidth Optimization for Multi-tenant Cloud **(EuroSys 2026)** --- [paper page](https://doi.org/10.1145/3767295.3769371) [github](https://github.com/casys-kaist/MTTM_ae_EuroSys26).
- TPage: Transparent Page Management for CXL-Based Tiered Memory Systems **(SC 2026, forthcoming)** --- [paper page](https://sc26.conference-program.com/presentation/?id=pap550&sess=sess232).
- 🔓 Demeter: A Scalable and Elastic Tiered Memory Solution for Virtualized Cloud via Guest Delegation **(SOSP 2025)** --- [paper page](https://doi.org/10.1145/3731569.3764801) [github](https://github.com/vtta/sosp25-demeter).
- 🔓 Tiered Memory Management Beyond Hotness **(OSDI 2025)** --- [paper](https://huaicheng.github.io/p/osdi25-soaralto.pdf) [github](https://github.com/MoatLab/SoarAlto) [slides](https://huaicheng.github.io/s/osdi25-soaralto-slides.pdf).
- 🔓 M5: Mastering Page Migration and Memory Management for CXL-based Tiered Memory Systems **(ASPLOS 2025)** --- [paper](https://tianyin.github.io/pub/m5.pdf) [github](https://github.com/ece-fast-lab/ASPLOS-2025-M5).
- 🔓 HybridTier: An Adaptive and Lightweight CXL-Memory Tiering System **(ASPLOS 2025)** --- [paper](https://www.sihangliu.com/docs/hybridtier_asplos25.pdf) [github](https://github.com/kevins981/hybridtier-asplos25-artifact).
- 🔓 DSA-2LM: A CPU-Free Tiered Memory Architecture with Intel DSA **(ATC 2025)** --- [paper](https://www.usenix.org/system/files/atc25-liu-ruili.pdf) [github](https://github.com/madsys-dev/DSA-2LM).
- 🔓 Tiered Memory Management: Access Latency is the Key! **(SOSP 2024)** --- [paper](https://www.cs.cornell.edu/~ragarwal/pubs/colloid.pdf) [github](https://github.com/host-architecture/colloid).
- 🔓 Nomad: Non-Exclusive Memory Tiering via Transactional Page Migration **(OSDI 2024)** --- [paper](https://www.usenix.org/system/files/osdi24-xiang.pdf) [github](https://github.com/lingfenghsiang/Nomad) [slides](https://www.usenix.org/system/files/osdi24_slides-xiang.pdf).
- MTM: Rethinking Memory Profiling and Migration for Multi-Tiered Large Memory **(EuroSys 2024)** --- [paper](https://pasalabs.org/papers/2024/Eurosys24_M3_Camera_Ready.pdf).
- FBMM: Making Memory Management Extensible With Filesystems **(ATC 2024)** --- [paper](https://www.usenix.org/system/files/atc24-tabatabai.pdf).
- FlexMem: Adaptive Page Profiling and Migration for Tiered Memory **(ATC 2024)** --- [paper](https://www.usenix.org/system/files/atc24-xu-dong.pdf).
- 🔓 MEMTIS: Efficient Memory Tiering with Dynamic Page Classification and Page Size Determination **(SOSP 2023)** --- [paper](https://cosmoss-jigu.github.io/pages/pubs/memtis-lee-sosp23.pdf) [github](https://github.com/cosmoss-jigu/memtis).
- TPP: Transparent Page Placement for CXL-Enabled Tiered-Memory **(ASPLOS 2023)** --- [paper](https://symbioticlab.org/publications/files/tpp:asplos23/tpp-asplos23.pdf).

## Communication Frameworks, Shared Memory, and Common Libraries

- 🔓 StarfishOS: Revisiting Single System Image on CXL with State-Partitioned Microkernel **(SOSP 2026)** --- [paper page](https://starfishos-org.github.io/starfishos-docs/) [github](https://github.com/starfishos-org/starfishos).
- Duhu: Shared Disaggregated Memory for Distributed Data Processing Frameworks **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-men.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-men.pdf).
- MEGALON: Efficient Data Sharing for Partly Coherent CXL Memory **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-hu-jiyu.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-hu_jiyu.pdf).
- 🔓 Building A CSFQ-Inspired Transport for Switched CXL Memory Pooling **(NSDI 2026)** --- [paper](https://www.usenix.org/system/files/nsdi26-guo-zerui.pdf) [github](https://github.com/netlab-wisconsin/MemChannel) [slides](https://www.usenix.org/system/files/nsdi26_slides-guo-zerui.pdf).
- 🔓 Cxlalloc: Safe and Efficient Memory Allocation for a CXL Pod **(ASPLOS 2026)** --- [paper](https://www.cs.utexas.edu/~witchel/pubs/ni26asplos-cxlalloc.pdf) [github](https://github.com/nwtnni/cxlalloc).
- Quantifying the Cost of Software-Managed Synchronization on Multi-Host CXL Memory **(SC 2026, forthcoming)** --- [paper page](https://sc26.conference-program.com/presentation/?id=pap281&sess=sess232).
- 🔓 cMPI: Using CXL Memory Sharing for MPI One-Sided and Two-Sided Inter-Node Communications **(SC 2025)** --- [paper](https://pasalabs.org/papers/2025/SC25_CXL.pdf) [github](https://github.com/skhynix/cMPI).
- 🔓 Re-architecting End-host Networking with CXL: Coherence, Memory, and Offloading **(MICRO 2025)** --- [paper](https://saksham.web.illinois.edu/assets/pdf/cxl-nic.pdf) [github](https://github.com/ece-fast-lab/MICRO-2025-CXL-NIC).
- CXLfork: Fast Remote Fork over CXL Fabrics **(ASPLOS 2025)** --- [paper](https://tianyin.github.io/pub/cxlfork.pdf).
- 🔓 TrEnv: Transparently Share Serverless Execution Environments Across Different Functions and Nodes **(SOSP 2024)** --- [paper](https://madsys.cs.tsinghua.edu.cn/publication/trenv-transparently-share-serverless-execution-environments-across-different-functions-and-nodes/SOSP24-huang.pdf) [github](https://github.com/switch-container).
- HydraRPC: RPC in the CXL Era **(ATC 2024)** --- [paper](https://www.usenix.org/system/files/atc24-ma.pdf).

## Machine Learning, Recommendation, and Near-Memory Processing

- Beluga: A CXL-Based Memory Architecture for Scalable and Efficient LLM KVCache Management **(SIGMOD 2026)** --- [preprint](https://arxiv.org/pdf/2511.20172).
- 🔓 LIA: A Single-GPU LLM Inference Acceleration with Cooperative AMX-Enabled CPU-GPU Computation and CXL Offloading **(ISCA 2025)** --- [paper page](https://doi.org/10.1145/3695053.3731092) [github](https://github.com/ece-fast-lab/ISCA-2025-LIA).
- 🔓 PIM Is All You Need: A CXL-Enabled GPU-Free System for LLM Inference **(ASPLOS 2025)** --- [preprint](https://arxiv.org/pdf/2502.07578) [github](https://github.com/Yufeng98/CENT).
- CARINA: An Efficient CXL-Oriented Embedding Serving System for Recommendation Models **(SIGMOD 2025)** --- [paper page](https://doi.org/10.1145/3725274).
- Machine Learning-Guided Memory Optimization for DLRM Inference on Tiered Memory **(HPCA 2025)** --- [paper](https://pasalabs.org/papers/2025/HPCA25_DLRM.pdf).
- Enabling Efficient Large Recommendation Model Training with Near CXL Memory Processing **(ISCA 2024; ReCXL)** --- [paper page](https://doi.org/10.1109/ISCA59077.2024.00036).
- Computational CXL-Memory Solution for Accelerating Memory-Intensive Applications **(HPCA 2024)** --- [paper page](https://www.hpca-conf.org/2024/program/main.php).
- An LPDDR-based CXL-PNM Platform for TCO-efficient Inference of Transformer-based Large Language Models **(HPCA 2024)** --- [paper page](https://doi.org/10.1109/HPCA57654.2024.00078).
- Low-Overhead General-Purpose Near-Data Processing in CXL Memory Expanders **(MICRO 2024)** --- [paper page](https://microarch.hosting.acm.org/micro57/program/).
- PIFS-Rec: Process-In-Fabric-Switch for Large-Scale Recommendation System Inferences **(MICRO 2024)** --- [paper page](https://microarch.hosting.acm.org/micro57/program/).
- Efficient Tensor Offloading for Large Deep-Learning Model Training based on Compute Express Link **(SC 2024)** --- [paper](https://pasalabs.org/papers/2024/tensor_offloading_cxl.pdf).
- CXL-ANNS: Software-Hardware Collaborative Memory Disaggregation and Computation for Billion-Scale Approximate Nearest Neighbor Search **(ATC 2023)** --- [paper](https://www.usenix.org/system/files/atc23-jang.pdf).
- Enabling Efficient Large-Scale Deep Learning Training with Cache Coherent Disaggregated Memory Systems **(HPCA 2022; COARSE)** --- [paper](https://www.zixuan.wang/files/hpca22-coarse.pdf).

## Databases, Transactions, and Key-Value Stores

- 🔓 XTRA: Unifying Cache Coherence and Concurrency Control for Distributed Transactions in a CXL Pod **(SOSP 2026)** --- [paper](https://sosposdi.com/publications/2026/xtra/SOSP26-XTRA-paper.pdf) [github](https://github.com/cszjyang/xtra) [slides](https://sosposdi.com/publications/2026/xtra/SOSP26-XTRA-slides.pdf).
- Disk-Based LSMs: An Unexpectedly Good Index for Partly Coherent CXL Memory **(SOSP 2026)** --- [paper](https://dassl-uiuc.github.io/pdfs/papers/prism.pdf).
- SIDLE: Tree-structure Aware Indexes for CXL-based Heterogeneous Memory **(VLDB 2026)** --- [paper](https://www.vldb.org/pvldb/vol19/p1499-zhao.pdf).
- LakeMem: An Elastic Disaggregated-Memory Caching Layer for Analytical Processing Systems **(SIGMOD 2026, industry)** --- [paper](https://cighao.com/papers/lakemem.pdf).
- Building Memory Efficient Key-Value Stores in the CXL Era **(ATC 2026, accepted)** --- [paper page](https://sigops.org/s/conferences/atc/2026/accepted.html).
- 🔓 Tigon: A Distributed Database for a CXL Pod **(OSDI 2025)** --- [paper](https://www.usenix.org/system/files/osdi25-huang-yibo.pdf) [github](https://github.com/ut-datasys/tigon) [slides](https://www.usenix.org/sites/default/files/conference/protected-files/osdi25_slides_huang_yibo.pdf).
- CtXnL: A Software-Hardware Co-Designed Solution for Efficient CXL-Based Transaction Processing **(ASPLOS 2025)** --- [paper page](https://doi.org/10.1145/3676641.3716244) [preprint](https://arxiv.org/pdf/2502.11046).
- 🔓 CXL Memory Performance for In-Memory Data Processing **(VLDB 2025)** --- [paper](https://www.vldb.org/pvldb/vol18/p3119-weisgut.pdf) [github](https://github.com/hpides/cxlbench/tree/paper/vldb25).
- Unlocking the Potential of CXL for Disaggregated Memory in Cloud-Native Databases **(SIGMOD 2025, industry)** --- [paper](https://cighao.com/papers/PolarDB_CXL.pdf).
- An Examination of CXL Memory Use Cases for In-Memory Database Management Systems using SAP HANA **(VLDB 2024)** --- [paper](https://www.vldb.org/pvldb/vol17/p3827-ahn.pdf).
- CXL and the Return of Scale-Up Database Engines **(VLDB 2024)** --- [paper](https://www.vldb.org/pvldb/vol17/p2568-lerner.pdf).

## Storage, Shared Logs, and CXL SSDs

- Borges: A Low-Latency Distributed Shared Log on a CXL Memory/SSD Hybrid **(SOSP 2026)** --- [paper](https://www.cs.utexas.edu/users/witchel/pubs/chen26sosp-borges.pdf).
- Espresso: Constructing Cost-Efficient CXL JBOF via Inter-SSD Computing Resource Sharing **(OSDI 2026)** --- [paper](https://www.usenix.org/system/files/osdi26-yi.pdf) [slides](https://www.usenix.org/system/files/osdi26_slides-yi.pdf).
- CXL AnySSD: A Composable CXL SSD Using a CXL Type-2 Device and Any SSDs **(MICRO 2026)** --- [paper page](https://www.microarch.org/micro59/program/).
- XHarvest: Rethinking High-Performance and Cost-Efficient SSD Architecture with CXL-Driven Harvesting **(ISCA 2025)** --- [paper page](https://www.iscaconf.org/isca2025/program/).
- 🔓 ByteFS: System Support for (CXL-based) Memory-Semantic Solid-State Drives **(ASPLOS 2025)** --- [paper](https://platformxlab.github.io/papers/bytefs-asplos25.pdf) [github](https://github.com/platformxlab/bytefs).
- 🔓 SkyByte: Architecting an Efficient Memory-Semantic CXL-based SSD with OS and Hardware Co-design **(HPCA 2025)** --- [paper](https://platformxlab.github.io/papers/skybyte-hpca25.pdf) [github](https://github.com/platformxlab/skybyte).
- Overcoming the Memory Wall with CXL-Enabled SSDs **(ATC 2023)** --- [paper](https://www.usenix.org/system/files/atc23-yang-shao-peng.pdf) [slides](https://www.usenix.org/system/files/atc23_slides_yang-shao-peng.pdf).

## Coherence, Programming Models, and Verification

- 🔓 A Programming Model for Disaggregated Memory over CXL **(ASPLOS 2026)** --- [paper](https://www.cs.tau.ac.il/~orilahav/papers/asplos26.pdf) [github](https://github.com/cores-lab/cxl0).
- 🔓 vCXLGen: Automated Synthesis and Verification of CXL Bridges for Heterogeneous Architectures **(ASPLOS 2026)** --- [paper](https://anatolelefort.net/papers/vcxlgen-asplos26-preprint.pdf) [github](https://github.com/TUM-DSE/vCXLGen).
- 🔓 CXLMC: Model Checking CXL Shared Memory Programs **(ASPLOS 2026)** --- [paper page](https://plrg.ics.uci.edu/publications_page/) [github](https://github.com/uci-plrg/cxlmc) [artifact](https://zenodo.org/records/18205014).
- C³: CXL Coherence Controllers for Heterogeneous Architectures **(HPCA 2026)** --- [paper page](https://2026.hpca-conf.org/details/hpca-2026-main-conference/5/-C-3-CXL-Coherence-Controllers-for-Heterogeneous-Architectures).
- 🔓 Formalising CXL Cache Coherence **(ASPLOS 2025)** --- [paper](https://johnwickerson.github.io/papers/cxl_cache_ASPLOS25.pdf) [github](https://github.com/ChengsongTan/CXLcacheFormalisation).

## Security, Reliability, and Failure Recovery

- Compute eXpress Leak: New Cache Attacks Using CXL Devices **(MICRO 2026)** --- [paper](https://mktrm.github.io/files/cxleak-micro26.pdf).
- DIKTAMO: Extending CXL for Resilience to CPU Failures **(MICRO 2026)** --- [preprint](https://arxiv.org/pdf/2602.08271).
- Decoupled-DSM: A Scalable Secure Trusted Execution Environment for Multi-Host CXL Disaggregated Shared Memory **(MICRO 2026)** --- [paper page](https://yuanchaoxu6.github.io/publications/).
- 🔓 ReScue: Reliable and Secure CXL Memory **(HPCA 2026)** --- [paper page](https://2026.hpca-conf.org/details/hpca-2026-main-conference/57/ReScue-Reliable-and-Secure-CXL-Memory) [github](https://github.com/ece-fast-lab/HPCA-2026-ReScue).
- Efficient Security Support for CXL Memory through Adaptive Incremental Offloaded (Re-)Encryption **(MICRO 2025)** --- [paper page](https://doi.org/10.1145/3725843.3756119).
- Scaling Out Chip Interconnect Networks with Implicit Sequence Numbers **(SC 2025)** --- [paper page](https://sc25.conference-program.com/presentation/?id=pap552&sess=sess192).
- 🔓 Toleo: Scaling Freshness to Tera-scale Memory Using CXL and PIM **(ASPLOS 2024; presented in 2025)** --- [preprint](https://arxiv.org/pdf/2410.12749) [github](https://github.com/joydddd/Toleo).
- 🔓 TAROT: A CXL SmartNIC-Based Defense Against Multi-bit Errors by Row-Hammer Attacks **(ASPLOS 2024)** --- [paper](https://scale.snu.ac.kr/papers/2024-04-Conference-ASPLOS-TAROT.pdf) [github](https://github.com/ece-fast-lab/ASPLOS-24-TAROT).
- Salus: Efficient Security Support for CXL-Expanded GPU Memory **(HPCA 2024)** --- [paper](https://hzhou.wordpress.ncsu.edu/files/2024/02/Salus_HPCA_24_Camera_Ready.pdf).
- 🔓 Partial Failure Resilient Memory Management System for (CXL-based) Distributed Shared Memory **(SOSP 2023)** --- [paper](https://madsys.cs.tsinghua.edu.cn/publication/partial-failure-resilient-memory-management-system-for-cxl-based-distributed-shared-memory/SOSP23-zhang.pdf) [github](https://github.com/madsys-dev/sosp-paper19-ae).

## Simulation and Emulation Infrastructure

- 🔓 OCEAN: Open-Source CXL Emulation for Hyperscale Architecture and Networking **(SC 2026, forthcoming)** --- [paper](https://asplos.dev/pdf/OCEAN.pdf) [github](https://github.com/fam-emu/OCEAN).
- 🔓 Cohet: A CXL-Driven Coherent Heterogeneous Computing Framework with Hardware-Calibrated Full-System Simulation **(HPCA 2026)** --- [paper page](https://2026.hpca-conf.org/details/hpca-2026-main-conference/43/Cohet-A-CXL-Driven-Coherent-Heterogeneous-Computing-Framework-with-Hardware-Calibrat) [github](https://github.com/TianheMICALab/SimCXL).
- 🔓 Cylon: Fast and Accurate Full-System Emulation of CXL-SSDs **(FAST 2026)** --- [paper](https://www.usenix.org/system/files/fast26-yoon.pdf) [github](https://github.com/MoatLab/Cylon) [slides](https://www.usenix.org/system/files/fast26_slides_yoon.pdf).
- 🔓 Xerxes: Extensive Exploration of Scalable Hardware Systems with CXL-Based Simulation Framework **(FAST 2026)** --- [paper](https://www.usenix.org/system/files/fast26-an.pdf) [github](https://github.com/ChaseLab-PKU/Xerxes).

## Supplementary Papers from Other Venues and Workshops

These papers are useful additions to an awesome list, but are outside the main CCF-A conference collection.

- CXL-CCL: Inter-Node Collective GPU-Communication Using a CXL Shared Memory Pool **(ICS 2026)** --- [paper](https://pasalabs.org/papers/2026/ics26_cxl-ccl.pdf).
- Hash Joins Meet CXL: A Fresh Look **(CIDR 2026)** --- [paper](https://www.vldb.org/cidrdb/papers/2026/p1-huang.pdf).
- Replacing NVMe Staging in LLM Inference with a High-Bandwidth CXL Memory Expander with an On-Device DMA Controller **(MemNetAI workshop at SIGCOMM 2026)** --- [paper page](https://conferences.sigcomm.org/sigcomm/2026/memnetai/).
- My CXL Pool Obviates Your PCIe Switch **(HotOS 2025)** --- [paper](https://www.asafcidon.com/uploads/5/9/7/0/59701649/cxl-pool-hotos.pdf) [slides](https://sigops.org/s/conferences/hotos/2025/slides/slides321.pdf).
- Pasha: An Efficient, Scalable Database Architecture for CXL Pods **(CIDR 2025)** --- [paper page](https://mail.vldb.org/cidrdb/2025/pasha-an-efficient-scalable-database-architecture-for-cxl-pods.html).
- Fabric-Centric Computing **(HotOS 2023)** --- [paper](https://pages.cs.wisc.edu/~mgliu/papers/fcc-hotos23.pdf).
- CXL Memory as Persistent Memory for Disaggregated HPC: A Practical Approach **(SC Workshops 2023)** --- [paper page](https://doi.org/10.1145/3624062.3624175).
- Hello Bytes, Bye Blocks: PCIe Storage Meets Compute Express Link for Memory Expansion **(HotStorage 2022)** --- [paper](https://www.hotstorage.org/2022/camera-ready/hotstorage22-31/pdf/hotstorage22-31.pdf).

## Related PCIe Interconnect Work

- Understanding Routable PCIe Performance for Composable Infrastructures **(NSDI 2024)** --- [paper](https://www.usenix.org/system/files/nsdi24-hou.pdf).
- 🔓 An Ultra-Low Latency and Compatible PCIe Interconnect for Rack-Scale Communication **(CoNEXT 2022, best paper)** --- [paper page](https://doi.org/10.1145/3555050.3569128) [github](https://github.com/NTSocks/ntsocks).

## Blogs on CXL

- [Compute Express Link (CXL): All you need to know](https://www.rambus.com/blogs/compute-express-link/)


Latest update: 11/06/2026

