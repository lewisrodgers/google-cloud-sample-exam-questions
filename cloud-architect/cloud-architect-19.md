# cloud-architect-19

The database administration team has asked you to help them improve the performance of their new database server running on Compute Engine. The database is used for importing and normalizing the company’s performance statistics. It is built with MySQL running on Debian Linux. They have an n1-standard-8 virtual machine with 80 GB of SSD zonal persistent disk which they can't restart until the next maintenance event. What should they change to get better performance from this system as soon as possible and in a cost-effective manner?

A. Increase the virtual machine’s memory to 64 GB.

B. Create a new virtual machine running PostgreSQL.

C. Dynamically resize the SSD persistent disk to 500 GB.

D. Migrate their performance metrics warehouse to BigQuery.

## Feedback

A is not correct because increasing the memory size requires a VM restart.

B is not correct because the DB administration team is requesting help with their MySQL instance. Migration to a different product should not be the solution when other optimization techniques can still be applied first.

C is correct because persistent disk performance is based on the total persistent disk capacity attached to an instance and the number of vCPUs that the instance has. Incrementing the persistent disk capacity will increment its throughput and IOPS, which in turn improve the performance of MySQL.

D is not correct because the DB administration team is requesting help with their MySQL instance. Migration to a different product should not be the solution when other optimization techniques can still be applied first.

https://cloud.google.com/compute/docs/disks/#pdspecs

https://cloud.google.com/compute/docs/disks/performance