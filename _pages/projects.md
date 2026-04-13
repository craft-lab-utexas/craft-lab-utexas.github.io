---
layout: page
title: research
permalink: /research/
nav: true
nav_order: 3
---

The CRaFT Lab develops formal reasoning systems and makes production-grade tools 
and services accessible at scale. Our research sits at the intersection of Formal Methods, 
Artificial Intelligence, theoretical Mathematics and scalable systems infrastructure.

---

## Formal Methods and Interactive Theorem Proving

Formal Methods (FM) provide mathematically rigorous techniques for specifying, 
verifying, and reasoning about systems. We work with a broad range of FM tools 
including Interactive Theorem Provers (ITPs) such as 
[Lean](https://leanprover.github.io/), 
SAT/SMT solvers such as [Z3](https://github.com/z3prover/z3), and model checkers such as 
[TLA+](https://lamport.azurewebsites.net/tla/tla.html) and [Alloy](https://alloytools.org/). 
A particular focus is the use of ITPs for theoretical mathematics, including the integer 
sequences defined in the Online Encyclopedia of Integer Sequences (OEIS) as well as for 
software verification.

---

## AI and Formal Methods

Part of our research is devoted to building and integrating FM tools with modern AI. 
We are interested in both directions of this relationship:

- **FM-assisted AI**: using formal verification techniques to improve the 
  robustness, reliability, and trustworthiness of AI systems, particularly 
  large language and reasoning models which are susceptible to hallucination 
  and unverified reasoning. 
- **AI-assisted FM**: leveraging LLMs/LRMs to accelerate formal reasoning tasks, including   
  autoformalization (encoding natural language mathematics into machine-verifiable proofs)
  and AI-guided proof search

Recent results such as Google DeepMind's AlphaProof demonstrate the rapid 
progress in this area and motivate our focus on building the infrastructure 
needed to support it at scale.

---

## Scalable Infrastructure for Formal Reasoning

A distinguishing focus of CRaFT Lab is the development of production-grade, 
hosted, open software infrastructure that makes FM and AI tools 
accessible to researchers and educators. Running tools such as SAT/SMT solvers, 
ITP servers, and LLM inference at research scale requires significant systems 
engineering. Within scope includes the development and long-term maintenance 
of the following:

- Hosted inference services for large language and reasoning models
- Scalable SAT/SMT solver services (e.g., Z3, CVC5)
- ITP server infrastructure for Lean and other provers
- Computer algebra system (CAS) interfaces
- Knowledge bases and formalization libraries

These tools and services will be deployed onto advanced computing 
infrastructure at the [Texas Advanced Computing Center (TACC)](https://tacc.utexas.edu) and will be made
available to researchers at UT Austin and partnering institutions.

---

## Theoretical Computer Science and Mathematics

Underlying all of our work is an interest in and  commitment to theoretical foundations. We are 
interested in problems at the boundary of mathematics and computer science 
including algebra, combinatorics, logic, proof theory, type theory, and their applications 
to verification and AI. 

---

## Collaborations and Funding

CRaFT Lab actively seeks collaborations across departments at UT Austin and 
with external partners in academia and industry. We are grateful for support 
from [TACC](https://tacc.utexas.edu).

If you are interested in collaborating, please reach out to 
[jstubbs@tacc.utexas.edu](mailto:jstubbs@tacc.utexas.edu).