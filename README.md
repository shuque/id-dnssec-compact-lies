# id-dnssec-compact-lies
Compact Denial of Existence in DNSSEC

This document describes a technique to generate a signed DNS response
on demand for a non-existent name by claiming that the name exists
but doesn't have data for the queried record type, and returning
NODATA answer with an accompanying NSEC proof.  Such answers require
only one NSEC record and allow online signing servers to minimize
signing operations and packet size.
