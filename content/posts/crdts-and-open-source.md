---
title: "CRDTs and Open Source"
date: 2018-10-19T21:29:10-06:00
draft: false
---

CRDTs, [conflict free replicated data types](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type), are data structures that can be synchronized across an unreliable network with consistency guarantees. [Here](https://www.youtube.com/watch?v=B5NULPSiOGw) is a talk on CRTDs from Martin Kleppmann. His group has produced a CRTD library called [automerge](https://github.com/automerge/automerge) which gives an application a JSON-like data structure that is replicated across multiple machines. Why is this significant? Open Source currently can't compete with SAAS because users want their data backed up and available on all devices, and unfortunately servers cost money. CRDTs will allow Open Source software to consistently replicate data across multiple machines without a centralized server. With CRDTs Open Source will be competitive with SAAS solutions. As an added bonus, CRDTs give users greater privacy because a centralized server is not needed.
