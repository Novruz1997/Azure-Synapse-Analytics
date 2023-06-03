# Azure-Synapse-Analytics

Serverless SQL pool is a serverless distributed query engine that you can sue to query data over your data lake using T-Sql

It uses Driver-Node Worker Node architecture. 


It uses Polaris Engine in Backend. 

It is serverless = No Infrastructure. 
Dsitributed Query Engine - Polaris
Query Using T-SQL.
Pay-Per-Query pricing model.
Not a Storage. = Serverless Sql Pool Cannot Create Tables, instead it creates external Tables.
With Synapse Link - We can query Cosmos DB containers from Serverless Sql Pool.
Serverless Sql Pool - Can Query Spark Tables (With ReplicatedDB)

Serveless Sql Pool - Support file reads directly from - Azure Storage Account (Delimited, JSON, Parquet, Delta Lake), Cosmos DB (Via Synapse Link (Only SQL Api, MongoDB API)).


Most Use Cases of Serverless Sql Pool:
	1. Discovery & Exploration
	2. Logical Data Warehouse on TOp of Data in Data Lake. (Via Ext Tables, Views)...
	3. Data Transformations.



Cost Calculation:
	Billed for Data Processed
		- Amount of data read from storage (Partition Query is efficient, read from the single partition less costly)
		- Amount of data in intermediate results
		- Amount of data written to storage
	Minimum of 10 MB per query.
	Currently 6.25$ per 1TB.
	Synapse Studio Provides UI for cost control.
