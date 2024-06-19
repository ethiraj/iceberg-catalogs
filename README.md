# Iceberg Catalogs: Your Central Hub 🧊

Welcome to the Iceberg Catalogs repository! This is your one-stop shop for information about Iceberg catalogs, their features, and how to choose the right one for your data lakehouse.

## Introduction

In the Iceberg ecosystem, catalogs play a crucial role in managing and organizing your tables. They store metadata about your tables, making them discoverable and accessible to query engines and other tools.

# Catalog Comparison

| Catalog             | Open Source | Key Features                                                              | Ideal Use Cases                                                                                                                                                                                               |
| ------------------- | ----------- | ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| REST Catalog        | ✅          | Server-side, accessible via REST API, highly scalable, easy to integrate     | Cloud environments, flexible integration needs, large-scale deployments                                                                                                                                       |
| Hive Metastore Catalog | ✅          | Leverages existing Hive Metastore, seamless Hive integration                   | Existing Hive environments, unified catalog with Hive tools, scenarios requiring compatibility with Hive workflows                                                                                           |
| Hadoop Catalog       | ✅          | Stores metadata in HDFS, compatible with the Hadoop ecosystem                  | Existing Hadoop environments where HDFS is primary storage                                                                                                                                                 |
| JDBC Catalog        | ✅          | Stores metadata in a JDBC database, lightweight, easy to set up             | Smaller deployments, environments where a simple database-like catalog is sufficient                                                                                                                          |
| Nessie Catalog       | ✅          | Transactional, git-like version control (branching, tagging, merging), auditing | Collaborative environments, scenarios where version control, rollback, and auditing of table changes are important                                                                                          |
| Polaris Catalog     | ✅          | Built on Iceberg's REST API, supports cross-engine operations (read/write)   | Multi-engine environments, preventing vendor lock-in, focus on data sharing and interoperability                                                                                                              |
| Project Nessie      | ✅          | Full-fledged REST API, enhanced branching/merging, fine-grained permissions  | Complex data workflows, collaboration at scale, advanced version control requirements                                                                                                                          |          
| AWS Glue Catalog     | ❌          | Serverless, integrates with other AWS services, scales automatically          | AWS-centric environments, leveraging existing AWS infrastructure, serverless architecture                                                                                                                        |
| Azure Purview        | ❌          | Data governance, discovery, classification, lineage, integration with Azure   | Azure-centric environments, strong focus on data governance and compliance                                                                                                                                     |
| GCP Data Catalog    | ❌          | Metadata management, discovery, data lineage, integration with GCP services    | GCP-centric environments, leveraging existing GCP infrastructure, comprehensive metadata management                                                                                                          |

## Choosing the Right Catalog

Selecting the best catalog for your needs depends on several factors:

*   **Environment:** Cloud vs. on-premises, existing tools and infrastructure.
*   **Scale:** The size and growth of your data.
*   **Features:** Version control, auditing, transactionality, ease of integration.
*   **Complexity:** Your desired level of catalog management complexity.

Refer to the detailed descriptions and examples in the respective catalog folders for more information.

## Additional Resources

*   [Iceberg Documentation on Catalogs](https://iceberg.apache.org/concepts/catalog/)
*   [Blog posts and tutorials on specific catalogs]
  
## Contributing

Your contributions are welcome! If you have insights, examples, or code related to Iceberg catalogs, please open a pull request. Let's build a valuable knowledge base for the community.

Let's make this a valuable resource for the Iceberg community!

