---
layout: page
permalink: /project/
title: Selected Projects I am Involved
tags: [project]
modified: 2-9-2016
comments: false
---

---

### Secure Outsourced Middleboxes

Middleboxes are essential for a wide range of advanced traffic processing in enterprise networks. The trend of deploying middleboxes in public clouds as virtualized services further expands potential benefits of middleboxes while avoiding local maintenance burdens. Despite promising, middlebox outsourcing is facing crucial security challenges. Traffic now is redirect to cloud, where the traffic content and proprietary middlebox rules are exposed. On the other hand, these boxes are no longer under the direct control of enterprises. It is desirable to ensure that these boxes function as intended. 

<div style="text-align:center">
<img  src="{{ site.BASE_PATH }}/images/mb.jpg" alt="Drawing" style="width: 400px;"/>
<br>
<br>
Cloud Middlebox Service Architecture
</div>

1. How to design a secure middlebox system that performs network functions without revealing either packet payloads or rules? 
2. How to devise practical mechanisms that provide runtime execution assurance of outsourced middleboxes with high confidence? 

Fulfilling those requirements will ease enterprises privacy and security concerns, extend their visibility into remote middleboxes, and promote further adoption of NFV services. Preliminary results that address the above questions are published in [IEEE INFOCOM’16](http://ieeexplore.ieee.org/document/7524526/?arnumber=7524526) and [IEEE ICNP’16](http://ieeexplore.ieee.org/document/7784424/). 

<iframe src="https://player.vimeo.com/video/192397197" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
<p><a href="https://vimeo.com/192397197">Towards Verifiable Outsourced Middleboxes</a></p>
Credit: Huayi Duan, Xingliang Yuan, and Cong Wang.

### Encrypted Distributed Data Store

In order to manage the persistently growing amount of data, distributed data stores have become the backbone of many public cloud services. However, with increasing data breaches, privacy concerns in data outsourcing become even more pressing than before. To address those concerns, we start from the most widely adopted data store, i.e., key-value stores, and build an encrypted, distributed, and searchable key-value store. Specifically, we cope with the following challenges so that the proposed system will not sacrifice the benefits of existing systems. 

1. How to securely distribute encrypted data across distributed nodes? 
2. How to design an overlay that supports multiple data models with strong security guarantees?  
3. How to design a framework for encrypted and distributed indexes that enable secure queries on secondary attributes of data?  

<div style="text-align:center">
<img  src="{{ site.BASE_PATH }}/images/kv.jpg" alt="Drawing" style="width: 300px;"/>
<br>
<br>
Encrypted Key-value Store Architecture
</div>
<br>

Our proposed encrypted key-value store achieves strong protection on data privacy while preserving prominent features of key-value stores. It is built on a secure data partition algorithm that distributes encrypted data evenly across a cluster of nodes. It also supports multiple data models in a privacy-preserving manner. To enable secure queries for encrypted secondary attributes of data, our design provides searchable encryption based encrypted secondary indexes which consider security, efficiency, and data locality simultaneously. The results are published in [ACM ASIACCS’16](http://dl.acm.org/citation.cfm?id=2897852) and [ACM ASIACCS’17](http://dl.acm.org/citation.cfm?id=3052977). 

<iframe src="https://player.vimeo.com/video/192397625" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
<p><a href="https://vimeo.com/192397625">BlindDB - an Encrypted, Distributed, and Searchable Key-value Store</a> </p>
Credit: Xinyu Wang, Jianxiong Lin, Xingliang Yuan, Yu Guo, and Cong Wang.


### Privacy-assured Similarity Search for Large-scale Applications

Big data are usually drawn from varieties of forms: not just texts, but also images, audio, video, and other information-rich content, which are usually represented as high-dimensional data records. In this context, similarity queries are more desired than exact-match queries. Meanwhile, multimedia data often contain sensitive or personal information. Thus, enabling secure content-aware query processing over encrypted multimedia data is very demanding. Yet, most prior solutions on encrypted search are for exact-match queries. 

<div style="text-align:center">
<img  src="{{ site.BASE_PATH }}/images/simsse.jpg" alt="Drawing" style="width: 400px;"/>
<br>
<br>
Privacy-preserving Image Querying Service
</div>
<br>

To bridge the gap, we first note that this problem could be theoretically handled by a direct combination of locality-sensitive hashing (LSH) and searchable symmetric encryption (SSE), where LSH is a well-studied algorithm for fast similarity search, and SSE is a widely adopted security framework for encrypted search. By treating LSH hash value(s) as keyword(s), one may apply known SSE schemes to realize secure similarity search. However, we observed that such a straightforward solution does not achieve practical scalability and efficiency as the sizes of datasets are continuously growing. Rather than just assembling off-the-shelf designs in a blackbox manner, we consider challenges and requirements in different  scenarios, e.g., applications that need to support low latency queries, applications that need to handle streaming data in high rates, and applications deployed in distributed systems. To serve these needs, we develop new constructions from the ground up. The results are published in [IEEE ICDCS’14](http://ieeexplore.ieee.org/document/6888896/?arnumber=6888896),   [ESORICS’15](http://link.springer.com/chapter/10.1007/978-3-319-24177-7_3), [IEEE TMM](http://ieeexplore.ieee.org/document/7552468/), and [IEEE/ACM IWQoS'17](). 


### Secure Content Delivery via Encrypted In-network Caching

To handle the exponential growth of media content, emerging network architectures along the direction of Information-Centric Networking (ICN) have been proposed. Storing data in advanced network devices such as cache-enabled routers, benefits like reduced content access latency are well appreciated. However, due to potentially wide attacking surfaces, caching data in the increasingly untrustworthy networked environment raises new concerns on user privacy exposure and unauthorized data access.  

<div style="text-align:center">
<img  src="{{ site.BASE_PATH }}/images/icn.jpg" alt="Drawing" style="width: 250px;"/>
<br>
<br>
Content Delivery Service via Encrypted In-network Caching
</div>
<br>

To address these concerns, we designed new networked systems for secure and efficient content dissemination through encrypted in-network caching. To move one-step further towards practice, we consider the effective support of content dissemination from multiple providers to authorized users, and study how to efficiently enable authorized search across encrypted in-network content from multiple providers under their own different keys. To broaden the application scenarios, our system also supports advanced content-aware data dissemination scenarios by incorporating the content near-duplicate detection into our encrypted in-network cache system. Preliminary results are published in [IEEE JSAC](http://ieeexplore.ieee.org/document/7485895/?arnumber=7485895) and [IEEE INFOCOM’16](http://ieeexplore.ieee.org/document/7524346/?arnumber=7524346). 




