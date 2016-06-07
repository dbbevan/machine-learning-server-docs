#Microsoft R Server 2016 Release notes

The following release notes apply to Microsoft R Server.

##Microsoft R Server 2016

**New in this Release**

+ 

+ DeployR includes the following changes and improvements:
    - Deployr Enterprise is more secure than ever with improved Web security features for better protection against malicious attacks, improved installation security, and improved Security Policy Management.
    - DeployR Enterprise now relies on an H2 database by default and allows you to easily use a SQL Server or PostgreSQL database instead to fit your production environment. 
    - DeployR Enterprise now has a simplified installer for a better customer experience.
    - Documentation is now available on MSDN.
    - The XML format for data exchange is not deprecated, but it will be removed from future versions of DeployR.
    - This release is of DeployR Enterprise only.


**Bug Fixes**

##Microsoft R Server 8.0.0

**New Features in this Release**

This guide is an introduction to using the new features of Microsoft R Services. The current release is Microsoft R Services 2016, which includes the following new features:

+ Revolution R Open is now Microsoft R Open, and Revolution R Enterprise is now generically known as Microsoft R Services, and specifically Microsoft R Server on Linux platforms.

+ Microsoft R Services installs on top of an enhanced version of R 3.2.2, Microsoft R Open for Revolution R Enterprise 8.0.0 (on Windows) or Microsoft R Open for Microsoft R Server (on Linux)

+ Installation of Microsoft R Services has been simplified from three installers to two: the new Microsoft R Open for Revolution R Enterprise/Microsoft R Server installer combines Microsoft R Open with the GPL/LGPL components needed to support Microsoft R Services, so there is no need for the previous “Revolution R Connector” install.

+ RevoScaleR includes:
    + New Fuzzy Matching Algorithms: The new rxGetFuzzyKeys and rxGetFuzzyDist functions provide access to fuzzy matching 
algorithms for cleaning and analyzing text data.
    + Support for Writing in ODBC Data Sources. The RxOdbcData data source now supports writing
    + Bug Fixes: 
        + When using rxDataStep, new variables created in a transformation no longer inherit the rxLowHigh attribute of the variable used to create them.
        + rxGetInfo was failing when an extended class of RxXdfData was used.
        + rxGetVarInfo now respects the ‘newName’ element of colInfo for non-xdf data sources.
        + If ‘inData’ for rxDataStep is a non-xdf data source that contains a colInfo specification using ‘newName’, the ‘newName’ should now be used for ‘varsToKeep’ and ‘varsToDrop’.
    + Deprecated and Defunct. 
        + ‘NIEDERR’ is no longer supported as a type of random number generator.
        + ‘scheduleOnce’ is now defunct for rxPredict.rxDForest and rxPredict.rxBTrees.
        + The compute context ‘RxLsfCluster’ is now defunct.
        + The compute context ‘RxHpcServer’ is now deprecated

+ DevelopR - The R Productivity Environment (the IDE provided with Revolution R Enterprise on Windows) is not deprecated, but it will be removed from future versions of Microsoft R Services.

+ RevoMPM, a Multinode Package Manager, is now defunct, as it was deemed redundant. Numerous distributed shells are available, including pdsh, fabric, and PyDSH. More sophisticated provisioning tools such as Puppet, Chef, and Ansible are also available. Any of these can be used in place of RevoMPM.

+ Known Issues: http://go.microsoft.com/fwlink/?LinkID=717964&clcid=0x409