# Iceberg Catalogs: Your Central Hub 🧊

Welcome to the Iceberg Catalogs repository! This is your one-stop shop for information about Iceberg catalogs, their features, and how to choose the right one for your data lakehouse.

## Iceberg 

**What is Apache Iceberg?**

Iceberg is an open table format for storing large, analytical datasets. It works seamlessly with poplar engines like Spark, Trino, Flink, Presto,etc.

**Why use Apache Iceberg?**

As organizations grow, their technology stacks and data processing needs evolve. Traditional data pipelines involving data lakes and warehouses often lead to data duplication, quality issues, and expensive maintenance.

Iceberg benefits:

- **Eliminates ETL:** Query data directly without complex data movement and duplication, reducing costs and improving data freshness.
- **Supports Diverse Engines:** Easily use different engines (e.g., Spark, Trino) for varying use cases like analytics or real-time queries, promoting flexibility and efficiency.
- **Cloud and Vendor Agnostic:** Not tied to any specific cloud provider or data warehouse vendor, offering freedom of choice and avoiding lock-in.
- **Reduces Storage Costs:** By eliminating the need for data duplication and optimizing storage formats, Iceberg can significantly reduce storage costs in cloud environments.

In essence, Apache Iceberg simplifies data pipelines, improves efficiency, enhances flexibility, and reduces costs in the ever-changing technology landscape.



## Iceberg catalogs

In the Iceberg ecosystem, catalogs play a crucial role in managing and organizing your tables. They store metadata about your tables, making them discoverable and accessible to query engines and other tools.

# Catalog Comparison

| Catalog                | Open Source | Approx. Release Date | Key Features                                                              | Ideal Use Cases                                                                                                                                                                                            | URLs                                                                                             |
| ---------------------- | ----------- | -------------------- | ------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Unity Catalog          | ✅          | 2023                 | Universal catalog for data and AI, supports any format, engine, and asset | Multi-format, multi-engine, and multi-asset environments, data and AI asset management, unified access and discovery                                                                                       | [Unity Catalog](https://docs.databricks.com/data-governance/unity-catalog/index.html)            |
| Polaris Catalog        | ✅          | 2022                 | Built on Iceberg's REST API, supports cross-engine operations (read/write)| Multi-engine environments, preventing vendor lock-in, focus on data sharing and interoperability                                                                                                           | [Polaris Catalog](https://polaris.example.com)                                                    |
| Nessie Catalog         | ✅          | 2021                 | Transactional, git-like version control (branching, tagging, merging), auditing | Collaborative environments, scenarios where version control, rollback, and auditing of table changes are important                                                                                       | [Nessie Catalog](https://projectnessie.org)                                                      |
| REST Catalog           | ✅          | 2020                 | Server-side, accessible via REST API, highly scalable, easy to integrate  | Cloud environments, flexible integration needs, large-scale deployments                                                                                                                                    | [REST Catalog](https://iceberg.apache.org/rest/)                                                 |
| Hive Metastore Catalog | ✅          | 2019                 | Leverages existing Hive Metastore, seamless Hive integration              | Existing Hive environments, unified catalog with Hive tools, scenarios requiring compatibility with Hive workflows                                                                                        | [Hive Metastore Catalog](https://cwiki.apache.org/confluence/display/Hive/AdminManual+Metastore) |
| Hadoop Catalog         | ✅          | 2019                 | Stores metadata in HDFS, compatible with the Hadoop ecosystem             | Existing Hadoop environments where HDFS is primary storage                                                                                                                                                | [Hadoop Catalog](https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/HdfsUserGuide.html) |
| JDBC Catalog           | ✅          | 2019                 | Stores metadata in a JDBC database, lightweight, easy to set up           | Smaller deployments, environments where a simple database-like catalog is sufficient                                                                                                                      | [JDBC Catalog](https://iceberg.apache.org/jdbc/)                                                |
| GCP Data Catalog       | ❌          | 2021                 | Metadata management, discovery, data lineage, integration with GCP services| GCP-centric environments, leveraging existing GCP infrastructure, comprehensive metadata management                                                                                                       | [GCP Data Catalog](https://cloud.google.com/data-catalog)                                        |
| AWS Glue Catalog       | ❌          | 2020                 | Serverless, integrates with other AWS services, scales automatically       | AWS-centric environments, leveraging existing AWS infrastructure, serverless architecture                                                                                                                 | [AWS Glue Catalog](https://aws.amazon.com/glue)                                                  |
| Azure Purview          | ❌          | 2020                 | Data governance, discovery, classification, lineage, integration with Azure| Azure-centric environments, strong focus on data governance and compliance                                                                                                                                | [Azure Purview](https://azure.microsoft.com/en-us/services/purview/)                             |

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

