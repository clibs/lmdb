Website: http://symas.com/mdb/

Quick Overview
--------------

LMDB is a tiny database with some great capabilities:

* Ordered-map interface (keys are always sorted, supports range lookups)
* Fully transactional, full ACID semantics with MVCC.
* Reader/writer transactions: readers don't block writers and writers don't block readers. Writers are fully serialized, so writes are always deadlock-free.
* Read transactions are extremely cheap, and can be performed using no mallocs or any other blocking calls.
* Supports multi-thread and multi-process concurrency, environments may be opened by multiple processes on the same host.
* Multiple sub-databases may be created with transactions covering all sub-databases.
* Memory-mapped, allowing for zero-copy lookup and iteration.
* Maintenance-free, no external process or background cleanup/compaction required.
* No application-level caching. LMDB fully exploits the operating system's buffer cache.
* 32KB of object code and 6KLOC of C.
* Licensed under the OpenLDAP Public License
* It is a read-optimized design and performs reads several times faster than other DB engines, several orders of magnitude faster in many cases. It is not a write-optimized design; for heavy random write workloads other DB designs may be more suitable.

License
-------
The OpenLDAP Public License
