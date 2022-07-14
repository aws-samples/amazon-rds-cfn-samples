## AWS Cloufdormation Templates for Aadhaar Data Vault Reference Architecture 

This repository contains the sample cloudformation templates for creating MySQL and PostgreSQL RDS
The cloudformation templates for MYSQL and PostgreSQL automates creation of Multi-AZ encrypted RDS instance in your chosen VPC. Below are key default properties set in the templates:
MySQL Version- 8.0.28 
PostgreSQL Version- 14.2
Backup retention period in days- 7
Instance type- db.t3.large 
PubliclyAccessible: 'false' 
StorageEncrypted: 'True' 
StorageType: gp2 
Allocated Storage- 20 GB
Multi-AZ: 'True' 
MySQL Default port- 3306
PostgreSQL Default port- 5432
DBInstanceIdentifier- 'AadhaarVaultDBServer'
DBName- 'AadhaarDB'

These templates can use used to create RDS instances in AWS VPC with two 'Private Subnets'. A KMS key ARN is required for the encryption at rest.
Post creation, users can change the properties of the database instance by using "Modify" option in AWS RDS console.
Users can download and further modify these templates to suite their specific needs. Recommended way is to open the template in cloudformation designer and edit the content. This way, it is easier to track and fix any errors introduced during editing process.

NOTE- These templates are only provided as a reference and are not officially part of AWS documentation.


## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

