---
layout: single
title: "Research Projects and Publications"
permalink: /research/
author_profile: true

---

My research papers can also be viewed at my [Google Scholar page](https://scholar.google.com/citations?hl=en&user=l7O3XKcAAAAJ&view_op=list_works&sortby=pubdate).

(NB: some papers may be listed in more than one area. Listings are approximately chronological.)

Hardware Acceleration of Homomorphic Encryption
--
Homomorphic encryption allows computation on data while it is still encrypted, enabling privacy-preserving outsourced computation. 
Unfortunately, the underlying mathematics lead to high computational intensity, data transfer latency, and memory overhead.
My work in hardware acceleration seeks to overcome these obstacles via bespoke hardware, utilizing in-memory computing to allow high parallelism and obviate the data transfer penalties seen in conventional architectures.
* [Privacy preserving in-memory computing engine (Preprint)](https://arxiv.org/abs/2308.02648)
* [Accelerating finite-field and torus FHE via compute-enabled (S)RAM (Published in IEEE Transactions on Computers in 2023)](https://ieeexplore.ieee.org/abstract/document/10202174/)
* Initial implementation and design of Google's [Jaxite](https://github.com/google/jaxite) library, which implements Torus FHE on a Tensor Processing Unit. 
* [Algorithmic acceleration of B/FV-like somewhat homomorphic encryption for compute-enabled RAM (published at Selected Areas in Cryptography 2020)](https://link.springer.com/chapter/10.1007/978-3-030-81652-0_3)
* [Computing-in-memory for performance and energy-efficient homomorphic encryption (published in IEEE Transactions on VLSI Systems in 2020)](https://ieeexplore.ieee.org/abstract/document/9179010/)

(More papers forthcoming!)

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
* [Cryptonomial: A Framework for Private Time-Series Polynomial Calculations (Published at Securecomm 2021)](https://eprint.iacr.org/2021/473.pdf)
* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Published at Securecomm 2021)](https://eprint.iacr.org/2020/1561.pdf)
* [Using Intel SGX to improve private neural network training and inference (Published at HoTSoS 2020)](https://dl.acm.org/doi/abs/10.1145/3384217.3386399)
* [Non-interactive MPC with trusted hardware secure against residual function attacks (Published at Securecomm 2019)](https://link.springer.com/chapter/10.1007/978-3-030-37231-6_25)

(More papers forthcoming!)

Homomorphic Encryption (besides hardware acceleration works)
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

(More papers forthcoming!)

Private Stream Aggregation
--
The problem of allowing an untrusted server to aggregate many users' data points has been previously addressed. 
However, many of these prior works face limitations including questionable security, small message spaces, poor scalability, or lacking post-quantum security.
My work in this area devises purpose-built protocols, using only the most necessary core mathematical building blocks from homomorphic encryption.
These works show massive performance gains over the prior state-of-the-art, and additionally contribute new functionality such as fault tolerance and polynomial aggregation.
Further, the greatly improved simplicity of these schemes paves the way forward for future research and development.
Applications of this work include privacy-preserving elections, advertising, data mining, and artificial intelligence; this work can also be directly applied to existing strategies such as federated learning.

* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Journal extension, published in SN Computer Science in 2024)](https://link.springer.com/article/10.1007/s42979-025-03804-w)
* [PPSA: Polynomial Private Stream Aggregation for Time-Series Data Analysis (Published at Securecomm 2024)](https://eprint.iacr.org/2024/1460.pdf)
* [SLAP: Simpler, Improved Private Stream Aggregation from Ring Learning with Errors](https://link.springer.com/article/10.1007/s00145-023-09450-w)
  * The software library for SLAP can be found [here](https://gitlab.com/jtakeshi/lattices/). It could do with some more QoL features, and maybe some multithreading.
* [TERSE: tiny encryptions and really speedy execution for post-quantum private stream aggregation (Published at Securecomm 2022)](https://link.springer.com/chapter/10.1007/978-3-031-25538-0_18)
* [Cryptonomial: A Framework for Private Time-Series Polynomial Calculations (Published at Securecomm 2021)](https://eprint.iacr.org/2021/473.pdf)
* [Cryptonite: A Framework for Flexible Time-Series Secure Aggregation with Non-interactive Fault Recovery (Published at Securecomm 2021)](https://eprint.iacr.org/2020/1561.pdf)

(More papers forthcoming!)

Technology and Society
--
My belief is that an important purpose of academic research is to not only carry out purely technical work, but to think critically about how that work affects society. This is especially important for computer scientists, considering how strongly the world is impacted by our domain. My work to uphold this obligation spans topics including AI, law, and higher education.

* Duty of Care: A Call for Open and Responsible AI Innovation in Healthcare. (Position paper to be published in the AAAI 2025 Fall Symposium Series, SECURE-AI4H)
* Spoke at "The Future of Voice Communications: AI Transformations Roundtable" - Old Dominion University and Map Communications (Spring 2025)
* Presented "Failure and Success in Graduate Study" - ODU CS 800 (Spring 2025)
* Presented "Privacy-Enhancing Technologies in American Law" at the Kwansei Gakuin University Workshop on Privacy-Enhancing Technologies and Law (2024)
* Presented "Privacy-Enhancing Technologies for Educationally Focused AI" at the [Trustworthy AI Lab for Education Summit](https://lucyinstitute.nd.edu/trustworthy-ai-lab-for-education-summit/) (2023)

(More papers forthcoming!)

Music Theory
--
Western music theory utilizes a 12-tone system, with the interval between each octave divided into 12 semitones. Previous work applied group theory to extend the mathematical framework underlying the 12-tone system to systems with 8k+4 semitones (for positive integers k). My senior thesis work under Dr. Mark Bollman explored continuing this line of research. Counterpoint, the style and rules of music defining the Baroque era, depends heavily on intervals between different melodic lines. Thus in order to be able to write contrapuntal music in systems of 8k+4 tones, a concept of “interval” is needed for these higher-order systems. My research showed that the traits of intervals in a 12-tone system can be used to derive an algorithm for classifying intervals in higher-order systems, and that the algorithm’s results are coherent and consistent with both the 12-tone system and higher-order systems. 

If there is a student with the prerequisite background in modern algebra and music theory, then I am happy to mentor them in continuing this work. A warning to anyone wanting to continue this line of research: though the mathematics are fascinating, a conclusion of previous work is that music in higher-order systems will sound unpalatably dissonant.

* [Classification of Consonance in Generalized Tonal Systems (published in The Pentagon, Vol 76, No. 2)](http://www.kappamuepsilon.org/Pentagon/Vol_76_Num_2_Spring_2017.pdf)
  * [Implementation of the classification algorithm](https://gitlab.com/jtakeshi/consonances)


Secure Data Deduplication
--
Deduplication is the process of identifying similar or identical data so as to conserve storage and bandwidth by not needlessly storing duplicates. Deduplication schemes are very diverse, differing in their goals, methods, and assumptions. Performing deduplication securely presents a natural conflict: users wish to safeguard their data, but information about the data must be used to detect duplicates. My work in deduplication asks: how much functionality can a deduplication scheme achieve in a highly adversarial scenario, using minimal cryptographic assumptions? It turns out you can do a lot: without even a single trusted party, secure nearly-identical deduplication can be achieved even against fully malicious adversaries.

* [Secure Single-Server Nearly-Identical Image Deduplication (Published at IEEE ICCCN 2020)](https://ieeexplore.ieee.org/abstract/document/9209728)
