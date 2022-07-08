# teas

## Description:

This is TEASE (Test-Evidence-As-ServicE) which, as the name might suggest, is (intentded to be) a micro-service that provisions a uniform approach to the recording and subsequent retrieval, of configuration management related records, in this case test evidence and which are, once stored, immutable.


---

## User Stories

### Evidence Storage

#### Story

As a test engineer, I want to be able to store immutable records of test evidence in a location of my choosing in order to be able to assert compliance with ruling standards.

#### [Expectations](src/test/features/storage.feature)

### Evidence Retrieval 

#### Story

As a release engineer, I want to be able to retrieve stored evidence in order to support audits of compliance with ruling standards.

#### [Expectations](src/test/features/retrieval.feature)

---

## To Do

- Extrapolate the generics to form a configurable immutable records archival & retrieval service such as might be employed in any decent CM system. (or ecosystem ;-))

---

END OF DOCUMENT
