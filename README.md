# tease

## Description:

This is TEASE (**T**est-**E**vidence-**A**s-a-**S**ervic**E**) which, as the name might suggest, is (intended to be) a micro-service provisioning a uniform approach to the recording and subsequent retrieval, of configuration management related records ,  and which are, once stored, immutable. in this case test evidence records are the core 

---

## User Stories


### Story

As a test engineer, I want to be able to store immutable records of test evidence in a location of my choosing in order to be able to assert compliance with ruling standards.

[Expectations](src/test/features/storage.feature)


### Story

As a release engineer, I want to be able to retrieve stored evidence in order to support audits of compliance with ruling standards.

[Expectations](src/test/features/retrieval.feature)

### Story

As a compliance engineer, I want to be assured that the data is incorruptibly stored in order that I may have full confidence in the data.

---

## To Do

- Extrapolate the generics to form a configurable immutable records archival & retrieval service such as might be employed in any decent CM system. (or ecosystem ;-))

---

END OF DOCUMENT
