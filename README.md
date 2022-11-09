# Using-SQLite-for-a-data-warehouse
Client/server SQL database engines strive to implement a shared repository of enterprise data. They emphasize scalability, concurrency, centralization, and control. SQLite strives to provide local data storage for individual applications and devices. SQLite emphasizes economy, efficiency, reliability, independence, and simplicity.

**Situations Where SQLite Works Well**  
- Embedded devices and the internet of things  
- on-disk file format for desktop applications such as version control systems, financial analysis tools, media cataloging and editing suites, CAD packages, record keeping programs, and so forth.  
- SQLite works great as the database engine for most low to medium traffic websites, enerally speaking, any site that gets fewer than 100K hits/day should work fine with SQLite.  
- Data analysis:  Raw data can be imported from CSV files, then that data can be sliced and diced to generate a myriad of summary reports. More complex analysis can be done using simple scripts written in Tcl or Python.  
- Many applications use SQLite as a cache of relevant content from an enterprise RDBMS. This reduces latency, since most queries now occur against the local cache and avoid a network round-trip. It also reduces the load on the network and on the central database server.

**Checklist For Choosing The Right Database Engine**  
- Is the data separated from the application by a network? → choose client/server
- Many concurrent writers? → choose client/server
- Big data? → choose client/server
- Otherwise → choose SQLite!
