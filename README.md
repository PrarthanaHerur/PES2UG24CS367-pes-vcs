# PES-VCS — Version Control System

## Student Details
Name: Prarthana Herur  
SRN: PES2UG24CS367  

---

## Phase 1: Object Storage

### Description
Implemented SHA-256 based content-addressable storage.
Objects are stored in `.pes/objects` using directory sharding.

### Output
![Test](images/phase1_test.png)
![Objects](images/phase1_objects.png)

---

## Phase 2: Tree Objects

### Description
Implemented tree structure for directories with serialization.

### Output
![Tree](images/phase2_test.png)
![Hex](images/phase2_xxd.png)

---

## Phase 3: Index (Staging Area)

### Description
Implemented staging area using a text-based index file.

### Output
![Status](images/phase3_status.png)
![Index](images/phase3_index.png)

---

## Phase 4: Commits and History

### Description
Implemented commit creation and log functionality.

### Output
![Log](images/phase4_log.png)
![Objects](images/phase4_objects.png)
![HEAD](images/phase4_head.png)

---

## Analysis Answers

### Q5.1
A branch is a file storing commit hash. Checkout updates HEAD and working directory.

### Q5.2
Dirty working directory is detected by comparing index metadata with working directory.

### Q5.3
Detached HEAD commits are not linked to branch but can be recovered via hash.

### Q6.1
Use graph traversal from branch heads to identify reachable objects.

### Q6.2
Garbage collection must avoid deleting objects used by active commits; Git uses locking.

---
