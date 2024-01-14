# Aware IM Server v8.8 Stack

## Application Server, Database Servers, Components, Frameworks, Dependencies, Microservices and other resources

---

> Aware IM is a rapid low-code application development tool that lets you create powerful aesthetically appealing web applications quickly.

[**Changelog**](https://www.awareim.com/dokuwiki/doku.php/changelog/8.8) <!--(http://www.awareim.com/changelog/?C=M;O=D) -->

✅ Next Release - January 2024.

  <details>

   <summary>New Features</summary>

- New Java
- Latest Kendo UI library with new themes (new preview browser engine for Windows based on Edge). Two themes are show-cased in the CRM (Bootstrap 3) and Library apps (Aqua Dark theme)
- Support for high resolution in dialogs of the Configuration Tool
- Redesign of outgoing emails (they are now specified in business version properties just like incoming emails
- Support for OAuth in emails
- Redesign of filters:
- Generic filter control that filters for all specified attributes using OR (showcased in the CRM app)
- "User defined" filter (new)
- "Value list" filter (new) - showcased in the Issue Resolution Issues page ("Issue All" query)
- Ability to combine different forms of filters
- Filters are fully supported for standard, custom queries, charts and calendars
- Support for QRCodes in forms and custom queries.
In custom queries:
<div class="aw-qrcode-settings" border-width="2px" border-color="#ff0000" color=#00ff00" padding="15px">
{B,qrcode}
</div>
- Support for Barcodes in forms and custom queries (showcased in the SalesPortal app).
In custom queries:
<div class="aw-barcode-settings" type="code39" width="280" height="100">
{B,barcode}
</div>
- Support for Line Icons font (free) - when any icon in the Config. Tool is selected there is a button to select from the Line Icons font or from Font Awesome font

- Support for tiles.
  Tiles are boxes often used in dashboards. You can put content into a tile on a grid.
  Each of the 9 possible locations can have text or icon or chart (Kendo sparkline). A tile can be chosen as content of
  a content panel (like GM, HTML etc). You can export a tile into XML and import it - thus copying/pasting into different VPs.
  Tiles can be selected from templates. You can also add your own tile to the list of templates if you export a tile and put it in the
  new folder under AwareIM/TileTemplates. When a new tab is created in a VP you can initialise it with tiles
  Same when creating a new business space (in Themes, tiles and font size link). When adding text or charts you can specify tag
  expressions <<COUNT SystemUser>>. This is how you specify data for bullet and pie charts. For other charts data is collected using a query.
  There is also the Add Tiles button in the VP's toolbar that replaces the content of the current tab with selected tiles
  (showcased in the Dashboard in the CRM, Issue Resolution and Library apps)

- Button Group widget for text attributes with static choices (showcased in the CRM app in forms for OutgoingLetter and OutgoingEmail objects)

- Support for special editing widgets in standard queries - switches, rating, toggle button, button group. They work
  in the inline editing mode - if a column is not editable, they are displayed as read-only widgets. If the column is editable
  clicking on them immediately changes the value in the database and recalculates the current record. Toggle button works for Yes/No
  attributes and for text with choices, where it toggles through possible choices. Styling presentation rules of the corresponding
  attribute may determine the colors of the Toggle Button and buttons of a Button Group.
  These can be specified if you select a column of the grid and choose Display/Editing property. Or if you go to the properties of
  the column from Displayed Columns and click on the Column Display button
  (showcased in the CRM "Unsent Letters" query, also Issue Resolution - "Issues All" query, "Issues Closed" query)

- Support for WorkSheets (new node in the tree - can drag and drop into a WorkSheet, go to element, add items from Find References)
- Redesign of a Duration attribute - new widget to edit the format of duration (also supports the initial value) - showcased in CRM (
  forms of all objects that are members of the Communication group) (zeroes are not allowed)

Improvements:

- Default for Yes/No switch is Yes/No
- Improvements for Google Maps
- ability to specify marker shape and color (and custom marker) in presentation rules (new element type there Google Maps Marker)
- Presentation rules for labels can be used to display a label on the marker
- Get Directions operation can be used in Operations with Records for a query (if this query is used by a Google Map in a VP)
  Also, has an option to display detailed directions in a separate window
- Ablity to specify panel caption separately from Panel Header, which allows to use captions in popup wwindows, for example, when there is no panel header
- Panel Operations can now be allowed on forms when a new object is being created. A special flag when defining a panel operation
- YESNAME and NONAME keys for the DISPLAY QUESTION action: DISPLAY QUESTION 'Do you want to continue' YESNAME 'I do' NONAME 'I do not'
- Tree improvements (multi-column only)
- Item display rules are supported,
- Grouping of operations on records
- Checkbox selection (pick from)
- Trees now support business object groups
- If a tree is expanded, sorting and filtering is supported (including filter row).
- Stylistical improvements to the bootstrap theme (showcased in the CRM sample app)
- Modern and classic left menu style (showcased in the Library sample app, which has a Modern style left menu)
- FORCE POPUP option for ENTER NEW and EDIT actions to override "single tab mode"
- Scaling issue with ID_GEN and MySQL. New setting in BASServer.props MULTISERVER=true
- Select All/Deselect All for a multi-attribute cell dialog
- Label style available for pictures
- While consuming REST service it is possible to encode Yes/No as boolean (a new drop down in Request Body details.
- "Absolute positioning" property when editing forms to solve the problem of "tall" controls in forms - showcased in CRM (Customer Photo, Interests checkboxes)
- Support for grouping in combo boxes of references and multi-selectors (showcased in Issue Resolution - form of the Issue object (Assigned To)
- Scheduler improvements
- Yearly view with the ability to specify number of months to show (showcased in CRM - "Company Diary" query)
- Maximum events per day for monthly view
- Adaptive slot height for monthly view(showcased in CRM - Company Diary)
- Control of allocation of 'all day' slot
- Html Editor improvements
- Images can be scaled
- Ability to control which tools of the editor are available
- UI style for calendar widgets - classic and modern
- Compact size flag for standard queries
- Ability to add "chip" widget to custom queries:
<div class="aw-chip-settings" fill_mode="outline" icon="check"0>
{AttrName,chip}
</div>
- Process diagram - selected expression is now displayed on the right and supports context assistant
- Invisibility condition for content panels in visual perspectives
- Ability to set a style to a reference grid in the Form Designer
- Chart improvements:
- Ability to combine more chart types in series
- Area charts - stacked, show markers, smooth and stepped (Library sample app - dashboard)
- New chart types:
- Vertical bullet
- Range Bar
- Range Area
- Bubble
- Scatter
- Funnel
- Bullet (in a visual perspective only)(showcased in SalesPortal in the TeamEfficiency tab, also in Library - inside tiles)
- Circular and Arc gauge (showcased in tthe Issue Resolution dashboard)
- Gauges in visual perspective
- More properties for gauges
- Visibility of major and minor ticks of an axis
- Color ranges support for axis in charts and gauges (Issue Resolution dashboard)
- Support for start angle, 'explode' and auto fit content for pie and donuts (explode is showcased in the Library dashboard)
- Support for stepped line
- Radar - area and bar
- SUpport for multiple Y axes and axis crossing values (usually specified as X crossing value) - showcased in the CRM chart)
- Menu command to toggle visibility of the left menu (Library sample app - dashboard)
- DQ() function to generate double quotation marks
- Ability to specify settings for popup windows of processes and Add New Reference operations. Also menu items
- Ability to specify different choices in different forms
</details>

✔️ [**v8.8 build 3137**](https://www.awareim.com/dokuwiki/doku.php/changelog/8.8/3137) - 23 May, 2023.

- New Features and improvements in version 8.8
  - 3132 - Support for max file size, total max file size and allowed extensions for multi-file upload
  - 3127 - [“Resolve Shortcuts”](https://www.awareim.com/dokuwiki/doku.php/docs/2500_config_apps/1100_add_edit_queries/0100_query_props#resolve_shortcuts) property when defining a query (performance booster)
  - 3126 - Support for non-iterated property in reports
  - 3126 - [GET_ATTR_VALUE](https://www.awareim.com/dokuwiki/doku.php/a_f/f/af/get_attr_value) function
  - 3123 - [**List of `8.8` release improvements**](https://www.awareim.com/dokuwiki/doku.php/changelog/8.8/3123)

### Application Server

#### Apache Tomcat

> Caution: Installing Aware IM update (Setup.exe), overwrites and resets Tomcat & JDK folders back to default. In fact, all files are replaced during update. Always keep all new and amended files incl. images separately and copy+paste them back once the install is complete.

- **Tomcat 9.0.44** 32bit is the default version packaged in the **Aware IM 8.6 and above** server installation.
- Tomcat 8.5.58 32bit is the default version packaged in the **Aware IM 8.5** server installation.
- Tomcat 8.5.24 32bit is the default version packaged in the **Aware IM 8.4 and below** server installation.

#### [**⚠️ Tomcat 10.1.18**](http://tomcat.apache.org/) - **5 January, 2024. Tomcat 10 is designed to run on `Java SE 11 or later`**

- [**Download Tomcat v10**](https://tomcat.apache.org/download-10.cgi)

  - ⚠️ Testing `Aware IM` **`8.8`** produced a "HTTP Status 500 – Internal Server Error" when trying to load the login url (http://localhost:8080/AwareIM/logonAdmin.jsp).
    - According to [Bard](https://bard.google.com/):<br>
      `The stack trace you provided indicates that the server is unable to find the javax.servlet.ServletResponse class. This can happen for a few reasons, but it is most likely because you are using an older version of the javax.servlet JAR file than the one that is required by Tomcat 10.1.13.`
  - [**Security**](https://tomcat.apache.org/security-10.html)

  - [Tomcat 10 Documentation](https://tomcat.apache.org/tomcat-10.1-doc/index.html).
  - [Tomcat 10 Changelog](https://tomcat.apache.org/tomcat-10.1-doc/changelog.html).
  - **Installation**
      <details>

      <summary>Microsoft Windows Based Systems</summary>

    - **IMPORTANT**: Ensure any prior modification of existing _`web.xml`_ and _`server.xml`_ configurations are not overwritten with the new version. There are configuration changes in the latest version of Tomcat relating to those two files.
    - **Installation Steps - Windows**
      - Stop the Aware IM server before updating Tomcat. Do **not** delete your current _C:\AwareIM\Tomcat_ folder.
      - 1. **Extract** the archive and open the folder.
      - 2. Open the extracted **Tomcat** folder.
      - 3. Select all files and folders and press `Crl+c` to copy
      - 4. Open you AwareIM v8.8 installation Tomcat folder **`C:\AwareIM\Tomcat`**
      - 5. Press `Ctrl+v` to paste and replace all files and folders.
      - 6. Rename or delete **ROOT** folder - _This is optional_. You can use this folder to store your own favicon.ico, error pages and other HTML/CSS/JS home page files.
        </details>

#### [**✔️ Tomcat 9.0.85**](http://tomcat.apache.org/) - **5 January, 2024. Tomcat 9 is designed to run on `Java SE 8 or later`**

- [**Download Tomcat v9**](https://tomcat.apache.org/download-90.cgi) - 64bit recommended. Manual Install.

  - Tested and working with `Aware IM` `6.x`, `7.x` & **`8.x`**
  - [**Security**](https://tomcat.apache.org/security-9.html)
      <details>

      <summary>Important fixes</summary>

    - `9.0.83` Request smuggling [CVE-2023-46589](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-46589) - Affects: 9.0.0-M1 to 9.0.82
    - `9.0.81` Request smuggling [CVE-2023-45648](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-45648) - Affects: 9.0.0-M1 to 9.0.80
    - `9.0.81` Denial of Service [CVE-2023-44487](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-44487) - Affects: 9.0.0-M1 to 9.0.80
    - `9.0.81` Information Disclosure [CVE-2023-42795](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-42795) - Affects: 9.0.0-M1 to 9.0.80
    - `9.0.75` Information disclosure [CVE-2023-34981](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-34981) - Affects: 9.0.74
    - `9.0.72` Apache Tomcat information disclosure [CVE-2023-28708](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28708) - Affects: 9.0.0-M1 to 9.0.71
    - `9.0.71` Apache Tomcat denial of service `CVE-2023-24998` - Affects: 9.0.0-M1 to 9.0.70
    - `9.0.54` Denial of Service `CVE-2021-42340` - Affects: 9.0.40 to 9.0.53
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

  - ✔️ [**Oracle OpenJDK `21.0.1`**](https://jdk.java.net/21/) - Production-ready open-source builds of the Java Development Kit
  - Superseded versions:
    - 📉 [Oracle OpenJDK `20`](https://jdk.java.net/20/)
    - 📉 [Oracle OpenJDK `19`](https://jdk.java.net/19/)
    - 📉 [Oracle OpenJDK `17`](https://jdk.java.net/17/)
    - 📉 [Archived Versions](https://jdk.java.net/archive/)

- [**Commercial Java SE Development Kit (JDK)**](https://www.oracle.com/technetwork/java/javase/overview/index.html) - [Important Oracle JDK License Update starting April 16, 2019](https://www.oracle.com/technetwork/java/javase/overview/oracle-jdk-faqs.html)

  - ✔️ [**JDK Version `21.0.1`**](https://www.oracle.com/java/technologies/downloads/) - **Works with Aware IM version `8.8`**. 17 October 2023.
  <!--  - 👍 [JDK Version `20.0.2`](https://www.oracle.com/java/technologies/downloads/) - **Works with Aware IM version `8.8`**. -->
  - 👍 [JDK Version `17.0.9`](https://www.oracle.com/java/technologies/downloads/) - **Works with Aware IM version `8.6 and above`**.
  - ✔️ [JDK Version `8, Update 391`](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html) - **Compatible with Aware IM versions `6.0` - `8.5`**. 17 October 2023.
  - Versions bundled with Aware IM:
    - Aware IM `v8.6 and above` - [JDK `12.0.2` Final](https://docs.oracle.com/en/java/javase/12/) - Archived.
    - Aware IM `v8.0 - 8.5` - JDK 8 Update 91 `1.8.0_91-b15`
  - [**All previous JDK versions archive**](https://www.oracle.com/java/technologies/downloads/archive/)
    - [Manual Downloads](https://java.com/en/download/manual.jsp)

#### Java Servlets

- ✔️ [**Jakarta Mail**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/) - **`1.6.7`** - April 8, 2021 Final Release. (formerly JavaMail)

  - ⚠️ Jakarta Mail 2.0.x - Incompatible with Aware IM `8.8`

  - [**Download jakarta.mail-1.6.7.jar**](https://mvnrepository.com/artifact/com.sun.mail/jakarta.mail/1.6.7)
    - **Installation**
      - In Aware IM **v8.3 and above**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\lib`_
      - In Aware IM **v8.2 and below**, rename _`jakarta.mail-x.x.x.jar`_ to **_`mail.jar`_** and replace the one in _`C:\AwareIM\Tomcat\lib`_
      - Restart Aware IM server
  - 📉 [JavaMail 1.6.2](https://javaee.github.io/javamail/) - August 30, 2018 Final Release. (superseded by JakartaMail)

- [**Apache ActiveMQ™**](http://activemq.apache.org/) - The most popular and powerful open source messaging and Integration Patterns server. Apache [ActiveMQ](https://en.wikipedia.org/wiki/Apache_ActiveMQ) is an open source message broker written in Java together with a full Java Message Service (JMS) client.

  > 📉 ActiveMQ `5.8.0` (06/02/2013) packaged with Aware IM.

  - 📉 Latest version of ActiveMQ that works with out-of-box installation of Aware IM is **`5.12.1`** (13 Oct 2015).

  - **Reported issues in Aware IM** - Scalability, bugs, performance...
    - [Highly demand -- updates - security concerns](https://awareim.com/forum/viewtopic.php?f=1&t=10539&p=48389)
    - [How many Communication driven apps can we host on 1 serv](https://awareim.com/forum/viewtopic.php?f=1&p=51529)
  - [**Issues**](https://github.com/RennurApps/AwareIM-resources/issues) - Refer to the Issues tab.
  - [**Bugs since `5.12.1`**](<https://issues.apache.org/jira/browse/AMQ-9279?jql=project%20%3D%20AMQ%20AND%20status%20in%20(Open%2C%20%22In%20Progress%22%2C%20Reopened)%20AND%20resolution%20%3D%20Unresolved%20AND%20affectedVersion%20in%20(5.12.2%2C%205.12.3%2C%205.13.0%2C%205.13.1%2C%205.13.2%2C%205.13.3%2C%205.13.4%2C%205.13.5%2C%205.14.0%2C%205.14.1%2C%205.14.2%2C%205.14.3%2C%205.14.4%2C%205.14.5%2C%205.15.0%2C%205.15.1%2C%205.15.10%2C%205.15.11%2C%205.15.12%2C%205.15.13%2C%205.15.14%2C%205.15.15%2C%205.15.2%2C%205.15.3%2C%205.15.4%2C%205.15.5%2C%205.15.6%2C%205.15.7%2C%205.15.8%2C%205.15.9%2C%205.16.0%2C%205.16.1%2C%205.16.2%2C%205.16.3%2C%205.16.4%2C%205.16.5%2C%205.16.6%2C%205.17.0%2C%205.17.1%2C%205.17.2%2C%205.17.3%2C%205.17.4%2C%205.17.5%2C%205.18.0%2C%205.18.1%2C%205.18.2)%20ORDER%20BY%20affectedVersion%20DESC%2C%20priority%20DESC%2C%20updated%20DESC>)
  - **Releases**:
    - ⚠️ [6.0.1 Release](https://activemq.apache.org/activemq-6000001-release) - 3 December, 2023. Java 17+ required.
    - ⚠️ [5.18.3 Release](https://activemq.apache.org/activemq-5018003-release) - 25 October, 2023. Java 11+ required.
    - ⚠️ [5.17.6 Release](https://activemq.apache.org/activemq-5017006-release) - 25 October, 2023. Java 11+ required.
    - ⚠️ [5.12.2+ Problem](https://activemq.apache.org/activemq-5016004-release) - **Inconsistent vector internals** Aware IM error.
      - ERROR:
        - `org.openadaptor.adaptor.jms.JMSListener - onMessage: JMSException: [javax.jms.JMSException: Failed to build body from bytes. Reason: java.io.StreamCorruptedException: Inconsistent vector internals [java.io.StreamCorruptedException: Inconsistent vector internals]]`
      - Changelog
        - This release enables ActiveMQ client TLS hostname validation by default which can cause a client connection failure for server certificates that do not match the server hostname. Please refer to SSL Transport Reference for configuration and [AMQ-7047](https://issues.apache.org/jira/browse/AMQ-7047) for more information.
        - Java 8 Required - The minimum Java version has been upgraded to Java 8.
        - This release affects applications using ObjectMessages.
    - ✔️ [**5.12.1 Release**](http://activemq.apache.org/activemq-5121-release.html)
      - Installation
        - In **v8.3 and above**, extract, rename `activemq-all-x.xx.x.jar` to `activemq-all-5.8.0.jar` and replace the one in `C:\AwareIM\lib`
        - In v8.2 and below, extract, rename `activemq-all-x.xx.x.jar` to `activemq-all-5.8.0.jar` and replace the one in `C:\AwareIM\Tomcat\lib`
    - 📉 [**5.8.0 Release**](http://activemq.apache.org/activemq-580-release.html) - Default version packaged with the server installation.

- [**Java Service Wrapper** -](http://wrapper.tanukisoftware.com/doc/english/download.jsp) - **32bit v3.5.54** 64-bit Windows versions of the Java Service Wrapper are not currently being made available in the Community Edition.

  - [**Licensing Overview**](https://wrapper.tanukisoftware.com/doc/english/licenseOverview.html) - Choosing an Appropriate License.

- [**Apache Axis2/Java**](https://axis.apache.org/axis2/java/core/) - Apache Axis2 Web Services JSON / SOAP / WSDL engine.

### Database Servers

- #### **MySQL**

  - [**MySQL Community Server**](http://www.mysql.com/products/community/)
    - [Supported Platforms: MySQL Database](https://www.mysql.com/support/supportedplatforms/database.html)
    - **Download MySQL**
      - ⚠️ [MySQL Community Server 8.2.0 Innovation](http://dev.mysql.com/downloads/mysql/) - [New Release](https://dev.mysql.com/doc/relnotes/mysql/8.2/en/) 26 October 2023.
        - Min Requirement: `Win 11`, `Windows Server 2016`, `macOS 13`, `Oracle Linux 7` / `Red Hat Enterprise Linux 7` / `CentOS 7`
      - ✔️ [**MySQL Community Server 8.0.35**](http://dev.mysql.com/downloads/mysql/)
      - 📉 [MySQL Community Server 5.7.44](https://dev.mysql.com/downloads/mysql/5.7.html)
    - Installation on Windows requires:
      - [**Visual Studio 2015, 2017, 2019, and 2022**](https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170) - Required by MySQL `8.0`, `8.2` and `5.7.38 and above`
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
  - [Download](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) - Version `16.1`

- **Maria DB**

  - [**MariaDB**](https://mariadb.org/) - Free and open-source software under the GNU General Public License.
  - [Download](https://mariadb.org/download/) - Version `11.2.2`.

- [**SQL Server**](https://www.microsoft.com/en-in/sql-server/)

  - [Download](https://www.microsoft.com/en-in/sql-server/sql-server-downloads)

- [**Oracle**](https://www.oracle.com/database/)
  - [Download](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html) - Oracle Database version `21c` (`21.3`)

#### Database Connectors

- [**MySQL Connectors**](https://www.mysql.com/products/connector/)

  - ✔️ [**Connector/J 8.2**](https://dev.mysql.com/downloads/connector/j/) - **Latest version `v8.2.0`**. Requires `Java 8` and `above`. Connector/J 8.1 supports MySQL `5.7`, `8.0`, and `8.1`.
    - [**Download Platform Independent Version**](https://dev.mysql.com/downloads/connector/j/)
    - **Installation**
      - Application Server
        1. Extract the files and rename `mysql-connector-java-8.x.xx-bin.jar` to `mysql-connector-j-8.0.31.jar`
        2. Copy and replace the existing file in
        - **v8.8**, `C:\AwareIM\lib`
        3. Restart AwareIM Server

- 📉 [Connector/J 8.0](https://downloads.mysql.com/archives/c-j/) - **Final version `v8.0.33`**. Archived.

- [**PostgreSQL JDBC Connector**](https://jdbc.postgresql.org/download/) - Current version `42.7.0`. Java 8 required.

#### [**MariaDB Connectors**](https://mariadb.com/kb/en/library/connectors/)

- ✔️ [**MariaDB Connector/J `2.3.0`**](https://mariadb.com/kb/en/about-mariadb-connector-j/) - Out-of-the-box support in Aware IM `v8.3`+. Java `8+`
- :warning: [MariaDB Connector/J `3.3.1`](https://mariadb.com/kb/en/mariadb-connector-j-3-3-1-release-notes/)

### **Web Application Framework**

- [**Kendo UI®**](https://www.telerik.com/kendo-ui) - Kendo UI for jQuery delivers everything you need for data handling, data grids, forms, navigation, performance, UX, design, accessibility, and so much more.
  - [**Roadmap**](https://www.telerik.com/support/whats-new/kendo-ui/roadmap)
  - [**Release History - jQuery**](https://www.telerik.com/support/whats-new/kendo-ui/release-history)
    - Latest Kendo UI Release [**Kendo UI R3 2023 SP1**](<https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2023-sp1-(version-2023-3-1114)>) - November 13, 2023
    - 📉 **Aware IM `8.6 - 8.8`** Kendo UI version [**Kendo UI R3 2020 SP1**](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2020-sp1) - **October 21, 2020**
    - 📉 Aware IM `8.1 - 8.5` Kendo UI version [Kendo UI R3 2017](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-r3-2017) - September 13, 2017
    - 📉 Aware IM `7.0 - 8.0` Kendo UI version [Kendo UI Q1 2016](https://www.telerik.com/support/whats-new/kendo-ui/release-history/kendo-ui-q1-2016) - January 12, 2016
  - [**jQuery Demos & Examples**](https://demos.telerik.com/kendo-ui/) - Kendo UI jQuery Components

#### Front-end open source toolkit

- **Bootstrap** - Frontend toolkit.

  - ❔ [Bootstrap v5.3.2](https://getbootstrap.com/)
  - ❔ [Bootstrap v4.6.2](https://getbootstrap.com/docs/4.6/getting-started/introduction/)
  - ✔️ [**Bootstrap v3**](https://getbootstrap.com/docs/3.4/) - **`3.4.1` (final)**. Bootstrap `3.3.4` bundled with Aware IM v `8.8`.
    - [Download v3.4.1](https://getbootstrap.com/docs/3.4/getting-started/#download)
    - [Bootstrap v3.4 CDN](https://getbootstrap.com/docs/3.4/getting-started/#download-cdn)
  - [All Bootstrap Versions](https://getbootstrap.com/docs/versions/)
  - [List of 300+ bootstrap resources](https://expeditedsecurity.com/the-big-badass-list-of-bootstrap-resources/)
  <!--    - **Plug into Aware IM**
        - Manual configuration through **Startup.html**
        - disable **`legend`** style as it seems to be in conflict with the ExtJS style
          - `/* legend { display: block; width: 100%; padding: 0; margin-bottom: 20px; font-size: 21px; line-height: inherit; color: #333; border: 0; border-bottom: 1px solid #e5e5e5; } */` -->

- [**Font Awesome 5**](https://fontawesome.com/) - Icon library.
  - ❔ Font Awesome `5.15.4 For The Web` - Latest version [Download](https://fontawesome.com/v5/download)
  - ✔️ Aware IM `8.8` bundles [Font Awesome version `5.6.3 Free For Web`](https://fontawesome.com/v5/download).
  - [Front-end Frameworks with comparison](http://bit.ly/RAfrontend) - Collection of best front-end frameworks
  - [Front End Development Bookmarks](http://bit.ly/FrontEndList) - A huge list of frontend development resources collected over time.

### Out-of-the-box Features

- **Integration with Stripe Multi-Payment** - Stripe is a very well-known payment platform and it supports multi-party payments. <!-- [Video](https://youtu.be/4m9YNPrpsvk%22) -->

- **Electronic Signature Capture** - For Aware IM `5.9 - 8.x`
  - [**Signature Pad**](https://github.com/szimek/signature_pad) - Implement and store electronic signatures out-of-the-box with Aware IM. HTML5 canvas based and works in all modern desktop and mobile browsers.
  - [**DEMO - Github**](http://szimek.github.io/signature_pad/)
  - [✔️ **Signature Pad v1.5.3**](https://www.jsdelivr.com/package/npm/signature_pad?version=1.5.3) - Tested and working in all versions `5.9 - 8.x`
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
  - Some alternatives to wkhtmltopdf:
    - [WeasyPrint](https://github.com/Kozea/WeasyPrint) - For Python 3.7+.
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
