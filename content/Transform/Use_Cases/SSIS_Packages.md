# SSIS Packages

SSIS is the ETL (extraction, transformation and load) method for SQL
2012 and 2014. SSIS packages are created in Management Studio using a
SQL Server Import and Export Wizard and requires licensing on both web
and database servers. They can also be created in Visual Studio 2012 or
2014 Development Studio using Integration Services Project.

One of the functions of Management Studio is to handle the storage of
import packages although it is not intended to be the design environment
for SSIS. However, as of SQL 2012, the standard installation does not
include the Business Intelligence Development Studio. To access a
package, the SSIS packages must be saved as files that can be opened in
Management Studio. This allows the ‘Create Table’ code of the SSIS
packages to be deleted from Management Studio. In addition, SQL Server
Data Tools, accessible through Visual Studio, also opens the SSIS
package files and allows further development.

SSIS packages are also saved with passwords. The Package Protection
Level is Encrypt sensitive data with password.

Another important difference is that SSIS package names do not contain
periods (.), which deviates from the standard naming convention. All
periods(.) must be removed from SSIS package names and replaced with
underscores. For example, TransformMMxx.dbo.stLFA1.BPCS.imp becomes
TransformMMxx\_dbo\_stLFA1\_BPCS\_imp.
