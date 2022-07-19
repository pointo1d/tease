# tease

## Description:

This is TEASE (**T**est-**E**vidence-**A**s-a-**S**ervic**E**) which, as the name might suggest, is (intended to be) a micro-service provisioning a uniform approach to the recording and subsequent retrieval, of configuration management related records and do so in a manner that ensures that the stored data isn't corrupted in/by the storage and once stored, the stored records are immutable where the initial i.e. pilot, case is test evidence based.

---

## Vision

In creating this, my vision was and indeed still is, of a micro-service container running locally at 3 levels whereby the...
- Lowest level i.e. closest to the record source, provisions both storage and retrieval capabilities.
- Higher level is the same container provisioning only a retrieval capability and is typically consumed by e.g. a centralized dashboarding facility.
- Highest level is also the same container, but this time merely serving to provide a central repository for meta-data e.g. 
    - Test pattern (+ any associated sub-pattern) definitions.
    - Archive registry. 

Moreover, in an attempt to follow the fundamental KISS (**K**eep **I**t **S**imple **S**tupid) principle, the vision entails the use of text records maintained using Git repositories - by this means, a version of the registered archive respoitory can readily be utilized at both local and remote levels - thus eliminating the "works for me" syndrome.

Note that the immutability of the stored records is, as the epithet suggests, inviolable whereas the meta-data used in the storage of the records isn't and may thus be modified ruled by the rigour of appropriate change procedures.

---

[Use Case Diagram](UML/tease.ucase.violet.html)

## Actors

### General (NFT)

This isn't a use case per-se, but merely a container for the NFT use cases that come into play in each and every one of of the following actor specific sub-sections...

As an _interested party_, I want...

- stored records to be immutable in order to be assured of their post-storage quality i.e. untampered state (**Immutable Stored Records**).
- stored records to be uniquely identifiable (**Uniquely Identified Stored Records**).

### Administrator

#### Use Case(s)

As an _Administrator_, I want to be able to maintain the meta-data repository in order to maintain the alignment between the definitions & the (current) _thinking_.

### QA Engineer

#### Use Case(s)

As a _QA Engineer_,  I want to be able to...
- Register an archive repository in order to provide a receiver for records to be lodged (write).
- Ensure the records are correctly attributed (by maintaining the test patterns (+ associated sub-patterns - if any) (read-write).
- Verify the correctness of submission(s)) &/or...
- Generate elements of release notes in terms of e.g. known failed tests & their mitigation(s) (if any).

### Engineer

#### Use Case(s)

As an _Engineer_ (dev, test or even SDET), I want to be able to...
- Lodge records.
- Retrieve lodged record(s), using an optional filter, in order to...
    - Verify the correctness of submission(s)) &/or...
    - Generate elements of release notes in terms of e.g. known failed tests & their mitigation(s) (if any).

### Project Owner

#### Use Case(s)

As a  _Project  Owner_, I want to be able to...
- retrieve stored records in order to generate such elements as progress/trend dashboarding, release note generation et al.

### Auditor

#### Use Case(s)

As an _Auditor_, I want to be able to...
- retrieve stored records in order to verify the integrity & correctness of the retrieved records.

---

## To Do

- Extrapolate the generics to create a configurable, immutable records archival/storage & retrieval service e.g. **R** **E** of **I**mmutable **E**vidence **S**ervice ;-), of which this i.e. test evidence, is but an instantiation and is such as might be employed in any CM system worthy of the epithet.

---

## References
1. UML Distilled (Third Edition), Fowler, 2004, Addison-Wesley, 0-321-19368-7
2. Use Case Modelling, Bittner & Spence, 2003, Addison-Wesley, 0-201-70913-9


---

## Author & Copyright

(c) Dave Pointon FIAP MBCS (pointo1d at gmail dot com)

---

## Date

Jul 2021

---

END OF DOCUMENT
