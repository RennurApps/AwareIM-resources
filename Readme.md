# Aware IM Server Stack
## Servers, Components, Frameworks, Dependencies and other resources
------------------------------------------------------------------------------------------------------------------------------------

> Aware IM is a rapid low-code application development tool that lets you create powerful aesthetically appealing web applications quickly.

*   [**Changelog**](http://www.awareim.com/changelog/?C=M;O=D)

#### Software

Written in 100% Java programming language. Aware IM is based on the plethora of Java technologies such as J2EE application server, JDBC, JMS, JSP/servlets technology, web services etc. These are robust technologies that have been proven in the industry.

<!-- Links to tutorials, documentation, events, apps have been moved [**here**](https://github.com/RennurApps/AwareIM-Help) --> 

*   [**Currently v8.4 build 2722**](https://www.awareim.com/changelog/Readme2722.txt) - 4 April, 2020.
    
    *   **New Features in version 8.4**
        *    Support for PostgreSQL
        *    Support for barcodes and QRcodes in the Report Designer
        *    Report Preview in the Report Designer
        *    Runs under Java 12/13 envirnonement
    *   8.4 Recent Improvements
        *   2720 - New function CR() returns a newline symbol \\n
        *   2714 - Predefined FileItem object can now be specified as process input
        *   2713 - TO\_TIMEZONE function
        *   2713 - Tab order of -1 can now be specified
        *   2711 - Image Gallery operation available to Custom Checkbox Lists
        *   2711 - Control Panel toolbar
        *   2711 - Improvements for auto-incremented numbers
            *   NEXT\_SEQUENCE\_NMB function
        *   2711 - Log improvements
        *   2710 - [Improvements](https://www.awareim.com/changelog/Readme2710.txt)
        *   2709 - Queries can now be defined using EXEC\_SQL statement
        *   2709 - Support for the latest version of PhoneGap build
        *   2705 - [List of improvements](https://www.awareim.com/changelog/Readme2705.txt)
*   v8.3
    
    *   **New Features in version 8.3**
        *    Relationships diagrams with the ability to edit relationships
        *    Process diagrams with the ability to show sub-processes
    *   8.3 Recent Improvements
        *   2629 - Ability to specify a script for Google Maps in visual perspectives
        *   2623 - Support for attributes that hold and display color
            *   1.  You define a text attribute with the property "Content" (former "Format") set to "Color" rather than default setting of "STANDARD"
            *   2.  If you put this attribute on a form Aware IM will generate a color-picker widget, rather than the standard text box. At runtime the user will be able to pick a color as the value for this attribute
            *   3.  You can then use this color in tag expressions at various places in the system - in HTML, attribute styles etc.  
                    For example, in HTML:  
                    `<div style="background-color:&lt;&lt;MyObject.ColorAttr&gt;&gt;"></div>`
            *   4.  If used in queries the system by default will display color boxes with actual colors
        *   2623 - Support for Swap-Select widget resize
        *   2621 - Graphic resizing of form width, label width, control width and column width
        *   2616 - It is now possible to disallow access to 'model' to configuration users
        *   2615 - Predefined elements use default output target for the content panel
*   v8.2
    
    *   **New Features in version 8.2**
        *    Multi-developer mode
        *    SAML support (Single Sign On framework)
        *    Custom HTML forms
        *    Kanban boards
    *   **Recent Improvements in version 8.2**
        *   2572 - Push notifications: GCM deprecated and replaced with FCM
            *   [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)
        *   2570 - "No data found" message displayed for custom queries if there is no data
        *   2565 - Ability to specify a script for modeless windows
        *   2562 - Documents used inside HTML cells return file name and so can now be displayed inside an IFRAME
        *   2562 - Values for Kanban columns support tag expressions
        *   2561 - It is now possible to capture HTTP response codes in REST

*   [**Version History**](http://www.awareim.com/changelog/?C=M;O=D)
    *   ✔️ **Currently v8.4** - Builds 2705+
        *   [Aware IM 8.4 released](https://www.awareim.com/aware-im-8-4-released/) - Released October 24, 2019
    *   **8.3** - Builds 2613-2631
        *   [Aware IM 8.3 released](https://www.awareim.com/aware-im-8-3-released/) - Released May 23, 2019
    *   **8.2** - Builds 2559-2574
        *   [Aware IM 8.2 released](https://www.awareim.com/aware-im-8-2-released/) - Released October 25, 2018
    *   **v8.1** - Builds 2452-2477
        *   [Aware IM 8.1 released](https://www.awareim.com/aware-im-8-1-released/) - Released April 19, 2018
        *   [Version 8.1 Overview - Youtube video](https://www.youtube.com/watch?v=sp4OvLR5ALI) - Aware IM version 8.1 features overview.
    *   **v8.0** - Builds 2341-2378
        *   [Aware IM 8.0 released](https://www.awareim.com/aware-im-8-0-released/) - Released August 3, 2017
        *   [Version 8.0 Overview - Youtube video](https://www.youtube.com/watch?v=NHvKFZHhADg) - Overview of the new Aware IM version 8.0 (Jun 28, 2017)
    *   **v7.1** - Builds 2223-2240
        *   [Aware IM 7.1 released](http://www.awareim.com/aware-im-7-1-released/) - Released September 6, 2016
    *   **v7.0** - Builds 2144-2181
        *   [Aware IM 7.0 released](http://www.awareim.com/aware-im-7-0-released/) - Released February 8, 2016
            *   [Watch a video about version 7.0](https://youtu.be/p5Q-YYAd6Fs)
    *   **v6.0** - Builds 2010-2056
        *   [Aware IM 6.0 released](http://awareim.com/aware-im-6-0-released/) - Released January 9, 2015
    *   **v5.9** - Builds 1881-1908
        *   [Aware IM 5.9 released](http://awareim.com/aware-im-5-9-released/) -
            *   Improvements
                *   **User Defined Processes/Workflows** - Ability for the administrator of end user to control access levels settings
                    *   How To (PDF) - Page 47
                    *   [Forum post](http://www.awareim.com/forum/viewtopic.php?t=7091)
    *   **v5.8** - Builds 1797-1814
        *   [Aware IM 5.8 released](http://www.awareim.com/aware-im-5-8-released/)
    *   **v5.7** - Builds 1691-1719
    *   **v5.6** - Builds 1638-1671
    *   **v5.5** - Builds 1588-1617

#### [](#operating-system)Operating System

*   Windows
*   Mac
*   Linux

#### [](#application-server)Application Server

##### [](#apache-tomcat)Apache Tomcat

> Disclaimer: Use this information and instructions at your own risk. There is no support provided for any of the updates performed outside of default Aware IM installation.

> Caution: Installing Aware IM update (Setup.exe), overwrites and resets Tomcat & JDK folders back to default. In fact, all files are replaced during update. Always keep all new and amended files incl. images separately and copy+paste them back once the install is complete.

> Tomcat 8.5.24 32bit is the default version packaged in the **Aware IM 8.1+** server installation.

> Tomcat 8.0.14 32bit is the default version packaged in the **Aware IM 6.0-8.0** server installation.

> Tomcat 6.0.35 32bit is the default version packaged in the **Aware IM 5.9** server installation.

*   [**Tomcat 9.0.36** - For Aware IM v8.x](http://tomcat.apache.org/) - 3 June, 2020. Tomcat 9 is designed to run on **`Java SE 8`** or later.
    *   ✔️ [**Download Tomcat v9**](https://tomcat.apache.org/download-90.cgi) - 64bit recommended. Manual Install. Tested and working with Aware IM versions `6.x`, `7.x` & `8.x`.
        *   [**Migrating to v9.0.x**](https://tomcat.apache.org/migration-9.html)
        *   [**Security**](https://tomcat.apache.org/security-9.html)
            *   **Important fixes**
                *   `9.0.36` HTTP/2 DoS `CVE-2020-11996` - Affects: 9.0.0.M1 to 9.0.35
                *   `9.0.35` Remote Code Execution via session persistence `CVE-2020-9484` - Affects: 9.0.0.M1 to 9.0.34
                *   `9.0.31` AJP Request Injection and potential Remote Code Execution `CVE-2020-1938` - Affects: 9.0.0.M1 to 9.0.30
                *   `9.0.20` Denial of Service `CVE-2019-10072` - Affects: 9.0.0.M1 to 9.0.19
                *   `9.0.19` Remote Code Execution on Windows `CVE-2019-0232` - Affects: 9.0.0.M1 to 9.0.17
                *   `9.0.16` Denial of Service `CVE-2019-0199` - Affects: 9.0.0.M1 to 9.0.14
                *   `9.0.10` Information Disclosure `CVE-2018-8037`
                *   `9.0.8` A bug in the UTF-8 decoder can lead to DoS `CVE-2018-1336`
                *   `9.0.5` Security constraint annotations applied too late `CVE-2018-1305`
                *   `9.0.5` Security constraints mapped to context root are ignored `CVE-2018-1304`
                *   `9.0.1` Remote Code Execution `CVE-2017-12617`
        *   **Installation** with Aware IM
            *   Windows Based Systems
                *   **IMPORTANT**:
                    *    Ensure any prior modification of existing _web.xml_ and _server.xml_ configurations are not overwritten with the new version. There are configuration changes in the latest version of Tomcat relating to those two files.
                *   **Installation Steps** - Stop the Aware IM server before updating Tomcat. Do **not** delete your current C:\\AwareIM\\Tomcat folder.
                    1.  **Extract** the archive and open the folder.
                    2.  Open the extracted **Tomcat** folder.
                    3.  Select all files and folders and press `Crl+c` to copy
                    4.  Open you AwareIM installation Tomcat folder **C:\\AwareIM\\Tomcat**
                    5.  Press `Ctrl+v` to paste and replace all files and folders.
                    6.  Java JDK tools.jar:
                        *   **In v8.3+**, if you have updated Java JDK, copy the latest version of tools.jar to the C:\\Awareim\\lib folder to replace the old one.
                        *   **In v8.2 and below**, if you have updated Java JDK, copy the latest version of tools.jar to the C:\\Awareim\\Tomcat\\lib folder to replace the old one.
                    7.  Rename or delete **ROOT** folder - _This is optional_. You can use this folder to store your own favicon.ico, error pages and other HTML/CSS/JS home page files.
    *   [Tomcat 9 Documentation](https://tomcat.apache.org/tomcat-9.0-doc/index.html).
    *   [Tomcat 9 Changelog](https://tomcat.apache.org/tomcat-9.0-doc/changelog.html).
*   [**Tomcat 8.5** - For Aware IM v6.0+](http://tomcat.apache.org/) - **Latest release is Tomcat v`8.5.54`** 3 Apr, 2020. (Aware IM bundled version `8.5.24`) - Tomcat 8.5 requires **`Java SE 7`** or later.
    *   [**Download Tomcat**](https://tomcat.apache.org/download-80.cgi)
    *   [**Security**](https://tomcat.apache.org/security-8.html)
    *   [**Migrating to v8.5.x**](https://tomcat.apache.org/migration-85.html)
    *   [Tomcat 8.5.x Documentation](https://tomcat.apache.org/tomcat-8.5-doc/)
    *   [Tomcat 8.5x Changelog](https://tomcat.apache.org/tomcat-8.5-doc/changelog.html)
*   [**Tomcat 6 (archived)** - For Aware IM v5.9 Only](http://tomcat.apache.org/) - Apr 2 2017 **Final version Tomcat 6.0.53**
    *   [Download Tomcat **v6** - Aware IM v5.9 Only](https://archive.apache.org/dist/tomcat/tomcat-6/v6.0.53/) - Support for Apache Tomcat 6.0.x has ended on 31 December 2016.
*   **Tomcat SSL/TLS Configuration HOW-TO** - Tomcat documentation.
    *   [**v9.0**](http://tomcat.apache.org/tomcat-9.0-doc/ssl-howto.html)
    *   [**v8.5**](http://tomcat.apache.org/tomcat-8.5-doc/ssl-howto.html)
    *   [Forum Post](http://www.awareim.com/forum/viewtopic.php?t=3554)

#### [](#java-jdk)Java JDK

*   [**OpenJDK Java SE Releases**](https://jdk.java.net) - Oracle provides the latest **OpenJDK** releases under the open source.
    
    *    [**Oracle OpenJDK `14`**](https://jdk.java.net/14/)
    *    [Oracle OpenJDK `13`](https://jdk.java.net/13/)
    *    [Oracle OpenJDK `12`](https://jdk.java.net/12/) - JDK 12 has been superseded.
    *    [Archived Versions](https://jdk.java.net/archive/)
*   [**Commercial Java SE Development Kit (JDK)**](https://www.oracle.com/technetwork/java/javase/overview/index.html) - [Important Oracle JDK License Update starting April 16, 2019](https://www.oracle.com/technetwork/java/javase/overview/oracle-jdk-faqs.html)
    
    *    [Version `14.0.1`](https://www.oracle.com/technetwork/java/javase/downloads/index.html#JDK14) - April 14, 2020
        *   **Not tested with Aware IM**
    *    [Version `11.0.7`](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) - April 14, 2020.
        *   **Not tested with Aware IM**
    *    ✔️ [**Version 8, Update 251**](https://www.oracle.com/java/technologies/javase-downloads.html#JDK8) - `1.8.0_251-b08` 14 April, 2020. **Compatible with all Aware IM versions**.
        *   More Download links found at [https://lv.binarybabel.org/catalog/java/jdk8](https://lv.binarybabel.org/catalog/java/jdk8)
    *    Versions bundled with Aware IM:
        *   Aware IM `v8.0+` - JDK 8 Update 91 `1.8.0_91-b15`
    *    [**All previous JDK versions archive**](https://www.oracle.com/technetwork/java/javase/archive-139210.html)
        *   [Manual Downloads](https://java.com/en/download/manual.jsp)
*   [**JavaMail**](https://javaee.github.io/javamail/) - JavaMail **`1.6.2`** - August 30, 2018 Final Release. Platform-independent and protocol-independent framework to build mail and messaging applications.
    
    *   [Changes](https://javaee.github.io/javamail/docs/CHANGES.txt)
    *   [Releases](https://github.com/javaee/javamail/releases)
    *   **Download JavaMail**
        *   [**javax.mail.jar**](https://github.com/javaee/javamail/releases/download/JAVAMAIL-1_6_2/javax.mail.jar)
        *   [MVNRepository](https://mvnrepository.com/artifact/com.sun.mail/javax.mail) - JavaMail API
    *   **Installation**
        *   In **v8.3+**, rename _`javax.mail.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\lib`_
        *   In **v8.2** and below, rename _`javax.mail.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\Tomcat\lib`_
        *   Restart Aware IM server
*   [**Apache ActiveMQ™**](http://activemq.apache.org/) - The most popular and powerful open source messaging and Integration Patterns server. Apache [ActiveMQ](https://en.wikipedia.org/wiki/Apache_ActiveMQ) is an open source message broker written in Java together with a full Java Message Service (JMS) client.
    
    > ActiveMQ replaced JBoss since Aware IM version 5.8. Aware IM installs ActiveMQ `5.8.0` (06/02/2013) as part of its core server library.
    
    > Latest version of ActiveMQ that works with Aware IM is **`5.12.1`**. Latest release is **`5.15.11`** (November 2019).
    
    *   **Reported issues in Aware IM** - Scalability, bugs, performance...
        
        *   [Highly demand -- updates - security concerns](https://awareim.com/forum/viewtopic.php?f=1&t=10539&p=48389)
        *   [How many Communication driven apps can we host on 1 serv](https://awareim.com/forum/viewtopic.php?f=1&p=51529)
    *   [**Issues**](https://github.com/RennurApps/AwareIM-resources/issues) - Refer to the Issues tab.
        
    *   [**Bugs since `5.12.1`**](https://issues.apache.org/jira/browse/AMQ-6456?jql=project%20%3D%20AMQ%20AND%20issuetype%20%3D%20Bug%20AND%20status%20in%20(Open%2C%20%22In%20Progress%22%2C%20Reopened%2C%20Resolved%2C%20Closed)%20AND%20priority%20in%20(Blocker%2C%20Critical)%20AND%20affectedVersion%20in%20(5.12.2%2C%205.12.3%2C%205.13.0%2C%205.13.1%2C%205.13.2%2C%205.13.3%2C%205.13.4%2C%205.13.5%2C%205.14.0%2C%205.14.1%2C%205.14.2%2C%205.14.3%2C%205.14.4%2C%205.14.5%2C%205.15.0%2C%205.15.1%2C%205.15.10%2C%205.15.11%2C%205.15.2%2C%205.15.3%2C%205.15.4%2C%205.15.5%2C%205.15.6%2C%205.15.7%2C%205.15.8%2C%205.15.9)%20ORDER%20BY%20affectedVersion%20ASC%2C%20priority%20ASC%2C%20updated%20DESC)
        
    *   **Releases**:
        
        *    [5.15.12 Release](http://activemq.apache.org/activemq-51512-release) - 9 Mar, 2020. **Inconsistent vector internals** Aware IM error.
            *   ERROR:
                *   `org.openadaptor.adaptor.jms.JMSListener - onMessage: JMSException: [javax.jms.JMSException: Failed to build body from bytes. Reason: java.io.StreamCorruptedException: Inconsistent vector internals [java.io.StreamCorruptedException: Inconsistent vector internals]]`
            *   Changelog
                *   This release enables ActiveMQ client TLS hostname validation by default which can cause a client connection failure for server certificates that do not match the server hostname. Please refer to SSL Transport Reference for configuration and [AMQ-7047](https://issues.apache.org/jira/browse/AMQ-7047) for more information.
                *   Java 8 Required - The minimum Java version has been upgraded to Java 8.
                *   This release affects applications using ObjectMessages.
            *   Aware IM 8.2 - Not Tested.
            *   Aware IM 8.1
                *   Configurator won't start
                *   Browser won't load the app
        *    [**5.12.1 Release**](http://activemq.apache.org/activemq-5121-release.html) - 👍 **Tested and working with Tomcat 6, 8 & 9**.
            *   Installation
                *   In **v8.3+**, extract, rename activemq-all-x.xx.x.jar to activemq-all-5.8.0.jar and replace the one in C:\\AwareIM\\lib
                *   In **v8.2 and below**, extract, rename activemq-all-x.xx.x.jar to activemq-all-5.8.0.jar and replace the one in C:\\AwareIM\\Tomcat\\lib
        *    [**5.8.0 Release**](http://activemq.apache.org/activemq-580-release.html) - Default version packaged with the server installation.
*   [**Java Service Wrapper** -](http://wrapper.tanukisoftware.com/doc/english/download.jsp) \- **32bit v3.5.42** 64-bit Windows versions of the Java Service Wrapper are not currently being made available in the Community Edition.
    
    *   [**Licensing Overview**](https://wrapper.tanukisoftware.com/doc/english/licenseOverview.html) - Choosing an Appropriate License.

#### [](#database-servers)Database Servers

*   #### [](#mysql)**MySQL**
    
    *   [**MySQL Community Server**](http://www.mysql.com/products/community/)
        *   Download
            
            *    [**MySQL Community Server 8.0.20**](http://dev.mysql.com/downloads/mysql/) - 27 Apr 2020. Upgrade from MySQL 5.7 to MySQL 8.0 is only supported using the in-place upgrade method.
                *   **Prerequisite**
                    *   [Visual Studio 2015, 2017 and 2019](https://support.microsoft.com/en-au/help/2977003/the-latest-supported-visual-c-downloads)
            
            *    [**MySQL Community Server 5.7.30**](https://dev.mysql.com/downloads/mysql/5.7.html) - 27 Apr 2020.
                *   **Prerequisite**
                    *   [Microsoft Visual C++ 2013](https://support.microsoft.com/en-us/help/3179560) MySQL 5.7 requires the Microsoft Visual C++ 2013 Redistributable Package to run on Windows platforms.
            *    [**MySQL Community Server 5.6.48**](https://dev.mysql.com/downloads/mysql/5.6.html) - 27 Apr 2020.
                *   **Prerequisite**
                    *   [Microsoft Visual C++ 2010](https://www.microsoft.com/en-au/download/details.aspx?id=26999) - Service Pack 1 MFC Security Update. MySQL 5.6 requires the Microsoft Visual C++ 2010 Redistributable Package to run on Windows platforms.
            *    [**MySQL Community Server 5.5.62**](https://dev.mysql.com/downloads/mysql/5.5.html) - 22 Oct 2018.
*   #### [](#apache-derby---home)**Apache Derby** - [Home](http://db.apache.org/derby/)
    
    *   **For Java 9 and higher** -
        *    [10.15.1.3](https://db.apache.org/derby/releases/release-10.15.1.3.cgi) - (March 5, 2019)
            *   Not supported by Aware IM `8.4` and below
    *   **For Java 8**
        *    [**Apache Derby 10.14.2.0**](https://db.apache.org/derby/releases/release-10.14.2.0.cgi) - (May 5, 2018)
            *   Installation: Copy and replace derby.jar in C:\\AwareIM\\Tomcat\\lib
        *   [Apache Derby 10.13.1.1](https://db.apache.org/derby/releases/release-10.13.1.1.cgi) - (October 25, 2016)
    *   **For Java 6 and higher**
        *    [Apache Derby 10.12.1.1](https://db.apache.org/derby/releases/release-10.12.1.1.cgi) - (October 11, 2015)
        *   [Apache Derby 10.11.1.1](http://db.apache.org/derby/releases/release-10.11.1.1.cgi) - (August 26, 2014)
    *   Downloads [http://db.apache.org/derby/derby\_downloads.html](http://db.apache.org/derby/derby_downloads.html)
*   #### [](#postgresql---postgresql-is-a-powerful-open-source-object-relational-database-system)**PostgreSQL** - [PostgreSQL](https://www.postgresql.org/) is a powerful, open source object-relational database system.
    
    *   [Download PostgreSQL](https://www.postgresql.org/download/) - Current version `12.2` 13 February 2020.
*   #### [](#maria-db)**Maria DB**
    
    *   [**MariaDB Server**](https://mariadb.org/) - Free and open-source software under the GNU General Public License.
        *   [**Download**](https://mariadb.org/download/)
            *   [**MariaDB version 10.4.12 Stable**](https://downloads.mariadb.org/mariadb/10.4.12/) - 28 January 2020.
*   #### [](#sql-server---microsoft-data-platforms)**SQL Server** - [Microsoft Data Platforms](https://www.microsoft.com/en-in/sql-server/)
    
    *   [SQL Server Downloads](https://www.microsoft.com/en-in/sql-server/sql-server-downloads)
*   #### [](#oracle---oracle-database)**Oracle** - [Oracle Database](https://www.oracle.com/database/)
    
    *   [Oracle Database Software Downloads](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html) - Oracle Database vesrios `19c` (`19.5`)

#### [](#database-connectors)Database Connectors

*   #### [](#mysql-connectors---grey_exclamationupdate-to-version-8x-highly-recommendedgrey_exclamation)[**MySQL Connectors**](https://www.mysql.com/products/connector/) - ❕**UPDATE TO VERSION 8.x HIGHLY RECOMMENDED**❕
    
    > From version 8.1 build 2461 onwards, Aware IM uses Connector/J JDBC driver version 5.1.46. JDBC driver communicates with MySQL servers.
    
    > Prior to Aware IM version 8.1 build 2461, a very old version of Connector/J JDBC driver (3.1.12 rel. 30/11/2005) is bundled with the Aware IM installation.
    
    *   [Connector/J Versions](https://dev.mysql.com/doc/connector-j/8.0/en/connector-j-versions.html) and what MySQL and Java JDK Versions they support.
        
    *   ✔️ [**Connector/J 8.0.x**](https://dev.mysql.com/downloads/connector/j/) - **Latest version `v8.0.20`**, 27 Apr 2020. It supports MySQL `5.5`, `5.6`, `5.7`, and `8.0`. It supports the `JDBC 4.2` specification. It is a MySQL driver for the `Java 8` platform. For `Java 7` or earlier, use `Connector/J 5.1` instead.
        
        *   **Installation**
            *   Application Server
                1.  Download `platform independent` version
                2.  Extract the files and rename `mysql-connector-java-8.x.xx-bin.jar` to `mysql-connector-java-5.1.46-bin.jar`
                3.  Copy and replace the existing file in
                    *   **v8.3+**, `C:\AwareIM\lib`
                    *   **v8.2 and below**, `C:\AwareIM\Tomcat\lib`
                4.  Restart AwareIM Server Control Panel
    *   ✔️ [**Connector/J 5.1.x**](https://dev.mysql.com/downloads/connector/j/5.1.html) - **Latest version `v5.1.48`**, 29 July 2019. Suitable for use with MySQL server versions `5.5`, `5.6`, and `5.7`. It supports the Java Database Connectivity (JDBC) 4.2 API. MySQL Connector/J is the official JDBC driver for MySQL.
        
        *   [**Download**](https://dev.mysql.com/downloads/connector/j/5.1.html) - Download the latest **Platform Independent** version.
        *   [Changes and Release Notes](https://dev.mysql.com/doc/relnotes/connector-j/en/index.html)
        *   [Aware IM Forum post](http://www.awareim.com/forum/viewtopic.php?t=5284)
        *   **Installation**
            *   Application Server
                1.  Download `platform independent` version
                2.  Extract the files and rename `mysql-connector-java-5.x.xx-bin.jar` to `mysql-connector-java-3.1.12-bin.jar`
                3.  Copy and replace the existing file in:
                    *   **v8.3+**, `C:\AwareIM\lib`
                    *   **v8.2 and below**, `C:\AwareIM\Tomcat\lib`
                4.  Restart AwareIM Server Control Panel
*   #### [](#postgresql-jdbc-connector---current-version-42212)[**PostgreSQL JDBC Connector**](https://jdbc.postgresql.org/download.html) - Current version `42.2.12`.
    
    *   Java 8 required.
*   #### [](#mariadb-connectors)[**MariaDB Connectors**](https://mariadb.com/kb/en/library/connectors/)
    
    *   [**MariaDB Connector/J**](https://downloads.mariadb.org/connector-java/+releases/) - Type 4 JDBC driver out-of-the-box support in Aware IM v8.3+.
        
        *    [MariaDB Connector/J 2.6.0 Stable](https://downloads.mariadb.org/connector-java/2.6.0/) - 28 January 2020.
            *   **Version untested with Aware IM**
        
        > Aware IM Version 8.3 uses MariaDB Connector/J driver version `2.3.0` (7 September 2018).
        

#### [](#web-application-framework---html5js-framework)**Web Application Framework** - HTML5/JS Framework

*   [**Kendo UI®**](http://www.telerik.com/kendo-ui) - **Aware IM v7.0+**. JavaScript, HTML5 UI widgets for responsive web and data visualization.
    *   [**Roadmap**](http://www.telerik.com/support/whats-new/kendo-ui/roadmap)
    *   [**Release History**](http://www.telerik.com/support/whats-new/kendo-ui/release-history)
        *   Latest Kendo UI Release [**Kendo UI R1 2020 SP2**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r1-2020-sp2) - April 6, 2020
        *   **Aware IM 8.1+** Kendo UI version [**Kendo UI R3 2017**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2017)
        *   Aware IM 7.0-8.0 Kendo UI version [Kendo UI Q1 2016](http://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-q1-2016) - January 12, 2016
    *   [**Demos**](http://demos.telerik.com/kendo-ui/) - Kendo UI Components
    *   70+ jQuery-based UI widgets in one powerful toolset.
    *   AngularJS integration, Bootstrap support, mobile controls, offline data solution.
*   **Ext JS v5.0.0** - for Aware IM v6.0 Only (final)
    *   [Guide](http://docs.sencha.com/extjs/5.0.0/index.html)
        *   [Ext JS 5 Examples](http://dev.sencha.com/ext/5.0.0/examples/index.html)
    *   [Whats's New](http://docs.sencha.com/extjs/5.0.0/whats_new/5.0/whats_new.html)
*   Ext JS v4.1.0 for Aware IM v5.9 Only (final)
    *   [Ext JS Docs](http://docs.sencha.com/extjs/4.1.0/)
    *   [Ext JS Examples](http://try.sencha.com/extjs/4.1.0/)

#### [](#mobile-web-framework)**Mobile Web Framework**

*   **Aware IM 7.x+** - Mobile apps with HTML5 and JavaScript.
    *   [**Kendo UI®**](http://www.telerik.com/kendo-ui)
*   Aware IM 5.x & 6.x
    *   [**Sencha Touch**](http://www.sencha.com/products/touch/) v2.3.1 (final). HTML5 Mobile app development.
        *   [Documentation](http://docs.sencha.com/touch/2.3.1/)

#### [](#front-end-framework)Front-end Framework

*   **Bootstrap** - For Aware IM version 5.x & 6.x only; Aware IM 7.0 has bootstrap integrated as part of Kendo UI.
    *   [Bootstrap v4](https://getbootstrap.com/) - Currently v**4.5.0** - Not tested with AwareIM 6.0 or below. Some v3 features dropped.
        *   [**Download**](https://getbootstrap.com/docs/4.4/getting-started/download/)
        *   [**BootstrapCDN**](https://getbootstrap.com/docs/4.4/getting-started/download/#bootstrapcdn) - Cached version of Bootstrap’s compiled CSS and JS.
    *   [**Bootstrap v3**](https://getbootstrap.com/docs/3.3/) - v3.3.7 (final).
        *   Integrating with Aware IM
            *   Manual configuration through Startup.html
            *   disable **`legend`** style with /\* \*/ brackets as it seems to be in conflict with the ExtJS style
                *   `/* legend { display: block; width: 100%; padding: 0; margin-bottom: 20px; font-size: 21px; line-height: inherit; color: #333; border: 0; border-bottom: 1px solid #e5e5e5; } */`
    *   [LayoutIt!](http://www.layoutit.com/build) - Drag & drop layout builder
    *   [Huge list of bootstrap resources](https://sendcheckit.com/the-big-badass-list-of-twitter-bootstrap-resources)
    *   [Bootstrap Tutorial](http://www.tutorialrepublic.com/twitter-bootstrap-tutorial/)
*   [Front-end Frameworks with comparison](http://bit.ly/RAfrontend) - Collection of best front-end frameworks
*   [Front End Development Bookmarks](http://bit.ly/FrontEndList) - A huge list of frontend development resources collected over time.

#### [](#aware-im-internal-features)Aware IM Internal Features

*   **Electronic Signature Capture** - For Aware IM 5.9+
    *   [**Signature Pad**](https://github.com/szimek/signature_pad) - Implement and store electronic signatures out-of-the-box with Aware IM. HTML5 canvas based and works in all modern desktop and mobile browsers.
    *   [**DEMO - Github**](http://szimek.github.io/signature_pad/)
    *   [**Signature Pad v3.0.0-beta.3**](https://www.jsdelivr.com/package/npm/signature_pad) - (c) 2018 Szymon Nowak. Tested ok in 8.1.
    *   [✔️ **Signature Pad v1.5.3**](https://www.jsdelivr.com/package/npm/signature_pad?version=1.5.3) - Tested and working in all versions 5.9+
    *   **Installation**:
        *   Replace ../AwareIM/signature/signature\_pad.js with the new version.
    *   **Options** - Edit **signature\_pad.js** found in **C:\\AwareIM\\Tomcat\\webapps\\AwareIM\\signature**
        *   `dotSize` - (float or function) Radius of a single dot.
        *   `minWidth` - (float) Minimum width of a line. Defaults to 0.5.
        *   `maxWidth` - (float) Maximum width of a line. Defaults to 2.5.
        *   **`backgroundColor`** - (string) Color used to clear the background. Can be any color format accepted by context.fillStyle. Defaults to `rgba(0,0,0,0)` (transparent black).
            *   I prefer a `**white background "rgb(255,255,255)"**` for the signatures since there are issues with transparent images in the Report Designer and PDF document export.
        *   `penColor` - (string) Color used to draw the lines. Can be any color format accepted by context.fillStyle. Defaults to "black".
        *   `velocityFilterWeight` - (float) Weight used to modify new velocity based on the previous velocity. Defaults to 0.7.
        *   `onBegin` - (function) Callback when stroke begin.
        *   `onEnd` - (function) Callback when stroke end.
    *   [Video Tutorial (approx. 3min)](http://www.awareim.com/tutorials/59/New%20In%205,9.html) - from 00:38min
*   **Social Logins**

#### [](#hybrid-native-apps)Hybrid Native Apps

*   **Phonegap** support

#### [](#integrations-custom-components-connectors-and-plugins)Integrations, custom components, connectors and plugins

Any application offering an API for developers makes it possible to integrate with Aware IM by writing a plugin.

*   [**wkhtmltopdf**](https://github.com/wkhtmltopdf/wkhtmltopdf) - wkhtmltopdf is a command line tools to render HTML into PDF using the QT Webkit rendering engine. These run entirely "headless" and do not require a display or display service.
    
    *   **Requires** [**Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019**](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) - Download and install first.
    *   **Download wkhtmltopdf**:
        *   [**Download wkhtmltopdf** Windows (MSVC)](https://wkhtmltopdf.org/downloads.html) - **v0.12.6** released on June 11, 2020 for Windows, Linux and OS X.
            *    **`v0.12.6`** Tested and working in Aware IM **6.0+**. Released June 11, 2020.
            *    **`v0.12.5`** Tested and working in Aware IM **6.0+**. Released June 11, 2018.
            *    `v0.12.4` Tested and working in Aware IM **6.0+**. Released November 22, 2016
    *   **Install wkhtmltopdf**
        *   Windows
            *   Extract \*.exe file to a folder (you can use [7-Zip](http://www.7-zip.org/)), copy+paste wkhtmltopdf folder to c:/AwareIM
    *   **Aware IM Process Rules**
        *   **Step 1** - Export Aware IM HTML Document to a HTML file
            *   `EXPORT DOCUMENT 'Your HTML Document' TO FILE 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html'`
        *   **Step 2** - Convert exported HTML file to PDF
            *   `EXECUTE PROGRAM 'C:\AwareIM\wkhtmltopdf\bin\wkhtmltopdf.exe file:///C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.pdf'`
        *   **Step 3** - Import PDF document to your myBO.DocumentPDF attribute
            *   `IMPORT DOCUMENT myBO.DocumentPDF FROM 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.pdf'`
        *   **Optional** - Delete exported HTML file
            *   `DELETE FILE 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html'`
*   **Business Intelligence, Report Writer/Server**
    
    *   **Power BI Interactive Data Visualization** - [Microsoft Power BI](https://powerbi.microsoft.com/en-us/)
    *   **TIBCO Jaspersoft**
        *   [**JasperReports® Server**](https://community.jaspersoft.com/project/jasperreports-server) - Self-service Reporting and Analysis Server
            *   [Documentation](https://community.jaspersoft.com/documentation?version=15786)
            *   [Installation Guide](https://community.jaspersoft.com/documentation/tibco-jasperreports-server-installation-guide/v61/introduction)
                *   Bundled with and installed own Tomcat server and PostgreSQL database
            *   **Connect to MySQL database**
                *   [Login to Jasper Reports Server](http://localhost:8081/jasperserver/login.html) - [http://localhost:8081/jasperserver/login.html](http://localhost:8081/jasperserver/login.html) Login UserID: `jasperadmin` Password: `jasperadmin` (change password after login)
                *   Data Sources > Add Resource > Data Source > JDBC Data Source
                    *   MySQL `com.mysql.jdbs.Driver`
                    *   Click on `Select Driver` > Choose File > `C:\Program Files (x86)\MySQL\MySQL Connector J\mysql-connector-java-x.x.xx-bin.jar`
                    *   `localhost`
                    *   port is usually `3306`
                    *   Databse name: `BASDB` (change if different)
                    *   URL: `jdbc:mysql://localhost:3306/BASDB`
                    *   database username (default: root) & password
        *   [**Jaspersoft® Studio**](http://community.jaspersoft.com/project/jaspersoft-studio) - The Eclipse-based Report Development Tool for JasperReports and JasperReports Server
            *   [User Guide](http://community.jaspersoft.com/documentation/tibco-jaspersoft-studio-user-guide/v610/getting-started-jaspersoft-studio)
        *   **Forum posts**
            *   [AWARE'S REPORTING - JASPER REPORTS UPGRADE FOR NEXT RELEASE?](http://www.awareim.com/forum/viewtopic.php?f=1&t=7744) - JasperRepoerts Server
    *   [**Metabase BI**](https://www.metabase.com/) - Open source.

<!-- 
# Donate
https://paypal.me/RennurApps?locale.x=en_AU
-->