---
title: "A Data Optimizer for Region-Aware Self-describing Files in Scientific Computing"
collection: publications
category: conf
permalink: /publication/raster
excerpt: 'Yanjie Song\*, <u>Tianyuan Wu*</u>, Yuanhao Li, Guancheng Li, Yuchen Liu, Shu Yin, Wei Xue, Junchao Wang (\* Equal contribution).'
date: 2024-11-22
venue: '2024 ACM Symposium on Cloud Computing (SoCC\'24)'
paperurl: 'http://www.tianyuanwu.com/files/socc24-final138.pdf'
citation: 'Yanjie Song, Tianyuan Wu, Yuanhao Li, Guancheng Li, Yuchen Liu, Shu Yin, Wei Xue, and Junchao Wang. "A Data Optimizer for Region-Aware Self-describing Files in Scientific Computing." In Proceedings of the 15th ACM Symposium on Cloud Computing, pp. 431-446. 2024.'
---

Acquiring data from scientific simulations for analytical purposes is inherently challenging due to the complex and irregularly shaped regions within which the data resides, particularly when using self-describing data formats. The process of region-based data distillation becomes even more arduous when employing persistent memory or parallel file systems. To tackle this challenge, we introduce RASTER (Region-Aware Self-describing daTa optimizER), a lightweight middleware designed for region-aware data preprocessing. RASTER dynamically reorganizes data into variable groups based on regional identifiers during runtime, thereby eliminating the need for sequential searches to locate the required data.

We have developed a prototype of RASTER and successfully integrated it into three distinct computing environments: a single-node server equipped with Intel Optane DC persistent memory, the Huawei OceanStor cloud storage platform, and the Sunway TaihuLight supercomputer. We then conducted a thorough evaluation of the RASTER prototype on the latter two platforms using a real-world scientific application, CESM (Community Earth System Model). Our experimental results demonstrate that RASTER enhances data acquisition performance by up to 2.83×and achieves a 2.36× speedup over conventional netCDF and the state-of-the-art ADIOS2. Additionally, RASTER significantly reduces memory usage by up to 400%, showcasing its scalability potential.