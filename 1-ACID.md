# ACID Transaction

ACID Transaction (Atomicity, Consistency, Isolation, Durability)

### Transcation
- Any poeration that is treated as a single unit, which either completes fully or does not complete at all and leaves system in a consistent state. 

#### Example

- Transfer Money from A to B, if it fails, both A and B should be in the same state and there's no an in-between state.

## ACID Properties
- Atomicity
- Consistency
- Isolation
- Durability

>> ACID Properties are the core properties of ACID transactions.  
if a database operation has these ACID properties, it is referred as an ACID transaction, a data storage that apply the ACID properties is said to be a transactional database. 


ACID transactions gurantee that each read,write and modification meet the folowing properties:
### Atomicity

Each statement in  a transaction (read, write,update or delete data)is treated as a single unit, which is either executed or not. 

It involves the following two operations:

- Commit: If a transaction commits, changes are made visible.

- Abort: If a transaction aborts, changes made to the database are not visible.

This property prevents data loss and corruption from occurring.


### Consistency

 Ensures that the database remains in a consistent state before and after transaction. 
 It guarantees that any transaction will take the database from one consistent state to another consistent state maintaining the rules and constraints defined to the data.

### Isolation

This property ensures that multiple transactions can occur concurrently without leading to the inconsistency of the database.  
Changes occurring in one transaction should not be visible in any another transaction until a change in that transaction is committed.  
This property ensures that when multiple transactions run at the same time, the result will be the same as if they were running one after the other.

### Durability

This property ensures that modifications and updates on the database will be permanently stored in the disk. 
It means that if a transaction is committed, the changes made to the database will not be lost even if the database is shut down or the system fails. 

 
## Advantages of ACID properties in DBMS

- **Data  Consistency: **ACID properties ensure that the data remains consistent and accurate after any transaction execution.

- **Data Integrity:**  ACID properties maintain the integrity of the data by ensuring that any changes to the database are permanent and cannot be lost.

- **Concurrency Control:** ACID properties help multiple transactions occurring concurrently by preventing interference between them.

- **Recovery:** ACID properties ensure that in case of any failure or crash, the system can recover the data up to the point of failure or crash.





## Disadvantages of ACID properties in DBMS

- **Performance:** ACID properties can lead to performance issues due to the additional task involved in implementing integrity and concurrency control.

- **Scalability:** ACID properties can make cause scalability issues in large distributed systems where multiple transactions can occur concurrently.

- **Complexity:** Implementing ACID properties to a database can cause complexity of the system and requires additional resources and tools.


## Conclusion

ACID properties involves four properties, Atomicity, Consistency, Isolation and Durability. **Atomicity** ensures that that the transaction is rolled back if any part fails. **Consistency** ensures the database remains consistent before and after the transaction. **Isolation** ensures that one transaction does not affect another one. **Durability** Ensures that the the database persist even after the system failure