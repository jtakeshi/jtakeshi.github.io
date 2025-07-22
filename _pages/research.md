---
layout: single
title: "Research"
permalink: /research/
author_profile: true

---

Research Projects and Publications
====
My research can also be viewed at my [Google Scholar page](https://scholar.google.com/citations?hl=en&user=l7O3XKcAAAAJ&view_op=list_works&sortby=pubdate)
(NB: some papers may be listed in more than one area. Listings are approximately chronological.)

Trusted Hardware
--
Hardware-enforced security can operate much more efficiently than other methods of private computation, but faces serious limitations at high scale.
I investigate the effective use of Trusted Execution Environments and their combination with cryptographic constructions.
This work seeks to expand the scale and classes of computation that TEEs are capable of, eventually expanding trusted computing at hostile hosts to applications such as high-scale data mining and large language models.

* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Journal extension, published in SN Computer Science in 2024)](https://link.springer.com/article/10.1007/s42979-025-03804-w)
* Applying Trusted Hardware to Interoperable Private Attribution (internship project at Meta, not publicly released).
* [TERSE: tiny encryptions and really speedy execution for post-quantum private stream aggregation (Published at Securecomm 2022)](https://link.springer.com/chapter/10.1007/978-3-031-25538-0_18)
* [Developing non-interactive MPC with trusted hardware for enhanced security (Journal extension, published in the International Journal of Information Security)](https://link.springer.com/article/10.1007/s10207-022-00583-w)
* [Provably secure contact tracing with conditional private set intersection (Published at Securecomm 2021)](https://link.springer.com/chapter/10.1007/978-3-030-90019-9_18)
* [GPS: Integration of Graphene, PALISADE, and SGX for Large-scale Aggregations of Distributed Data. (Preprint)](https://eprint.iacr.org/2021/1155.pdf)
* [CryptoGram: fast private calculations of histograms over multiple users’ inputs (Published at DCOSS 2021)](https://ieeexplore.ieee.org/abstract/document/9600039/)
* [Cryptonomial: A Framework for Private Time-Series Polynomial Calculations (Published at Securecomm 2021)]: (https://eprint.iacr.org/2021/473.pdf)
* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Published at Securecomm 2021)](https://eprint.iacr.org/2020/1561.pdf)
* [Using Intel SGX to improve private neural network training and inference (Published at HoTSoS 2020)](https://dl.acm.org/doi/abs/10.1145/3384217.3386399)
* [Non-interactive MPC with trusted hardware secure against residual function attacks (Published at Securecomm 2019)](https://link.springer.com/chapter/10.1007/978-3-030-37231-6_25)

(More papers forthcoming!)

Hardware Acceleration of Homomorphic Encryption
--
Homomorphic encryption allows computation on data while it is still encrypted, enabling privacy-preserving outsourced computation. 
Unfortunately, the underlying mathematics lead to high computational intensity, data transfer latency, and memory overhead.
My work in hardware acceleration seeks to overcome these obstacles via bespoke hardware, utilizing in-memory computing to allow high parallelism and obviate the data transfer penalties seen in conventional architectures.
* [Privacy preserving in-memory computing engine (Preprint)](https://arxiv.org/abs/2308.02648)
* [Accelerating finite-field and torus FHE via compute-enabled (S)RAM (Published in IEEE Transactions on Computers in 2023)](https://ieeexplore.ieee.org/abstract/document/10202174/)
* [Algorithmic acceleration of B/FV-like somewhat homomorphic encryption for compute-enabled RAM (published at Selected Areas in Cryptography 2020)](https://link.springer.com/chapter/10.1007/978-3-030-81652-0_3)
* [Computing-in-memory for performance and energy-efficient homomorphic encryption (published in IEEE Transactions on VLSI Systems in 2020)](https://ieeexplore.ieee.org/abstract/document/9179010/)

(More papers forthcoming!)


Homomorphic Encryption (not related to hardware acceleration)
--
Since the original formulation of fully homomorphic encryption in 2009, a great deal of research has gone into taking FHE from a theoretical construction to practical deployment.
My work joins this effort by helping to explore and improve software utility, performance, and real-world applications.
The impact of this body of work contributes to making FHE truly usable for the ordinary software engineer, allowing seamless integration of privacy into the applications that process our personal data.

* [HEProfiler: An in-depth profiler of approximate homomorphic encryption libraries (published in the Journal of Cryptographic Engineering in 2025)](https://link.springer.com/article/10.1007/s13389-025-00377-5)
  * The software framework of HEProfiler can be found [here](https://gitlab.com/jtakeshi/homenc-profile).
  * I expanded upon this work in an industry project, though it is not publicly available.
* [Summation-based Private Segmented Membership Test from Threshold-Fully Homomorphic Encryption (published in the Proceedings on Privacy-Enhancing Technologies Symposium in 2024)](https://crysp.petsymposium.org/popets/2024/popets-2024-0114.php)
  * If you are wondering how dividing by zero is relevant to a FBI watchlist, this paper will be interesting to you!
* [Provably secure contact tracing with conditional private set intersection (Published at Securecomm 2021)](https://link.springer.com/chapter/10.1007/978-3-030-90019-9_18)
* [GPS: Integration of Graphene, PALISADE, and SGX for Large-scale Aggregations of Distributed Data. (Preprint)](https://eprint.iacr.org/2021/1155.pdf)


Private Stream Aggregation
--
The problem of allowing an untrusted server to aggregate many users' data points has been previously addressed. 
However, many of these prior works face limitations including questionable security, small message spaces, poor scalability, or lacking post-quantum security.
My work in this area devises purpose-built protocols, using only the most necessary core mathematical building blocks from homomorphic encryption.
These works show massive performance gains over the prior state-of-the-art, and additionally contribute new functionality such as fault tolerance and polynomial aggregation.
Further, the greatly improved simplicity of these schemes paves the way forward for future research and development.
Applications of this work include privacy-preserving elections, advertising, data mining, and artificial intelligence; this work can also be directly applied to existing strategies such as federated learning.

* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Journal extension, published in SN Computer Science in 2024)](https://link.springer.com/article/10.1007/s42979-025-03804-w)
* [PPSA: Polynomial Private Stream Aggregation for Time-Series Data Analysis (Published at Securecomm 2024)(https://eprint.iacr.org/2024/1460.pdf)
* [SLAP: Simpler, Improved Private Stream Aggregation from Ring Learning with Errors](https://link.springer.com/article/10.1007/s00145-023-09450-w)
  * The software library for SLAP can be found [here](https://gitlab.com/jtakeshi/lattices/). It could do with some more QoL features, and maybe some multithreading.
* [TERSE: tiny encryptions and really speedy execution for post-quantum private stream aggregation (Published at Securecomm 2022)](https://link.springer.com/chapter/10.1007/978-3-031-25538-0_18)
* [Cryptonomial: A Framework for Private Time-Series Polynomial Calculations (Published at Securecomm 2021)]: (https://eprint.iacr.org/2021/473.pdf)
* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Published at Securecomm 2021)](https://eprint.iacr.org/2020/1561.pdf)



Secure Data Deduplication
--

Technology and Society
--

Music Theory
--
