# Aware IM Server v9.0 Stack

## Application Server, Database Servers, Components, Frameworks, Dependencies, Microservices and other resources

---

> Aware IM is a rapid low-code application development tool that lets you create powerful aesthetically appealing web applications quickly.

[**Changelog**](https://www.awareim.com/dokuwiki/doku.php/changelog/9.0) <!--(http://www.awareim.com/changelog/?C=M;O=D) -->

✔️ [**v9.0 build 3280**](https://www.awareim.com/dokuwiki/doku.php/changelog/9.0/3280) - 23 September, 2024.

- New Features and improvements in version 9.0
  - 3279 - Using standard CSV export now creates unique file names, so there is no conflict when people export at the same time
  - 3279 - New options for EXPORT action - do not export a line with column descriptions, do not export attribute format and use labels in the column descriptions
  - 3279 - Ability to specify selection mechanism for custom queries
  - 3273 - 'load on demand' in grouped queries supports sorting and paging properly
  - 3273 - Performance improvements for big complicated forms with many presentation rules
  - 3273 - Improvements to Scroll View in custom queries
    - new UI
    - allow displaying several items per page
    - preview fixes
    - example in CRM
  - 3273 - Support for client credentials flow in OAuth
  - 3273 - “name field for binary REST part
  - 3271 - ['load on demand' for grouped queries supports filtering and paging](https://www.awareim.com/dokuwiki/doku.php/docs/2500_config_apps/1100_add_edit_queries/0200_display_results/0100_standard_view#load_data_on_demand)
  - 3265 - [[DISPLAY](https://www.awareim.com/dokuwiki/doku.php/a_f/a/display)]/[[PICK FROM](https://www.awareim.com/dokuwiki/doku.php/a_f/a/pick_from)] … [USING QueryName]
  - 3263 - [Multi-checkbox filter for standard queries](https://www.awareim.com/dokuwiki/doku.php/docs/2500_config_apps/1100_add_edit_queries/0200_display_results/0700_query_filters#multi-checkbox_filter)
  - 3260 - [CREATE FOR EACH STRING](https://www.awareim.com/dokuwiki/doku.php/a_f/a/create)
  - 3260 - [PARSE_JSON2 function](https://www.awareim.com/dokuwiki/doku.php/a_f/f/af/parse_json2) - Returns the value of the specified attribute in the same node
  - 3260 - Ability to direct actions in the template builder of a custom query to a `<DIV>`
  - 3259 - Ability to save all REST communication details in a log (business object)
  - 3257 - Loading content on demand for grouped queries - very useful for larger sets of data
  - 3254 - Grouping now calculates summaries correctly even for big data sets
  - 3254 - Support for group direction
  - 3254 - Support for displaying group summaries in the group header column
  - 3254 - Query preview is now supported for queries with grouping
  - 3254 - Support for aggregates for all group levels
  - 3254 - Ability to initially collapse any group
  - 3254 - Ability to hide aggregates in column headers when a group is expanded
  - 3254 - Auto refresh didn't work when calendar events were moved or resized
  - 3254 - Left menu toggle command didn't work correctly when the top menu ran across the entire screen
  - 3249 - New library for rendering HTML inside a PDF
  - 3249 - Scaling image option for tags representing images in the Report Designer
  - 3249 - Changing size and orientation of the report is now visually supported.
  - 3246 - Date, time and duration widgets support mobile rendering
  - 3246 - Multi-selection calendar widget - [Demo](https://demos.telerik.com/kendo-ui/calendar/selection)
  - 3246 - [CREATE FOR EACH DATE IN …](https://www.awareim.com/dokuwiki/doku.php/a_f/a/create) - [Forum Post](https://awareim.com/forum/viewtopic.php?f=1&t=12893)
  - 3243 - Custom row filter now supports attributes with dynamic choices
  - 3243 - Placeholders for Line Icons PRO font
  - 3241 - Support for alignment in tiles
  - 3241 - Minor improvements of dialogs on a Mac
  - 3241 - It should now be possible to explicitly indicate if a visual perspective can be used as a URL parameter
  - 3237 - Tile dialog has better layout and supports Preview
  - 3237 - Tree queries support paging (multi-column only)
  - 3237 - Custom queries support paging options
  - 3232 - [**`9.0` New Release**](https://www.awareim.com/dokuwiki/doku.php/changelog/9.0/3232) - 28 Jan 2024.

### Application Server

#### Apache Tomcat

> Caution: Installing Aware IM update (Setup.exe), overwrites and resets Tomcat & JDK folders back to default. In fact, all files are replaced during update. Always keep all new and amended files incl. images separately and copy+paste them back once the install is complete.

- **Tomcat 9.0.44** 32bit is the default version packaged in the **Aware IM 8.6 and above** server installation.
- Tomcat 8.5.58 32bit is the default version packaged in the **Aware IM 8.5** server installation.
- Tomcat 8.5.24 32bit is the default version packaged in the **Aware IM 8.4 and below** server installation.

#### [**⚠️ Tomcat `10.1.31`**](http://tomcat.apache.org/) - 13 Sep, 2024. Tomcat 10 is designed to run on `Java SE 11 or later`

> ⚠️Tomcat output: <br>
> SEVERE: Servlet [action] in web application [/AwareIM] threw load() exception
> java.lang.ClassNotFoundException: javax.servlet.http.HttpServlet

- [**Download Tomcat v10**](https://tomcat.apache.org/download-10.cgi) - 64bit recommended. Manual Install required.

 <!-- - Works with AwareIM version `9.0`. -->

- [**Security**](https://tomcat.apache.org/security-10.html)

- [Tomcat 10 Documentation](https://tomcat.apache.org/tomcat-10.1-doc/index.html).
- [Tomcat 10 Changelog](https://tomcat.apache.org/tomcat-10.1-doc/changelog.html).

#### [**✔️ Tomcat `9.0.96`**](http://tomcat.apache.org/) - **3 October, 2024. Tomcat 9 is designed to run on `Java SE 8 or later`**

<!-- ** Tomcat `9.0.89+`** (http://tomcat.apache.org/) Has issues processing SSL:

<!-- Jun 20, 2024 7:40:09 PM org.apache.coyote.AbstractProtocol$ConnectionHandler process
SEVERE: Error reading request, ignored
java.lang.IllegalArgumentException
	at java.nio.ByteBuffer.allocate(ByteBuffer.java:334)
	at org.apache.coyote.http11.filters.ChunkedInputFilter.<init>(ChunkedInputFilter.java:120)
	at org.apache.coyote.http11.Http11Processor.<init>(Http11Processor.java:172)
	at org.apache.coyote.http11.AbstractHttp11Protocol.createProcessor(AbstractHttp11Protocol.java:1358)
	at org.apache.coyote.AbstractProtocol$ConnectionHandler.process(AbstractProtocol.java:924)
	at org.apache.tomcat.util.net.Nio2Endpoint$SocketProcessor.doRun(Nio2Endpoint.java:1734)
	at org.apache.tomcat.util.net.SocketProcessorBase.run(SocketProcessorBase.java:52)
	at org.apache.tomcat.util.net.AbstractEndpoint.processSocket(AbstractEndpoint.java:1333)
	at org.apache.tomcat.util.net.SecureNio2Channel$HandshakeWriteCompletionHandler.completed(SecureNio2Channel.java:124)
	at org.apache.tomcat.util.net.SecureNio2Channel$HandshakeWriteCompletionHandler.completed(SecureNio2Channel.java:117)
	at sun.nio.ch.Invoker.invokeUnchecked(Invoker.java:126)
	at sun.nio.ch.Invoker$2.run(Invoker.java:218)
	at sun.nio.ch.AsynchronousChannelGroupImpl$1.run(AsynchronousChannelGroupImpl.java:112)
	at org.apache.tomcat.util.threads.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1190)
	at org.apache.tomcat.util.threads.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:659)
	at org.apache.tomcat.util.threads.TaskThread$WrappingRunnable.run(TaskThread.java:63)
	at java.lang.Thread.run(Thread.java:750) -->

- [**Download Tomcat v9**](https://tomcat.apache.org/download-90.cgi)

  - Works with AwareIM versions `6.0` - `9.0`
  - [**Security**](https://tomcat.apache.org/security-9.html)

  - [Tomcat 9 Documentation](https://tomcat.apache.org/tomcat-9.0-doc/index.html).
  - [Tomcat 9 Changelog](https://tomcat.apache.org/tomcat-9.0-doc/changelog.html).

- **Installation**
    <details>

    <summary>Microsoft Windows Based Systems</summary>

  - **IMPORTANT**: Ensure any prior modification of existing _`web.xml`_ and _`server.xml`_ configurations are not overwritten with the new version. There are configuration changes in the latest version of Tomcat relating to those two files.
  - **Installation Steps - Windows**
    - Stop the Aware IM server before updating Tomcat. Do **not** delete your current _C:\AwareIM\Tomcat_ folder.
    - 1. **Extract** the archive and open the folder.
    - 2. Open the extracted **Tomcat** folder.
    - 3. Select all files and folders and press `Crl+c` to copy
    - 4. Open you AwareIM v9.0 installation Tomcat folder **`C:\AwareIM\Tomcat`**
    - 5. Press `Ctrl+v` to paste and replace all files and folders.
    - 6. Rename or delete **ROOT** folder - _This is optional_. You can use this folder to store your own favicon.ico, error pages and other HTML/CSS/JS home page files.
      </details>

#### Java JDK

- [**OpenJDK Java SE Releases**](https://jdk.java.net) - Oracle provides the latest **OpenJDK** releases under the open source.

  - ✔️ [**Oracle OpenJDK `23.0.1`**](https://jdk.java.net/23/) - Production-ready open-source builds of the Java Development Kit
  - Superseded versions:
    <!-- - 📉 [Oracle OpenJDK `20`](https://jdk.java.net/20/)
     - 📉 [Oracle OpenJDK `19`](https://jdk.java.net/19/) -->
    <!-- - 📉 [Oracle OpenJDK `17`](https://jdk.java.net/17/) --> 
    - 📉 [Archived Versions](https://jdk.java.net/archive/)

- [**Commercial Java SE Development Kit (JDK)**](https://www.oracle.com/au/java/technologies/downloads/) <!-- [Important Oracle JDK License Update starting April 16, 2019](https://www.oracle.com/technetwork/java/javase/overview/oracle-jdk-faqs.html) -->

  - ✔️ [**JDK Version `23.0.1`**](https://www.oracle.com/au/java/technologies/downloads/#java23) - Works with Aware IM version `9.0`. 15 October 2024.
  - 👍 [JDK Version `21.0.5`](https://www.oracle.com/au/java/technologies/downloads/#java21) - Works with Aware IM version `9.0`. 15 October 2024.
  - 👍 [JDK Version `17.0.13`](https://www.oracle.com/au/java/technologies/downloads/#java17) - Works with Aware IM version `8.6` - `9.0`. 15 October 2024.
  - 👍 [JDK Version `8, Update 431`](https://www.oracle.com/au/java/technologies/downloads/#java8) - Aware IM versions `6.0` - `8.5`. 15 October 2024. 
  - Versions bundled with Aware IM:
    - Aware IM `v9.0` - [JDK `17.0.6`](https://docs.oracle.com/en/java/javase/17/)
    - Aware IM `v8.6 - v8.8` - [JDK `12.0.2` Final](https://docs.oracle.com/en/java/javase/12/) - Archived.
    - Aware IM `v8.0 - v8.5` - JDK 8 Update 91 `1.8.0_91-b15`
  - [**All previous JDK versions archive**](https://www.oracle.com/java/technologies/downloads/archive/)
    - [Manual Downloads](https://java.com/en/download/manual.jsp)

#### Java Servlets

- ✔️ [**Jakarta Mail `1.6.7`**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/) - April 8, 2021 Final Release. (formerly JavaMail)

  - [**Download jakarta.mail-1.6.7.jar**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/1.6.7)
    - **Installation**
      - In Aware IM **v8.3 and above**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\lib`_
      - In Aware IM **v8.2 and below**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\Tomcat\lib`_
      - Restart Aware IM server
  - 📉 [JavaMail 1.6.2](https://javaee.github.io/javamail/) - August 30, 2018 Final Release. (superseded by JakartaMail)

- [**Apache ActiveMQ™**](http://activemq.apache.org/) - The most popular and powerful open source messaging and Integration Patterns server. Apache [ActiveMQ](https://en.wikipedia.org/wiki/Apache_ActiveMQ) is an open source message broker written in Java together with a full Java Message Service (JMS) client.

  > 📉 ActiveMQ `5.8.0` (06/02/2013) packaged with Aware IM.

  - 📉 Latest version of ActiveMQ that works with out-of-box installation of Aware IM is **`5.12.1`** (13 Oct 2015).

  <!-- - **Reported issues in Aware IM** - Scalability, bugs, performance...
    - [Highly demand -- updates - security concerns](https://awareim.com/forum/viewtopic.php?f=1&t=10539&p=48389)
    - [How many Communication driven apps can we host on 1 serv](https://awareim.com/forum/viewtopic.php?f=1&p=51529)
  - [**Issues**](https://github.com/RennurApps/AwareIM-resources/issues) - Refer to the Issues tab. -->

  - **Releases**:
    - ⚠️ [6.1.3 Release](https://activemq.apache.org/components/classic/download/classic-06-01-03) - 8 August, 2024. Java 17+ required.
    - ⚠️ [5.18.5 Release](https://activemq.apache.org/components/classic/download/classic-05-18-05) - 24 August, 2024. Java 11+ required.
    - ⚠️ [5.17.6 Release](https://activemq.apache.org/components/classic/download/classic-05-17-06) - 25 October, 2023. Java 11+ required.
    - ⚠️ [5.12.2+ Problem](https://activemq.apache.org/components/classic/download/classic-05-12-02) - **Inconsistent vector internals** Aware IM error.
      - ERROR:
        - `org.openadaptor.adaptor.jms.JMSListener - onMessage: JMSException: [javax.jms.JMSException: Failed to build body from bytes. Reason: java.io.StreamCorruptedException: Inconsistent vector internals [java.io.StreamCorruptedException: Inconsistent vector internals]]`
      - Changelog
        - This release enables ActiveMQ client TLS hostname validation by default which can cause a client connection failure for server certificates that do not match the server hostname. Please refer to SSL Transport Reference for configuration and [AMQ-7047](https://issues.apache.org/jira/browse/AMQ-7047) for more information.
        - Java 8 Required - The minimum Java version has been upgraded to Java 8.
        - This release affects applications using ObjectMessages.
    - ✔️ [**5.12.1 Release**](https://activemq.apache.org/components/classic/download/classic-05-12-01)
      - Installation
        - In **v8.3 and above**, extract, rename `activemq-all-x.xx.x.jar` to `activemq-all-5.8.0.jar` and replace the one in `C:\AwareIM\lib`
        <!--  - In v8.2 and below, extract, rename `activemq-all-x.xx.x.jar` to `activemq-all-5.8.0.jar` and replace the one in `C:\AwareIM\Tomcat\lib` -->
    - 📉 [**5.8.0 Release**](https://activemq.apache.org/components/classic/download/classic-05-08-00) - Default version packaged with the server installation.

- [**Java Service Wrapper** -](http://wrapper.tanukisoftware.com/doc/english/download.jsp) - **32bit v3.5.56** 64-bit Windows versions of the Java Service Wrapper are not currently being made available in the Community Edition.

  - [**Licensing Overview**](https://wrapper.tanukisoftware.com/doc/english/licenseOverview.html) - Choosing an Appropriate License.

- [**Apache Axis2/Java**](https://axis.apache.org/axis2/java/core/) - Apache Axis2 Web Services JSON / SOAP / WSDL engine.

### Database Servers

- #### **MySQL**

  - [**MySQL Community Server**](http://www.mysql.com/products/community/)
    - [Supported Platforms: MySQL Database](https://www.mysql.com/support/supportedplatforms/database.html)
    - **Download MySQL**
      - ⚠️ [MySQL Community Server 9.1.0 Innovation](http://dev.mysql.com/downloads/mysql/) - [New Release](https://dev.mysql.com/doc/refman/9.1/en/) 15 October 2024.
        - Min Requirement: `Win 11`, `Windows Server 2016`, `macOS 13`, `Oracle Linux 7` / `Red Hat Enterprise Linux 7` / `CentOS 7`
      - ⚠️ [MySQL Community Server 8.4.3 LTS](http://dev.mysql.com/downloads/mysql/) - 15 October 2024.
        - Min Requirement: `Win 11`, `Windows Server 2016`, `macOS 13`, `Oracle Linux 7` / `Red Hat Enterprise Linux 7` / `CentOS 7`
      - ✔️ [**MySQL Community Server `8.0.40`**](http://dev.mysql.com/downloads/mysql/) - 15 October 2024.
      - 📉 [MySQL Community Server `5.7.44`](https://downloads.mysql.com/archives/community/) - Archived.
    - Installation on Windows requires:
      - [**Visual Studio 2015, 2017, 2019, and 2022**](https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170) - Required by MySQL `8.0`, `8.3` and `5.7.38 and above`
      - [**Visual Studio 2013**](https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170) - Required by MySQL `5.7.9 - 5.7.39`

- **Apache Derby** - [Home](http://db.apache.org/derby/)
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
- **PostgreSQL**

  - [PostgreSQL](https://www.postgresql.org/) is a powerful, open source object-relational database system.
  - [Download](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) - Version `16.4` <!-- https://endoflife.date/postgresql -->

- **Maria DB**

  - [**MariaDB**](https://mariadb.org/) - Free and open-source software under the GNU General Public License.
  - [Download](https://mariadb.org/download/) - Version `11.5.2`.

- [**SQL Server**](https://www.microsoft.com/en-in/sql-server/)

  - [Download](https://www.microsoft.com/en-in/sql-server/sql-server-downloads)

- [**Oracle**](https://www.oracle.com/database/)
  - [Download](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html) - Oracle Database. <!-- https://endoflife.date/oracle-database -->

#### Database Connectors

- [**MySQL Connectors**](https://www.mysql.com/products/connector/)

  - ✔️ [**Connector/J `9.1`**](https://dev.mysql.com/downloads/connector/j/) - **Latest version `v9.1.0`**. Requires `Java 8` and `above`. Connector/J 8.3 supports MySQL `5.7`, `8.0`, and `8.3`.

    - [**Download Platform Independent Version**](https://dev.mysql.com/downloads/connector/j/)
    - **Installation**
      - Application Server
        1. Extract the files and rename `mysql-connector-java-9.x.xx-bin.jar` to `mysql-connector-j-8.0.31.jar`
        2. Copy and replace the existing file in `C:\AwareIM\lib`
        3. Restart AwareIM Server

  - 📉 [Connector/J `8.4`](https://downloads.mysql.com/archives/c-j/) - Final version `v8.4`. Archived.

- [**PostgreSQL JDBC Connector**](https://jdbc.postgresql.org/download/) - Current version `42.7.4`. Java 8 required.

- [**MariaDB Connectors**](https://mariadb.com/kb/en/library/connectors/)

  - ✔️ [**MariaDB Connector/J `2.3.0`**](https://mariadb.com/kb/en/about-mariadb-connector-j/) - Out-of-the-box support in Aware IM `v8.3`+. Java `8+`
  - :warning: [MariaDB Connector/J `3.4.1`](https://mariadb.com/kb/en/mariadb-connector-j-3-4-0-release-notes/)

### **Web Application Framework**

- [**Kendo UI®**](https://www.telerik.com/kendo-ui) - Kendo UI for jQuery delivers everything you need for data handling, data grids, forms, navigation, performance, UX, design, accessibility, and so much more.
  - [**Roadmap**](https://www.telerik.com/support/whats-new/kendo-ui/roadmap)
  - [**Release History - jQuery**](https://www.telerik.com/support/whats-new/kendo-ui/release-history)
    - Latest Kendo UI Release [**Kendo UI for jQuery 2024.3.806 (2024 Q3)**](<https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-for-jquery-2024-3-806-(2024-q3)>) - August 7, 2024
    - 👍 **Aware IM `9.0` Kendo UI version** [**Kendo UI R2 2023 SP1**](<https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r2-2023-sp1-(version-2023-2-718)>) - July 19, 2023
    - 📉 Aware IM `8.6 - 8.8` Kendo UI version [Kendo UI R3 2020 SP1](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2020-sp1) - October 21, 2020
    - 📉 Aware IM `8.1 - 8.5` Kendo UI version [Kendo UI R3 2017](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2017) - September 13, 2017
    - 📉 Aware IM `7.0 - 8.0` Kendo UI version [Kendo UI Q1 2016](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-q1-2016) - January 12, 2016
  - [**jQuery Demos & Examples**](https://demos.telerik.com/kendo-ui/) - Kendo UI jQuery Components

#### Front-end open source toolkit

- **Bootstrap** - Frontend toolkit.

  - ❔ [Bootstrap `v5.3.3`](https://getbootstrap.com/)
  - ❔ [Bootstrap `v4.6.2`](https://getbootstrap.com/docs/4.6/getting-started/introduction/)
  - ✔️ [**Bootstrap v3**](https://getbootstrap.com/docs/3.4/) - **`3.4.1` (final)**. Bootstrap `3.3.4` bundled with Aware IM `v9.0`.
    - [Download `v3.4.1`](https://getbootstrap.com/docs/3.4/getting-started/#download)
    - [Bootstrap `v3.4` CDN](https://getbootstrap.com/docs/3.4/getting-started/#download-cdn)
  - [All Bootstrap Versions](https://getbootstrap.com/docs/versions/)
  - [List of 300+ bootstrap resources](https://expeditedsecurity.com/the-big-badass-list-of-bootstrap-resources/)
  <!--    - **Plug into Aware IM**
        - Manual configuration through **Startup.html**
        - disable **`legend`** style as it seems to be in conflict with the ExtJS style
          - `/* legend { display: block; width: 100%; padding: 0; margin-bottom: 20px; font-size: 21px; line-height: inherit; color: #333; border: 0; border-bottom: 1px solid #e5e5e5; } */` -->

##### Icons

- [**Font Awesome 5**](https://fontawesome.com/) - Icon library.

  - ❔ Font Awesome `5.15.4 For The Web` - Latest version [Download](https://fontawesome.com/v5/download)
  - ✔️ Aware IM `9.0` bundles [Font Awesome version `5.6.3 For The Web`](https://github.com/FortAwesome/Font-Awesome/releases/tag/5.6.3).

- [**Lineicons**](https://lineicons.com/icons/) - An extensive library of over 8400 professionally designed SVG icons

  - Lineicons Free `4.0 basic` included.

- [**Kendo UI Iconography**](https://www.telerik.com/design-system/docs/foundation/iconography/styles-and-guidelines/)

  <!--   - [Front-end Frameworks with comparison](http://bit.ly/RAfrontend) - Collection of best front-end frameworks -->
  <!--  - [Front End Development Bookmarks](http://bit.ly/FrontEndList) - A huge list of frontend development resources collected over time. -->

### Out-of-the-box Features

- **Integration with Stripe Multi-Payment** - Stripe is a very well-known payment platform and it supports multi-party payments. <!-- [Video](https://youtu.be/4m9YNPrpsvk%22) -->

- **Electronic Signature Capture** - For Aware IM `5.9 - 9.x`
  - [**Signature Pad**](https://github.com/szimek/signature_pad) - Implement and store electronic signatures out-of-the-box with Aware IM. HTML5 canvas based and works in all modern desktop and mobile browsers.
  - [**DEMO - Github**](http://szimek.github.io/signature_pad/)
  - [✔️ **Signature Pad `v1.5.3`**](https://www.jsdelivr.com/package/npm/signature_pad?version=1.5.3) - Tested and working in all versions `5.9 - 9.x`
  - **Installation**:
    - Replace ../AwareIM/signature/signature_pad.js with the new version.
  - **Options** - Edit **signature_pad.js** found in **C:\AwareIM\Tomcat\webapps\AwareIM\signature**
    - `dotSize` - (float or function) Radius of a single dot.
    - `minWidth` - (float) Minimum width of a line. Defaults to 0.5.
    - `maxWidth` - (float) Maximum width of a line. Defaults to 2.5.
    - **`backgroundColor`** - (string) Color used to clear the background. Can be any color format accepted by context.fillStyle. Defaults to `rgba(0,0,0,0)` (transparent black).
      - I prefer a **white background `rgb(255,255,255)`** for the signatures since there are issues with transparent images in the Report Designer and PDF document export.
    - `penColor` - (string) Color used to draw the lines. Can be any color format accepted by context.fillStyle. Defaults to "black".
    - `velocityFilterWeight` - (float) Weight used to modify new velocity based on the previous velocity. Defaults to 0.7.
    - `onBegin` - (function) Callback when stroke begin.
    - `onEnd` - (function) Callback when stroke end.
  - [Video Tutorial (approx. 3min)](http://www.awareim.com/tutorials/59/New%20In%205,9.html) - from 00:38min

### Interoperability: Integrations, custom components, connected apps and plugins

Developers can integrate any application with Aware IM by writing a plugin, as long as the application offers an API.

- ✔️ [**wkhtmltopdf**](https://github.com/wkhtmltopdf/wkhtmltopdf) - wkhtmltopdf is a command line tool to render HTML into PDF using the QT Webkit rendering engine. These run entirely "headless" and do not require a display or display service.

  - **Requires** [**Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017, 2019, and 2022**](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)
  - **Download wkhtmltopdf**:
    - [**Download wkhtmltopdf** Windows (MSVC)](https://wkhtmltopdf.org/downloads.html) - **v`0.12.6`** released on June 11, 2020 for Windows, Linux and OS X.
      - **`v0.12.6 Final`** Tested and working in Aware IM **6.0+**. Released June 11, 2020. Archived.
  - **Install wkhtmltopdf**
    - Windows OS
      - Extract `*.exe` file to a folder (you can use [7-Zip](http://www.7-zip.org/)), copy+paste `wkhtmltopdf` folder to `c:/AwareIM/`
  - **Aware IM Process Rules**
    - **Step 1** - Export Aware IM HTML Document to a HTML file
      - `EXPORT DOCUMENT 'Your HTML Document' TO FILE 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html'`
    - **Step 2** - Convert exported HTML file to PDF
      - `EXECUTE PROGRAM 'C:\AwareIM\wkhtmltopdf\bin\wkhtmltopdf.exe file:///C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.pdf'`
    - **Step 3** - Import PDF document to your myBO.DocumentPDF attribute
      - `IMPORT DOCUMENT myBO.DocumentPDF FROM 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.pdf'`
    - **Optional** - Delete exported HTML file
      - `DELETE FILE 'C:/YourFileLocation/<<myBO.Name>>_No<<myBO.ID>>.html'`
  - Some alternatives to wkhtmltopdf:
    - [**Playwright**](https://playwright.dev/) - [Java `8+`](https://playwright.dev/java/) / Node.js / [Python `3.8+`](https://playwright.dev/python/) / .Net <!-- https://nagasudhir.blogspot.com/2023/09/html-to-pdf-conversion-in-python-with.html VIDEO: https://www.youtube.com/watch?v=_L6ELUJN-9Q -->
    - [WeasyPrint](https://github.com/Kozea/WeasyPrint) - For Python `3.7+`.
    - [Total HTML Converter](https://www.coolutils.com/TotalHTMLConverter)
    - [Prince XML](http://www.princexml.com/) - Commercial.
    - [PDFreactor](https://www.pdfreactor.com/) - Commercial. Works with any language.
    - [xhtml2pdf](https://pypi.org/project/xhtml2pdf/) - Python project.

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
          - Database name: `BASDB` (change if different)
          - URL: `jdbc:mysql://localhost:3306/BASDB`
          - database username (default: root) & password
    - [**Jaspersoft® Studio**](http://community.jaspersoft.com/project/jaspersoft-studio) - The Eclipse-based Report Development Tool for JasperReports and JasperReports Server
      - [User Guide](http://community.jaspersoft.com/documentation/tibco-jaspersoft-studio-user-guide/v610/getting-started-jaspersoft-studio)
    - **Forum posts**
      - [AWARE'S REPORTING - JASPER REPORTS UPGRADE FOR NEXT RELEASE?](http://www.awareim.com/forum/viewtopic.php?f=1&t=7744) - JasperReports Server
