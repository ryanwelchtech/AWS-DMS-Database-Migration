# AWS Database Migration Project

This project demonstrates the migration of a WordPress application from an on-premises environment to AWS using AWS Database Migration Service (DMS). The on-premises environment was simulated using EC2 instances, and the migration involved moving both the application files and the database to AWS.

## Project Overview
The project consisted of five stages:
1. **Provision the Environment**: Created the on-premises and AWS infrastructure using CloudFormation.
2. **Establish Private Connectivity**: Set up VPC peering and configured routing between on-premises and AWS environments.
3. **Create AWS Infrastructure**: Deployed an RDS MariaDB instance and an EC2 instance for the WordPress application.
4. **Migrate Database & Cutover**: Used AWS DMS to migrate the database and updated the application to point to the new RDS endpoint.
5. **Cleanup**: Removed all AWS resources to ensure cost efficiency.

## Key Steps
- **Infrastructure Setup**: Used CloudFormation to provision EC2 instances for the on-premises environment and AWS infrastructure.
- **VPC Peering**: Established secure connectivity between on-premises and AWS VPCs.
- **RDS Deployment**: Created a highly available MariaDB instance on RDS.
- **Database Migration**: Used AWS DMS to replicate and migrate data from the on-premises database to RDS.
- **Application Migration**: Migrated WordPress files using SCP and updated the application configuration.
- **Testing & Validation**: Verified the application functionality post-migration.
- **Cleanup**: Deleted all resources to avoid unnecessary costs.

## Platforms and Technologies
- **AWS Services**: EC2, RDS, DMS, VPC, CloudFormation, IAM, Session Manager.
- **Database**: MariaDB.
- **Web Server**: Apache HTTP Server.
- **Scripting**: Bash, PHP.
- **Tools**: SCP, MySQL CLI.

## How to Use
1. Follow the detailed guide provided in the project documentation.
2. Ensure all prerequisites (e.g., AWS account, IAM permissions) are met.
3. Execute the steps in each stage sequentially.

## License
This project is open-source and available under the MIT License.
