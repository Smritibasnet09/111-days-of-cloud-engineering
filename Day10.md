**Day 10 of #111CodeForChange 🚀**
**Topic: Amazon RDS & Aurora**

Today I learned about **Amazon RDS (Relational Database Service)** and **Amazon Aurora**, and how AWS simplifies database management in the cloud.

🔹 **Amazon RDS (Relational Database Service)**

* Fully managed service to set up, operate, and scale databases
* AWS handles backups, patching, and maintenance
* Supports multiple database engines: PostgreSQL, MySQL, MariaDB, Oracle, SQL Server, IBM Db2
* Also includes Amazon’s own high-performance database: **Aurora**

🔹 **Key Concepts**

* **Multi-AZ Deployment**
  → Provides high availability & disaster recovery
  → Not used for scaling workload

* **Read Replicas**
  → Used for scaling read operations
  → Data is asynchronously copied from primary DB

🔹 **Amazon Aurora**

* High-performance relational database built by AWS
* Supports global databases (Global Aurora)
* Better scalability and availability compared to standard RDS

🔹 **Backups in RDS**

* Automated backups (continuous)
* Manual backups (snapshots)

🔹 **Caching & Performance**

* **Memcached** → Multi-threaded, simple caching
* **Redis** → More advanced, supports persistence & complex data
* **TTL [Time to live]** → Defines how long cached data stays valid

🔹 **Other Concepts**

* Forward Proxy & Reverse Proxy basics for handling requests efficiently

**Key Takeaway:**
RDS makes database management easier, while Aurora takes performance and scalability to the next level.

