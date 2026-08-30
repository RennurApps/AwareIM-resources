# Aware IM Server v10.1 Stack

## Application Server, Database Servers, Components, Frameworks, Dependencies, Microservices and other resources

---

> Aware IM is a rapid low-code application development tool that lets you create powerful aesthetically appealing web applications quickly.

[**Changelog**](https://docs.awareim.com/ref/changelog/10.1) 

✔️ [**v10.1 build 3726**](https://docs.awareim.com/ref/changelog/10.1/3726) - 29 Aug 2026.

- New Features and improvements in version 10.1
  - 3718 - [**`10.1` New Release**](https://docs.awareim.com/ref/changelog/10.1/3718) - 19 Aug 2026.

### Application Server

#### Apache Tomcat

<!--  Caution: Installing Aware IM update (Setup.exe), overwrites and resets Tomcat & JDK folders back to default. In fact, all files are replaced during update. Always keep all new and amended files incl. images separately and copy+paste them back once the install is complete. -->

#### [**👍 Tomcat `11.0.25`**](http://tomcat.apache.org/) - 12 Aug, 2026. 11.0.6 bundled with the latest Aware IM. Tomcat 11 is designed to run on `Java 17 or later`. 

- [**Download Tomcat v11**](https://tomcat.apache.org/download-11.cgi) - 64bit recommended. Manual Install required.

#### [**📉 Tomcat `10.1.57`**](http://tomcat.apache.org/) - 3 Jul, 2026. Tomcat 10 is designed to run on `Java SE 11 or later`

<!-- #### [**📉 Tomcat `9.0.120`**](http://tomcat.apache.org/) - **3 Jul, 2026. Tomcat 9 is designed to run on `Java SE 8 or later`** -->


#### Java JDK

- [**OpenJDK Java SE Releases**](https://jdk.java.net) - Oracle provides the latest **OpenJDK** releases under the open source.

  - ✔️ [**Oracle OpenJDK `26.0.2.1`**](https://jdk.java.net/26/) - Production-ready open-source builds of the Java Development Kit
    - 📉 [Archived Versions](https://jdk.java.net/archive/)

- [**Commercial Java SE Development Kit (JDK)**](https://www.oracle.com/au/java/technologies/downloads/) <!-- [Important Oracle JDK License Update starting April 16, 2019](https://www.oracle.com/technetwork/java/javase/overview/oracle-jdk-faqs.html) -->

  - ✔️ [**JDK Version `26.0.2.1`**](https://www.oracle.com/anz/java/technologies/downloads/#java26) - Works with Aware IM version `10.1`.
  - 📉 [JDK Version `25.0.4.1`](https://www.oracle.com/anz/java/technologies/downloads/#java25) - Works with Aware IM version `10.1`. 
  - 👍 [JDK Version `21.0.12.1`](https://www.oracle.com/anz/java/technologies/downloads/#java21) - 21.0.5 is default for `10.1`. 
  - Versions bundled with Aware IM:
    - Aware IM `v9.0` - [JDK `17.0.6`](https://docs.oracle.com/en/java/javase/17/)
    - Aware IM `v8.6 - v8.8` - [JDK `12.0.2` Final](https://docs.oracle.com/en/java/javase/12/) - Archived.
    - Aware IM `v8.0 - v8.5` - JDK 8 Update 91 `1.8.0_91-b15`
  - [**All previous JDK versions archive**](https://www.oracle.com/java/technologies/downloads/archive/)
    - [Manual Downloads](https://java.com/en/download/manual.jsp)

#### Java Servlets

<!-- - ✔️ [**Jakarta Mail `1.6.8`**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/) - Jul 23, 2025 Final Release. (formerly JavaMail)

  - [**Download jakarta.mail-1.6.8.jar**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/1.6.8) or [here](https://repo1.maven.org/maven2/com/sun/mail/jakarta.mail)
    - **Installation**
      - In Aware IM **v8.3 and above**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\lib`_
      - In Aware IM **v8.2 and below**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\Tomcat\lib`_
      - Restart Aware IM server
  - 📉 [JavaMail 1.6.2](https://javaee.github.io/javamail/) - August 30, 2018 Final Release. (superseded by JakartaMail) -->

- [**Apache ActiveMQ Classic**](http://activemq.apache.org/) - The most popular and powerful open source messaging and Integration Patterns server. Apache [ActiveMQ](https://en.wikipedia.org/wiki/Apache_ActiveMQ) is an open source message broker written in Java together with a full Java Message Service (JMS) client.

  > 👍 ActiveMQ `6.1.7` (22/06/2025) packaged with Aware IM.

  - **Releases**:
    - ✔️ [6.3.1 Release](https://activemq.apache.org/components/classic/download/classic-06-03-01) - Works with latest version 10.1. 
      - Installation
        - Extract and rename `activemq-all-6.3.1.jar` to `activemq-all-6.1.7.jar` and replace the one in `C:\AwareIM\lib`
    - 👍 [6.1.7 Release](https://activemq.apache.org/components/classic/download/classic-06-01-07) - Default version packaged with 10.1.
    - 📉 [**5.19.10 Release**](https://activemq.apache.org/components/classic/download/classic-05-19-10) - 10 Aug, 2026. Java 11+ required. 
    - 📉 [Download Archichives](https://activemq.apache.org/components/classic/documentation/download-archives) 

- [**Java Service Wrapper** -](http://wrapper.tanukisoftware.com/doc/english/download.jsp) - **32bit v3.6.5** 64-bit Windows versions of the Java Service Wrapper are not currently being made available in the Community Edition.

  - [**Licensing Overview**](https://wrapper.tanukisoftware.com/doc/english/licenseOverview.html) - Choosing an Appropriate License.

<!-- - [**Apache Axis2/Java**](https://axis.apache.org/axis2/java/core/) - Apache Axis2 Web Services JSON / SOAP / WSDL engine. -->

### Database Servers

- #### **MySQL**

  - [**MySQL Community Server**](http://www.mysql.com/products/community/)
    - [Supported Platforms: MySQL Database](https://www.mysql.com/support/supportedplatforms/database.html)
    - **Download MySQL**
      - ✔️ [**MySQL Community Server 9.7.2 LTS**](http://dev.mysql.com/downloads/mysql/) July 2026.
        - Min Requirement: `Win 11`, `Windows Server 2016`, `macOS 13`, `Oracle Linux 7` / `Red Hat Enterprise Linux 7` / `CentOS 7`
      - 👍 [MySQL Community Server 8.4.11 LTS](http://dev.mysql.com/downloads/mysql/) - July 2026.
        - Min Requirement: `Win 10`, `Windows Server 2016`, `macOS 13`, `Oracle Linux 7` / `Red Hat Enterprise Linux 7` / `CentOS 7`
      - 📉 [MySQL Community Server `8.0.46`](http://dev.mysql.com/downloads/mysql/) - April 2026.
      - 📉 [MySQL Community Server `5.7.44`](https://downloads.mysql.com/archives/community/) - Archived.
    - Installation on Windows requires:
      - [**Visual C++ v14 Redistributable**](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170) - Required by MySQL `8.0`, `8.3` and `5.7.38 and above`
      - [**Visual Studio 2013**](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170) - Required by MySQL `5.7.9 - 5.7.39`

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
  - [Download](https://www.postgresql.org/download/) - Version `18.6` <!-- https://endoflife.date/postgresql -->

- **Maria DB**

  - [**MariaDB**](https://mariadb.org/) - Free and open-source software under the GNU General Public License.
  - [Download](https://mariadb.org/download/) - Version `12.3.2`.

- [**SQL Server**](https://www.microsoft.com/en-in/sql-server/)

  - [Download](https://www.microsoft.com/en-in/sql-server/sql-server-downloads)

- [**Oracle**](https://www.oracle.com/database/)
  - [Download](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html) - Oracle Database. <!-- https://endoflife.date/oracle-database -->

#### Database Connectors

- [**MySQL Connectors**](https://www.mysql.com/products/connector/)

  - ✔️ [**Connector/J `26.7.0`**](https://dev.mysql.com/downloads/connector/j/) - **Latest version `26.7.0`**. Requires `Java 8` and `above`. 
    - [**Download Platform Independent Version**](https://dev.mysql.com/downloads/connector/j/)
    - **Installation**
      - Application Server
        1. Extract the files and rename `mysql-connector-java-26.x.x-bin.jar` to `mysql-connector-j-8.0.31.jar`
        2. Copy and replace the existing file in `C:\AwareIM\lib`
        3. Restart AwareIM Server
  - 📉 [**Connector/J `9.7`**](https://downloads.mysql.com/archives/c-j/) - Archived. Requires `Java 8` and `above`. 
  - 📉 [Connector/J `8.4`](https://downloads.mysql.com/archives/c-j/) - Final version. Archived.

- [**PostgreSQL JDBC Connector**](https://jdbc.postgresql.org/download/) - Current version `42.7.13`. Java 8 required.

- [**MariaDB Connectors**](https://mariadb.com/kb/en/library/connectors/)

  - ✔️ [**MariaDB Connector/J `2.3.0`**](https://mariadb.org/connector-java/all-releases/) - Out-of-the-box support in Aware IM `v8.3`+. Java `8+`
  - :warning: [MariaDB Connector/J `3.5.10`](https://mariadb.org/download/?t=connector&p=connector-java&r=3.5.10&os=source)

### **Web Application Framework**

- [**Kendo UI®**](https://www.telerik.com/kendo-ui) - Kendo UI for jQuery delivers everything you need for data handling, data grids, forms, navigation, performance, UX, design, accessibility, and so much more.
  - [**Roadmap**](https://www.telerik.com/support/whats-new/kendo-ui/roadmap)
  - [**Release History - jQuery**](https://www.telerik.com/support/whats-new/kendo-ui/release-history)
    - Latest Kendo UI Release [**Kendo UI for jQuery 2026.3.811 (2026 Q3)**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-for-jquery-2026-3-811-(2026-q3)) - August 12, 2026.
    - 👍 **Aware IM `10.1` Kendo UI version** [**Kendo UI R2 2023 SP1**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r2-2023-sp1-(version-2023-2-718)) - July 19, 2023
    - 👍 Aware IM `9.0` Kendo UI version [**Kendo UI R2 2023 SP1**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r2-2023-sp1-(version-2023-2-718)) - July 19, 2023
    - 📉 Aware IM `8.6 - 8.8` Kendo UI version [Kendo UI R3 2020 SP1](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2020-sp1) - October 21, 2020
    - 📉 Aware IM `8.1 - 8.5` Kendo UI version [Kendo UI R3 2017](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2017) - September 13, 2017
    - 📉 Aware IM `7.0 - 8.0` Kendo UI version [Kendo UI Q1 2016](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-q1-2016) - January 12, 2016
  - [**jQuery Demos & Examples**](https://demos.telerik.com/kendo-ui/) - Kendo UI jQuery Components

#### Front-end open source toolkit

- **Bootstrap** - Frontend toolkit.

  - ❔ [Bootstrap `v5.3.8`](https://getbootstrap.com/)
  - ❔ [Bootstrap `v4.6.2`](https://getbootstrap.com/docs/4.6/getting-started/introduction/)
  - ✔️ [**Bootstrap v3**](https://getbootstrap.com/docs/3.4/) - **`3.4.1` (final)**. Bootstrap `3.3.4` bundled with Aware IM `v10.1`.
    - [Download `v3.4.1`](https://getbootstrap.com/docs/3.4/getting-started/#download)
    - [Bootstrap `v3.4` CDN](https://getbootstrap.com/docs/3.4/getting-started/#download-cdn)
  - [All Bootstrap Versions](https://getbootstrap.com/docs/versions/)
  - [List of 300+ bootstrap resources](https://expeditedsecurity.com/the-big-badass-list-of-bootstrap-resources/)
  <!--    - **Plug into Aware IM**
        - Manual configuration through **Startup.html**
        - disable **`legend`** style as it seems to be in conflict with the ExtJS style
          - `/* legend { display: block; width: 100%; padding: 0; margin-bottom: 20px; font-size: 21px; line-height: inherit; color: #333; border: 0; border-bottom: 1px solid #e5e5e5; } */` -->

##### Icons

- [**Font Awesome**](https://fontawesome.com/) - Icon library.

  - ❔ Font Awesome `7.3.1 For The Web` - Latest version [Download](https://fontawesome.com/) - Released  July 2026.
  - ✔️ [Font Awesome version `6.7.2 For The Web`](https://github.com/FortAwesome/Font-Awesome/releases/tag/6.7.2) - Final. Released December 2024.
  - 👍 Aware IM `10.1` bundles [Font Awesome version `6.7.1 For The Web`](https://github.com/FortAwesome/Font-Awesome/releases/tag/5.6.3) - Released November 2024.

- [**Lineicons**](https://lineicons.com/icons/) - An extensive library of over 8400 professionally designed SVG icons

  - Lineicons Free `4.0 basic` included.

- [**Kendo UI Iconography**](https://www.telerik.com/design-system/docs/foundation/iconography/styles-and-guidelines/)

  <!--   - [Front-end Frameworks with comparison](http://bit.ly/RAfrontend) - Collection of best front-end frameworks -->
  <!--  - [Front End Development Bookmarks](http://bit.ly/FrontEndList) - A huge list of frontend development resources collected over time. -->

### Out-of-the-box Features

- **Integration with Stripe Multi-Payment** - Stripe is a very well-known payment platform and it supports multi-party payments. <!-- [Video](https://youtu.be/4m9YNPrpsvk%22) -->

- **Sign-on Glass / Electronic Signature Capture** - For Aware IM `5.9 - 9.x`
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

  - **Requires** [**Visual C++ v14 Redistributable**](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)
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
