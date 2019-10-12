Hive Data Model

	• The metadata repository of Hive known as Hive MetaStore consists of namespaces, object definitions, and the details of underlying data.
	• A Hive schema or database in Hive is essentially a namespace that holds metadata information for a set of tables.
	• A schema and a database are synonyms in term of Hive. At filesystem level, it is a directory under which all internal tables that belong to that namespace are stored. 
	• Hive also has a concept of external tables in which the files might exist in other locations in HDFS.
	• The top-level directory is defined in hive-site.xml  hive.metastore.warehouse.dir parameter. The default value of this parameter is /apps/hive/warehouse. This can be changed by admin
	• When HIVE is installed, a default database called default is created. 
		○ Default database does not have its own directly. 
		○ Tables created in default database are stored in top-level directory 
		○ For external tables, metadata information is stored in Hive Metastore and data is in their own directory in HDFS.
