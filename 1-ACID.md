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

 




