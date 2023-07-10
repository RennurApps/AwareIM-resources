# Aware IM Server v8.8 Stack

## Application Server, Database Servers, Components, Frameworks, Dependencies, Microservices and other resources.

---

> Aware IM is a rapid low-code application development tool that lets you create powerful aesthetically appealing web applications quickly.

[**Changelog**](https://www.awareim.com/dokuwiki/doku.php/changelog/8.8) <!--(http://www.awareim.com/changelog/?C=M;O=D) -->

<!-- #### Software -->
<!--
Aware IM is based on the plethora of Java technologies such as J2EE application server, JDBC, JMS, JSP/servlets technology, web services etc. These are robust technologies that have been proven in the industry.
-->
<!-- Links to tutorials, documentation, events, apps have been moved [**here**](https://github.com/RennurApps/AwareIM-Help) -->

✔️ [**v8.8 build 3137**](https://www.awareim.com/dokuwiki/doku.php/changelog/8.8/3137) - 23 May, 2023. <br>

- New Features and improvements in version 8.8
  - 3132 - Support for max file size, total max file size and allowed extensions for multi-file upload
  - 3127 - [“Resolve Shortcuts”](https://www.awareim.com/dokuwiki/doku.php/docs/2500_config_apps/1100_add_edit_queries/0100_query_props#resolve_shortcuts) property when defining a query (performance booster)
  - 3126 - Support for non-iterated propery in reports
  - 3126 - [GET_ATTR_VALUE](https://www.awareim.com/dokuwiki/doku.php/a_f/f/af/get_attr_value) function
  - 3123 - [**List of `8.8` release improvements**](https://www.awareim.com/dokuwiki/doku.php/changelog/8.8/3123)

### Application Server

#### Apache Tomcat

> Disclaimer: Use this information and instructions at your own risk. There is no support provided for any of the updates performed outside of default Aware IM installation.

> Caution: Installing Aware IM update (Setup.exe), overwrites and resets Tomcat & JDK folders back to default. In fact, all files are replaced during update. Always keep all new and amended files incl. images separately and copy+paste them back once the install is complete.

> 📉 **Tomcat 9.0.44** 32bit is the default version packaged in the **Aware IM 8.6 and above** server installation.

> Tomcat 8.5.58 32bit is the default version packaged in the **Aware IM 8.5** server installation.

> Tomcat 8.5.24 32bit is the default version packaged in the **Aware IM 8.4 and below** server installation.

- :warning: [**Tomcat 10.1.10**](http://tomcat.apache.org/) - Tomcat 10 is designed to run on **`Java SE 8`** or later.

  > Users of Tomcat 10 onwards should be aware that, as a result of the move from Java EE to Jakarta EE as part of the transfer of Java EE to the Eclipse Foundation, the primary package for all implemented APIs has changed from `javax.*` to `jakarta.*`. This will almost certainly require code changes to enable applications to migrate from Tomcat 9 and earlier to Tomcat 10 and later.

  - :warning: **Few java exceptions `Aware IM 8.5`**
  - :warning: **Not compatible with `Aware IM 6.0 and below`**
  - [**Download Tomcat v10**](https://tomcat.apache.org/download-10.cgi)<br>

- ✔️ [**Tomcat 9.0.76** - For Aware IM v8.x](http://tomcat.apache.org/) - 5 June, 2023. Tomcat 9 is designed to run on **`Java SE 8`** or later.

  - [**Download Tomcat v9**](https://tomcat.apache.org/download-90.cgi) - 64bit recommended. Manual Install.

    - ✔️ Tested and working with `Aware IM` `6.x`, `7.x` & `8.x`
    - [**Security**](https://tomcat.apache.org/security-9.html)
        <details>
        <summary>Important fixes</summary>

      - `9.0.75` Important: Information disclosure [CVE-2023-34981](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-34981) - Affects: 9.0.74
      - `9.0.72` Important: Apache Tomcat information disclosure [CVE-2023-28708](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28708) - Affects: 9.0.0-M1 to 9.0.71
      - `9.0.71` Important: Apache Tomcat denial of service `CVE-2023-24998` - Affects: 9.0.0-M1 to 9.0.70
      - `9.0.54` Important: Denial of Service `CVE-2021-42340` - Affects: 9.0.40 to 9.0.53
      - `9.0.48` Request Smuggling `CVE-2021-33037` - Affects: 9.0.0.M1 to 9.0.46
      - `9.0.45` Denial of Service `CVE-2021-30639` - Affects: 9.0.44
      - `9.0.43` Request mix-up with h2c `CVE-2021-25122` - Affects: 9.0.0.M1 to 9.0.41
      - `9.0.40` Information disclosure `CVE-2021-24122` - Affects: 9.0.0.M1 to 9.0.39 - 14 January 2021
      - `9.0.37` WebSocket DoS `CVE-2020-13935` - Affects: 9.0.0.M1 to 9.0.36 - 14 July 2020
      - `9.0.36` HTTP/2 DoS `CVE-2020-11996` - Affects: 9.0.0.M1 to 9.0.35 - 25 June 2020
      - `9.0.35` Remote Code Execution via session persistence `CVE-2020-9484` - Affects: 9.0.0.M1 to 9.0.34 - 20 May 2020
      - `9.0.31` AJP Request Injection and potential Remote Code Execution `CVE-2020-1938` - Affects: 9.0.0.M1 to 9.0.30 - 24 February 2020
      - `9.0.20` Denial of Service `CVE-2019-10072` - Affects: 9.0.0.M1 to 9.0.19 - 20 June 2019
      - `9.0.19` Remote Code Execution on Windows `CVE-2019-0232` - Affects: 9.0.0.M1 to 9.0.17 - 10 April 2019
      - `9.0.16` Denial of Service `CVE-2019-0199` - Affects: 9.0.0.M1 to 9.0.14 - 25 March 2019
      - `9.0.10` Information Disclosure `CVE-2018-8037` - 22 July 2018
      - `9.0.8` A bug in the UTF-8 decoder can lead to DoS `CVE-2018-1336` - 22 July 2018
      - `9.0.5` Security constraint annotations applied too late `CVE-2018-1305` - 23 February 2018
      - `9.0.5` Security constraints mapped to context root are ignored `CVE-2018-1304` - 23 February 2018
      - `9.0.1` Remote Code Execution `CVE-2017-12617` - 20 September 2017
      </details>

    - [Tomcat 9 Documentation](https://tomcat.apache.org/tomcat-9.0-doc/index.html).
    - [Tomcat 9 Changelog](https://tomcat.apache.org/tomcat-9.0-doc/changelog.html).
    - **Installation**
        <details>
        <summary>Microsoft Windows Based Systems</summary>

      - **IMPORTANT**: Ensure any prior modification of existing _`web.xml`_ and _`server.xml`_ configurations are not overwritten with the new version. There are configuration changes in the latest version of Tomcat relating to those two files.
      - **Installation Steps**
        - Stop the Aware IM server before updating Tomcat. Do **not** delete your current _C:\AwareIM\Tomcat_ folder.
        - 1. **Extract** the archive and open the folder.
        - 2. Open the extracted **Tomcat** folder.
        - 3. Select all files and folders and press `Crl+c` to copy
        - 4. Open you AwareIM installation Tomcat folder **`C:\AwareIM\Tomcat`**
        - 5. Press `Ctrl+v` to paste and replace all files and folders.
        - 6. Java JDK `tools.jar`:
             - **In v8.6-8.8**, `tools.jar` is not required.
             - **In v8.3-8.5**, if you have updated Java JDK, copy the latest version of `tools.jar` to the _C:\Awareim\lib_ folder to replace the old one.
             - **In v8.2 and below**, if you have updated Java JDK, copy the latest version of `tools.jar` to the _C:\Awareim\Tomcat\lib_ folder to replace the old one.
        - 7. Rename or delete **ROOT** folder - _This is optional_. You can use this folder to store your own favicon.ico, error pages and other HTML/CSS/JS home page files.
          </details>

#### Java JDK

- [**OpenJDK Java SE Releases**](https://jdk.java.net) - Oracle provides the latest **OpenJDK** releases under the open source.

  - ✔️ [**Oracle OpenJDK `20`**](https://jdk.java.net/20/)
  - :+1: [Oracle OpenJDK `19`](https://jdk.java.net/19/)
  - 📉 [Oracle OpenJDK `17`](https://jdk.java.net/17/)
      <details>
      <summary>8.5 Server Error</summary>

    - **Aware IM `8.5 2836`** server error: > Server unknown error javax/activation/DataSource exiting... > java.lang.NoClassDefFoundError: javax/activation/DataSource > at com.bas.basserver.channels.ChannelManager.startupEntity(Unknown Source) > at com.bas.basserver.domainmanager.DomainManager.A(Unknown Source) > at com.bas.basserver.domainmanager.DomainManager.<init>(Unknown Source) > at com.bas.basserver.bsmanager.E.A(Unknown Source) > at com.bas.newcp.ServerStarterECP.K(Unknown Source) > at com.bas.newcp.ServerStarterECP.main(Unknown Source) > Caused by: java.lang.ClassNotFoundException: javax.activation.DataSource > at java.base/jdk.internal.loader.BuiltinClassLoader.loadClass(BuiltinClassLoader.java:636) > at java.base/jdk.internal.loader.ClassLoaders$AppClassLoader.loadClass(ClassLoaders.java:182) > at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:519) > ... 6 more
    </details>

  - [Archived Versions](https://jdk.java.net/archive/)

- [**Commercial Java SE Development Kit (JDK)**](https://www.oracle.com/technetwork/java/javase/overview/index.html) - [Important Oracle JDK License Update starting April 16, 2019](https://www.oracle.com/technetwork/java/javase/overview/oracle-jdk-faqs.html)
  - ✔️ [**Version `20.0.1`**](https://www.oracle.com/java/technologies/downloads/) - **Works with Aware IM version `8.8`**.
  - :+1: [Version `17.0.7`](https://www.oracle.com/java/technologies/downloads/) - **Works with Aware IM version `8.6 and above`**.
  - 📉 [**Version `12.0.2` Final**](https://www.oracle.com/java/technologies/javase/jdk12-archive-downloads.html) - **Bundled with Aware IM `8.6 and above`** - Archived.
  - [Version 8, Update 371](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html) - **Compatible with Aware IM versions `6.0` - `8.5`**.
  - Versions bundled with Aware IM:
    - Aware IM `v8.6 and above` - [JDK `12.0.2` Commercial](https://docs.oracle.com/en/java/javase/12/)
    - Aware IM `v8.0 - 8.5` - JDK 8 Update 91 `1.8.0_91-b15`
  - [**All previous JDK versions archive**](https://www.oracle.com/java/technologies/downloads/archive/)
    - [Manual Downloads](https://java.com/en/download/manual.jsp)

####

- ✔️ [**Jakarta Mail**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/) - **`1.6.7`** - April 8, 2021 Final Release. (formerly JavaMail)
  - [**Download jakarta.mail-1.6.7.jar**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/1.6.7)
    - **Installation**
      - In Aware IM **v8.3 and above**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\lib`_
      - In Aware IM **v8.2 and below**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\Tomcat\lib`_
      - Restart Aware IM server
  - 📉 [JavaMail 1.6.2](https://javaee.github.io/javamail/) - August 30, 2018 Final Release. (superseded by JakartaMail)

####

- [**Apache ActiveMQ™**](http://activemq.apache.org/) - The most popular and powerful open source messaging and Integration Patterns server. Apache [ActiveMQ](https://en.wikipedia.org/wiki/Apache_ActiveMQ) is an open source message broker written in Java together with a full Java Message Service (JMS) client.

  > ActiveMQ replaced JBoss since Aware IM version 5.8. Aware IM installs ActiveMQ `5.8.0` (06/02/2013) as part of its core server library.

  > Latest version of ActiveMQ cthat works with Aware IM is **`5.12.1`** (13 Oct 2015). <br>

  - **Reported issues in Aware IM** - Scalability, bugs, performance...
    - [Highly demand -- updates - security concerns](https://awareim.com/forum/viewtopic.php?f=1&t=10539&p=48389)
    - [How many Communication driven apps can we host on 1 serv](https://awareim.com/forum/viewtopic.php?f=1&p=51529)
  - [**Issues**](https://github.com/RennurApps/AwareIM-resources/issues) - Refer to the Issues tab.
  - [**Bugs since `5.12.1`**](<https://issues.apache.org/jira/browse/AMQ-7229?jql=project%20%3D%20AMQ%20AND%20status%20in%20(Open%2C%20%22In%20Progress%22%2C%20Reopened)%20AND%20resolution%20%3D%20Unresolved%20AND%20affectedVersion%20in%20(5.12.2%2C%205.12.3%2C%205.13.0%2C%205.13.1%2C%205.13.2%2C%205.13.3%2C%205.13.4%2C%205.13.5%2C%205.14.0%2C%205.14.1%2C%205.14.2%2C%205.14.3%2C%205.14.4%2C%205.14.5%2C%205.15.0%2C%205.15.1%2C%205.15.10%2C%205.15.11%2C%205.15.12%2C%205.15.13%2C%205.15.14%2C%205.15.15%2C%205.15.2%2C%205.15.3%2C%205.15.4%2C%205.15.5%2C%205.15.6%2C%205.15.7%2C%205.15.8%2C%205.15.9%2C%205.16.0%2C%205.16.1%2C%205.16.2%2C%205.16.3%2C%205.16.4%2C%205.16.5%2C%205.17.0%2C%205.17.1%2C%205.17.2)%20ORDER%20BY%20priority%20DESC%2C%20updated%20DESC>)
  - **Releases**:
    - ⚠️ [5.18.2 Release](https://activemq.apache.org/activemq-5018002-release) - 2 July, 2023. Java compatibility: 11+. **Not tested with Aware IM**.
    - ⚠️ [5.17.5 Release](https://activemq.apache.org/activemq-5017005-release) - 2 July, 2023. Java compatibility: 11+. **Not tested with Aware IM**.
    - ⚠️ [5.16.4 Release](https://activemq.apache.org/activemq-5016004-release) - 15 February, 2022. **Inconsistent vector internals** Aware IM error.
      - ERROR:
        - `org.openadaptor.adaptor.jms.JMSListener - onMessage: JMSException: [javax.jms.JMSException: Failed to build body from bytes. Reason: java.io.StreamCorruptedException: Inconsistent vector internals [java.io.StreamCorruptedException: Inconsistent vector internals]]`
      - Changelog
        - This release enables ActiveMQ client TLS hostname validation by default which can cause a client connection failure for server certificates that do not match the server hostname. Please refer to SSL Transport Reference for configuration and [AMQ-7047](https://issues.apache.org/jira/browse/AMQ-7047) for more information.
        - Java 8 Required - The minimum Java version has been upgraded to Java 8.
        - This release affects applications using ObjectMessages.
      - Aware IM 8.2 - Not Tested.
      - Aware IM 8.1
        - Configurator won't start
        - Browser won't load the app
    - ✔️ [**5.12.1 Release**](http://activemq.apache.org/activemq-5121-release.html)
      - Installation
        - In **v8.3 and above**, extract, rename `activemq-all-x.xx.x.jar` to `activemq-all-5.8.0.jar` and replace the one in `C:\AwareIM\lib`
        - In v8.2 and below, extract, rename `activemq-all-x.xx.x.jar` to `activemq-all-5.8.0.jar` and replace the one in `C:\AwareIM\Tomcat\lib`
    - 📉 [**5.8.0 Release**](http://activemq.apache.org/activemq-580-release.html) - Default version packaged with the server installation.

- [**Java Service Wrapper** -](http://wrapper.tanukisoftware.com/doc/english/download.jsp) \- **32bit v3.5.54** 64-bit Windows versions of the Java Service Wrapper are not currently being made available in the Community Edition.

  - [**Licensing Overview**](https://wrapper.tanukisoftware.com/doc/english/licenseOverview.html) - Choosing an Appropriate License.

### [](#database-servers)Database Servers

- #### [](#mysql)**MySQL**

  - [**MySQL Community Server**](http://www.mysql.com/products/community/)
    - Download
      - ✔️ [**MySQL Community Server 8.0.33**](http://dev.mysql.com/downloads/mysql/)
        - [Visual Studio 2015, 2017, 2019, and 2022](https://support.microsoft.com/en-au/help/2977003/the-latest-supported-visual-c-downloads) - Visual C++ Redistributable.
      - 👍 [**MySQL Community Server 5.7.42**](https://dev.mysql.com/downloads/mysql/5.7.html)
        - [Microsoft Visual C++ 2013](https://support.microsoft.com/en-us/help/3179560) MySQL 5.7 requires the Microsoft Visual C++ 2013 Redistributable Package to run on Windows platforms.
      - 📉 [**MySQL Community Server 5.6.51 (Final)**](https://downloads.mysql.com/archives/community/).
        - [Microsoft Visual C++ 2010](https://www.microsoft.com/en-au/download/details.aspx?id=26999) - Service Pack 1 MFC Security Update. MySQL 5.6 requires the Microsoft Visual C++ 2010 Redistributable Package to run on Windows platforms.

- #### [](#apache-derby---home)**Apache Derby** - [Home](http://db.apache.org/derby/)
<!--
    *   **For Java 9 and higher** -
        *    [10.15.1.3](https://db.apache.org/derby/releases/release-10.15.1.3.cgi) - (March 5, 2019)
            *   Not supported by Aware IM `8.4` and below
    *   **For Java 8**
        *    [**Apache Derby 10.14.2.0**](https://db.apache.org/derby/releases/release-10.14.2.0.cgi) - (May 5, 2018)
            *   Installation: Copy and replace derby.jar in C:\AwareIM\Tomcat\lib
        *   [Apache Derby 10.13.1.1](https://db.apache.org/derby/releases/release-10.13.1.1.cgi) - (October 25, 2016)
    *   **For Java 6 and higher**
        *    [Apache Derby 10.12.1.1](https://db.apache.org/derby/releases/release-10.12.1.1.cgi) - (October 11, 2015)
        *   [Apache Derby 10.11.1.1](http://db.apache.org/derby/releases/release-10.11.1.1.cgi) - (August 26, 2014)
    *   Downloads [http://db.apache.org/derby/derby_downloads.html](http://db.apache.org/derby/derby_downloads.html)
-->
- #### [](#postgresql---postgresql-is-a-powerful-open-source-object-relational-database-system)**PostgreSQL** - [PostgreSQL](https://www.postgresql.org/) is a powerful, open source object-relational database system.

  - Download PostgreSQL
    - [Windows installers](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) - Version `15.3`

- #### [](#maria-db)**Maria DB**

  - [**MariaDB Server**](https://mariadb.org/) - Free and open-source software under the GNU General Public License.
    - [**Download**](https://mariadb.org/download/) - Version `11.0.2`.

- #### [](#sql-server---microsoft-data-platforms)**SQL Server** - [Microsoft Data Platforms](https://www.microsoft.com/en-in/sql-server/)

  - [SQL Server Downloads](https://www.microsoft.com/en-in/sql-server/sql-server-downloads)

- #### [](#oracle---oracle-database)**Oracle** - [Oracle Database Enterprise Edition](https://www.oracle.com/database/)

  - [Oracle Database Software Downloads](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html) - Oracle Database version `21c` (`21.3`)

#### [](#database-connectors)Database Connectors

- #### [](#mysql-connectors---grey_exclamationupdate-to-version-8x-highly-recommendedgrey_exclamation)[**MySQL Connectors**](https://www.mysql.com/products/connector/) - ❕**UPDATE TO VERSION 8.x HIGHLY RECOMMENDED**❕

  - ✔️ [**Connector/J 8.0.x**](https://dev.mysql.com/downloads/connector/j/) - **Latest version `v8.0.33`**. It supports MySQL `5.5`, `5.6`, `5.7`, and `8.0`. It supports the `JDBC 4.2` specification. It is a MySQL driver for the `Java 8` platform. For `Java 7` or earlier, use `Connector/J 5.1` instead.
    - [**Download Platform Independent Version**](https://dev.mysql.com/downloads/connector/j/)
    - **Installation**
      - Application Server
        1.  Extract the files and rename `mysql-connector-java-8.x.xx-bin.jar` to `mysql-connector-j-8.0.31.jar`
        2.  Copy and replace the existing file in
            - **v8.8**, `C:\AwareIM\lib`
        3.  Restart AwareIM Server

- #### [**PostgreSQL JDBC Connector**](https://jdbc.postgresql.org/download/) - Current version `42.6.0`. Java 8 required.
- #### [**MariaDB Connectors**](https://mariadb.com/kb/en/library/connectors/)
  - [**MariaDB Connector/J**](https://mariadb.com/kb/en/mariadb-connector-j/) - Type 4 JDBC driver out-of-the-box support in Aware IM `v8.3`+. - ✔️ **MariaDB Connector/J `2.3.0`** - :warning: [MariaDB Connector/J `3.1.4`](https://mariadb.com/kb/en/mariadb-connector-j-306-release-notes/) - 29 Jun 2022.
  <!--      - **Server error starting Aware IM `8.5`**
        - `Loading class 'com.mysql.jdbc.Driver'. This is deprecated. The new driver class is com.mysql.cj.jdbc.Driver'. The driver is automatically registered via the SPI and manual loading of the driver class is generally unnecessary. Message returned from the database Access denied for user 'root'@'localhost' (using password: YES) Server startup error. Access to database is denied.` -->

### [](#web-application-framework---html5js-framework)**Web Application Framework** - HTML5/JS Framework

- [**Kendo UI®**](https://www.telerik.com/kendo-ui) - **Aware IM `v7.0`+**. JavaScript, HTML5 UI widgets for responsive web and data visualization.
  - [**Roadmap**](https://www.telerik.com/support/whats-new/kendo-ui/roadmap)
  - [**Release History - jQuery**](https://www.telerik.com/support/whats-new/kendo-ui/release-history)
    - Latest Kendo UI Release [**Kendo UI R2 2023**](<https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r2-2023-(version-2023-2-606)>) - June 7, 2023
    - 📉 **Aware IM `8.6 - 8.8`** Kendo UI version [**Kendo UI R3 2020 SP1**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2020-sp1) - **October 21, 2020**
    - 📉 Aware IM `8.1 - 8.5` Kendo UI version [Kendo UI R3 2017](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2017) - September 13, 2017
    - 📉 Aware IM `7.0 - 8.0` Kendo UI version [Kendo UI Q1 2016](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-q1-2016) - January 12, 2016
  - [**jQuery Demos & Examples**](https://demos.telerik.com/kendo-ui/) - Kendo UI jQuery Components

#### [](#front-end-toolkit)Front-end open source toolkit

- **Bootstrap** - For Aware IM version 5.x & 6.x only; `Aware IM 7.0 and above` has bootstrap integrated as part of Kendo UI app framework.

  - [Bootstrap v5](https://getbootstrap.com/) - Currently **`v5.3.0`** - Not tested with AwareIM.
  - [Bootstrap v4.6](https://getbootstrap.com/docs/4.6/getting-started/introduction/) - `4.6.2` - Not tested with AwareIM.
    - [Download](https://getbootstrap.com/docs/4.6/getting-started/download/)
    - [jsDelivr](https://getbootstrap.com/docs/4.6/getting-started/download/#jsdelivr) - Skip the download with jsDelivr to deliver cached version of Bootstrap’s compiled CSS and JS to your project.
  - 📉 [Bootstrap v4.5](https://getbootstrap.com/docs/4.5/getting-started/introduction/) - `4.5.3` - Not tested with AwareIM.
    - [Download](https://getbootstrap.com/docs/4.5/getting-started/download/)
    - [jsDelivr](https://getbootstrap.com/docs/4.5/getting-started/download/#jsdelivr) - Cached version of Bootstrap’s compiled CSS and JS.
  - ✔️ [**Bootstrap v3**](https://getbootstrap.com/docs/3.4/) - **`3.4.1` (final)**. Bootstrap 3.3.4 bundled with Aware IM v`8.8`.
    - [Download](https://getbootstrap.com/docs/3.4/getting-started/#download)
    - [BootstrapCDN](https://getbootstrap.com/docs/3.4/getting-started/#download-cdn)
    - **Plug into Aware IM**
      - Manual configuration through **Startup.html**
      - disable **`legend`** style with /\* \*/ brackets as it seems to be in conflict with the ExtJS style
        - `/* legend { display: block; width: 100%; padding: 0; margin-bottom: 20px; font-size: 21px; line-height: inherit; color: #333; border: 0; border-bottom: 1px solid #e5e5e5; } */`
  - [All Bootstrap Versions](https://getbootstrap.com/docs/versions/)
  - [Huge list of bootstrap resources](https://sendcheckit.com/the-big-badass-list-of-twitter-bootstrap-resources)

- **Font Awesome 5**

  - Aware IM `8.8` bundles [Font Awesome version 5.6.3 Free For Web](https://fontawesome.com/v5/download).

- [Front-end Frameworks with comparison](http://bit.ly/RAfrontend) - Collection of best front-end frameworks
- [Front End Development Bookmarks](http://bit.ly/FrontEndList) - A huge list of frontend development resources collected over time.

### [](#aware-im-internal-features)Out-of-the-box Features

- **Integration with Stripe Multi-Payment** - Stripe is a very well-known payment platform and it supports multi-party payments. <!-- [Video](https://youtu.be/4m9YNPrpsvk%22) -->

- **Electronic Signature Capture** - For Aware IM `5.9 - 8.x`
  - [**Signature Pad**](https://github.com/szimek/signature_pad) - Implement and store electronic signatures out-of-the-box with Aware IM. HTML5 canvas based and works in all modern desktop and mobile browsers.
  - [**DEMO - Github**](http://szimek.github.io/signature_pad/)
  - [✔️ **Signature Pad v1.5.3**](https://www.jsdelivr.com/package/npm/signature_pad?version=1.5.3) - Tested and working in all versions `5.9 - 8.x`
  - **Installation**:
    - Replace ../AwareIM/signature/signature/\_pad.js with the new version.
  - **Options** - Edit **signature_pad.js** found in **C:\AwareIM\Tomcat\webapps\AwareIM\signature**
    - `dotSize` - (float or function) Radius of a single dot.
    - `minWidth` - (float) Minimum width of a line. Defaults to 0.5.
    - `maxWidth` - (float) Maximum width of a line. Defaults to 2.5.
    - **`backgroundColor`** - (string) Color used to clear the background. Can be any color format accepted by context.fillStyle. Defaults to `rgba(0,0,0,0)` (transparent black).
      - I prefer a `**white background "rgb(255,255,255)"**` for the signatures since there are issues with transparent images in the Report Designer and PDF document export.
    - `penColor` - (string) Color used to draw the lines. Can be any color format accepted by context.fillStyle. Defaults to "black".
    - `velocityFilterWeight` - (float) Weight used to modify new velocity based on the previous velocity. Defaults to 0.7.
    - `onBegin` - (function) Callback when stroke begin.
    - `onEnd` - (function) Callback when stroke end.
  - [Video Tutorial (approx. 3min)](http://www.awareim.com/tutorials/59/New%20In%205,9.html) - from 00:38min

### [](#integrations-custom-components-connectors-and-plugins)Integrations, custom components, connectors and plugins

Any application offering an API for developers makes it possible to integrate with Aware IM by writing a plugin.

- ✔️ [**wkhtmltopdf**](https://github.com/wkhtmltopdf/wkhtmltopdf) - wkhtmltopdf is a command line tool to render HTML into PDF using the QT Webkit rendering engine. These run entirely "headless" and do not require a display or display service.

  - **Requires** [**Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017, 2019, and 2022**](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) - Download and install first.
  - **Download wkhtmltopdf**:
    - [**Download wkhtmltopdf** Windows (MSVC)](https://wkhtmltopdf.org/downloads.html) - **v`0.12.6`** released on June 11, 2020 for Windows, Linux and OS X.
      - **`v0.12.6`** Tested and working in Aware IM **6.0+**. Released June 11, 2020.
      - `v0.12.5` Tested and working in Aware IM **6.0+**. Released June 11, 2018.
      - `v0.12.4` Tested and working in Aware IM **6.0+**. Released November 22, 2016
  - **Install wkhtmltopdf**
    - Windows OS
      - Extract `*.exe` file to a folder (you can use [7-Zip](http://www.7-zip.org/)), copy+paste wkhtmltopdf folder to c:/AwareIM
  - **Aware IM Process Rules**
    - **Step 1** - Export Aware IM HTML Document to a HTML file
      - `EXPORT DOCUMENT 'Your HTML Document' TO FILE 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html'`
    - **Step 2** - Convert exported HTML file to PDF
      - `EXECUTE PROGRAM 'C:\AwareIM\wkhtmltopdf\bin\wkhtmltopdf.exe file:///C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.pdf'`
    - **Step 3** - Import PDF document to your myBO.DocumentPDF attribute
      - `IMPORT DOCUMENT myBO.DocumentPDF FROM 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.pdf'`
    - **Optional** - Delete exported HTML file
      - `DELETE FILE 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html'`

- [**Pandoc - a universal document converter**](https://pandoc.org/) - If you need to convert files from one markup format into another, pandoc is your swiss-army knife.

- [**WeasyPrint**](https://weasyprint.org/) Smart solution helping web developers to create PDF documents. It’s free and open source software that can be easily plugged to your applications and websites and turns simple HTML pages into gorgeous Invoices, Reports, Posters, Letters and Tickets.

- **Business Intelligence, Report Writer/Server**

  - **Power BI Interactive Data Visualization** - [Microsoft Power BI](https://powerbi.microsoft.com/en-us/)
  - **TIBCO Jaspersoft**
    - [**JasperReports® Server**](https://community.jaspersoft.com/project/jasperreports-server) - Self-service Reporting and Analysis Server
      - [Download JasperReports](https://www.jaspersoft.com/download)
      - [Documentation](https://community.jaspersoft.com/documentation?version=15786)
      - [Installation Guide](https://community.jaspersoft.com/documentation/tibco-jasperreports-server-installation-guide/v61/introduction)
        - Bundled with and installed own Tomcat server and PostgreSQL database
      - **Connect to MySQL database**
        - [Login to Jasper Reports Server](http://localhost:8081/jasperserver/login.html) - [http://localhost:8081/jasperserver/login.html](http://localhost:8081/jasperserver/login.html) Login UserID: `jasperadmin` Password: `jasperadmin` (change password after login)
        - Data Sources > Add Resource > Data Source > JDBC Data Source
          - MySQL `com.mysql.jdbs.Driver`
          - Click on `Select Driver` > Choose File > `C:\Program Files (x86)\MySQL\MySQL Connector J\mysql-connector-java-x.x.xx-bin.jar`
          - `localhost`
          - port is usually `3306`
          - Databse name: `BASDB` (change if different)
          - URL: `jdbc:mysql://localhost:3306/BASDB`
          - database username (default: root) & password
    - [**Jaspersoft® Studio**](http://community.jaspersoft.com/project/jaspersoft-studio) - The Eclipse-based Report Development Tool for JasperReports and JasperReports Server
      - [User Guide](http://community.jaspersoft.com/documentation/tibco-jaspersoft-studio-user-guide/v610/getting-started-jaspersoft-studio)
    - **Forum posts**
      - [AWARE'S REPORTING - JASPER REPORTS UPGRADE FOR NEXT RELEASE?](http://www.awareim.com/forum/viewtopic.php?f=1&t=7744) - JasperRepoerts Server
