# tease

## Description:

This is TEASE (**T**est-**E**vidence-**A**s-a-**S**ervic**E**) which, as the name might suggest, is (intended to be) a micro-service provisioning a uniform approach to the recording and subsequent retrieval, of configuration management related records and do so in a manner that ensures that the stored data isn't corrupted in/by the storage and once stored, the stored records are immutable where the initial i.e. pilot, case is test evidence based.

---

## Vision

In creating this, my vision was and indeed still is, of a service running at 2 levels whereby the...
- Lowest level i.e. closest to the record source, is a container provisioning both storage and retrieval capabilities.
- Higher level is the same container provisioning only a retrieval capability and is typically consumed by e.g. a centralized dashboarding facility.

Moreover, in an attempt to follow the fundamental KISS (**K**eep **I**t **Simple** **S**tupid) principle, the vision entails the use of text records maintained using Git repositories - by this means, a version of the registered archive respoitory can readily be utilized at both local and remote levels - thus eliminating the "works for me" syndrome.

Note that the immutability of the stored records is, as the epithet suggests, inviolable whereas the meta-data used in the storage of the records isn't (to the same degeree) and may be modified ruled by the rigour of appropriate change procedures.

---

## Actors

### QA Engineer

The _QA Engineer_ is a read-write role whose responsibilities are to...
- Ensure the creation & initial registration of the archive repository (write).
- Ensure the records are correctly attributed (by maintaining the test patterns (+ associated sub-patterns - if any) (read-write).
- Verify the correctness of submission(s)) &/or...
- Generate elements of release notes in terms of e.g. known failed tests & their mitigation(s) (if any).

### Engineer

The _Engineer_ has 2 basic responsibilities...
- Subsequent submission of evidence records and optionally...
- Retrieval of created records - to ...
    - Verify the correctness of submission(s)) &/or...
    - Generate elements of release notes in terms of e.g. known failed tests & their mitigation(s) (if any).

### Project Owner

The _Project  Owner_ is a read-only role having the responsibility to retrive stored records for the purposes of such things as progress/trend dashboarding, release note generation et al.

### Auditor

The _Auditor_ is a read-only role having the sole responsibility to verify the integrity & correctness of the stored records.
sile 


## Use Cases

### Submit Record

As an _Engineer_, I want to be able to store immutable records of test evidence in a location of my choosing in order to be able to assert compliance with ruling standards.

### Register Archive

As an _Engineer_, I want to be able to register a repository of my choosing as a records archive in order that I might subsequently submit records to the registered archive..

### Register Pattern

As a _QA Engineer_, I want to be able to register a new test pattern, c/w optionally one, or more, associated sub-patterns, in order to correctly attribute recorded evidence.

### Update Pattern

As a _QA Engineer_, I want to be able to update previously registered test pattern, typically to add/remove associated sub-patterns, in order to correctly attribute recorded evidence.

Note that deletion of a test (sub-)pattern requires that records attributed with the soon-to-be deleted pattern are re-allocated to a different sub-pattern.

### Retrieve Record

As a _Project Owner_, I want to be able to retrieve stored record(s) in order to utilize them (the retrieved records) as a data source for the generation of dashboard(s) &/or release note(s) .

As an _Auditor_, I want to be able to retrieve stored records (+ associated meta-data) in order to audit compliance with ruling standards.

---

## To Do

- Extrapolate the generics to create a configurable, immutable records archival/storage & retrieval service e.g. **R** **E** of **I**mmutable **E**vidence **S**ervice ;-), of which this i.e. test evidence, is but an instantiation and is such as might be employed in any CM system worthy of the epithet.

---

END OF DOCUMENT
