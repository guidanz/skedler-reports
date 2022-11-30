# v6.1.0 (2022-11-30)

### Features
	* Added latest version support for Security Onion 2.3.181
	* Added support to latest version elasticsearch 8.5.x and kibana 8.5.x
	* Improved datasource connection verification

### Bug fixes
	* Fixed issue in rendering the datatable chart in kibana 6.8
	* Fixed issue with propagating template changes to reports
	* Fixed issues in applying quick time filter
	* Fixed issue in generating report while the report name contains special characters(:,?,#,\,/,%)
	* Fixed the Skedler server crashing issue while fetching saved search
	* Fixed issue with old table chart

### Minor changes
	* Sandbox - Survey time increased and removed survey for users who already gave feedback
	* Added option to select the tabular report export format (tar/zip)
	* Added validations on saving notification channels

# v6.0.0 (2022-10-31)

### Features
	* Node.js version upgraded into v16.17.1 to fix security vulnerabilities
	* Added support for bucket filter query in tabular report generation
	* Added support for latest version of Grafana 9.2.1
	* Added support for influx 2+ with flux query in the tabular report generation

### Bug fixes
	* Fixed the reporting name issue in the history while generating the report with burst queries

### Minor changes
	* Added option to update reports which are applied by corresponding template
	* Added guide to say the default username and password  in the sign-in page
	* Fixed UI responsiveness issues

# v5.15.0 (2022-09-30)

### Features
	* Added header and timewindow for excel and csv reports
	* Added option for adding tags to organise the reports
	* Added Grid Configuration in templates
	* Added Grafana latest version support
	* Added ELK latest version support
	* Added support for Grafana macros and template variable querying for Mysql
	* Added support to share the templates
	* Added feature to support for provisioning the Datasources, Orgs, Notification Channels

### Bug fixes
	* Handled error case for excel report generation when chart's query has created using Grafana code editor
	* Fixed showing no data issue when applying burst filter in report designer
	* Handled error cases on the Kibana lens chart while generating a report
	* Fixed issues in tabular generation
	* Fixed issue in report generation when already added charts are deleted from Dashboard
	* Fixed line break issue in $TimeWindow parameter while generating the report
	* Fixed the issue in generating landscape PDF report by using ELK datasource

### Minor changes
	* Retained all template elements except charts on switching between dashboards
	* Applied theme only for chart element on changing theme of the report
	* Improved UI experience in changing page settings for smart layout
	* Fixed report edit option finding UI issue

# v5.14.0 (2022-08-30)

### Features
	* Implemented no authentication for Grafana's datasources
	* Provided option to split the dashboard page automatically if it exceeds more than 200 inches
	* Added option for bulk schedule and share reports to users
	* Added latest version support for ELK
	* Added latest version support for Grafana

### Bug fixes
	* Disabling sending emails from Skelder for the on-premise application
	* Fixed issues in uploading CMYK type of JPG file
	* Fixed issue while connecting ELK in the report for the first time
	* Fixed issue in excel report extension name while downloading the report through download icon 
	* Fixed issue in applying burst filter in tabular designer
	* Fixed issue in migrating data table and saved search reports

### Minor changes
	* Added search option to template module
	* Added option to replace an image with a newly uploaded image in the report designer
	* Designer Enhancement - Background color for Texts
	* Designer enhancement - Formatting option for the Date Time field

# v5.13.0 (2022-07-29)

### Features
	* Redesigned the template page

### Bug fixes
	* Fixed security issues in listing datasources
	* Fixed the issue in connecting ELK which has no spaces
	* Fixed issues in Postgres excel report generation
	* Fixed dashboard timeout errors
	* Fixed the memory leak issue while reporting generation

### Minor changes
	* Added product expire notification bar with quick navigation

# v5.12.0 (2022-06-28)

### Features
	* Added latest version support for grafana
	* Added latest version support for grafana
	* Implemented Grid lyout chart rendering in designer
	* Implemented global styles for the text, shape and chart elements for the report
	* Added support for Grafana latest version 9.0.0
	* Added Support for kibana latest version 8.2.3

### Bug fixes
	* Fixed the issue in updating the time window in tabular reporting
	* Fixed issues in sharing reports with a group of users
	* Fixed the issue in applying themes

### Minor changes
	* Implemented RBAC in UI routing
	* Changed product logo as per skedler brand
	* Improved get all templates API
	* Removed unused icons and actions in product ui
	* Fixed issues in creating and authenticating ldap users
	* Fixed filter & paramater UI issues

# v5.11.0 (2022-05-25)

### Features
	* Added SSL support to Skedler
	* LDAP integration with Skedler
	* Added default template for dashboard layout
	* Added no template option for dashboard layout
	* Revamped report designer for better usability

### Bug fixes
	* Move elements based on the text element's height in the group element
	* Fixed issues in report generation when the banner is enabled in Kibana
	* Fixed issues in dragging and dropping the templates on the page

### Minor changes
	* Added an option to provide SOS user credentials while adding datasource
	* Added option to search dashboards by Grafana folder

# v5.10.0 (2022-04-14)

### Features
	* Added support for Grafana 8.4.4
	* Added support for elasticsearch and kibana 8.1.0
	* Added feature to snap elements while resizing and dragging the element in designer
	* Improved user experience in the designer
	* Support For Security Onion System v2.3.110

### Bug fixes
	* Fixed issue in stopping redis after completion of migration
	* Fixed chart rendering issue when it has large dataset in kibana
	* Fixed use dashboard timewindow issue in report designer

### Minor changes
	* Displayed element's dimension while resizing the element
	* Moved element styling to the design toolbar
	* Added option to select folder in selecting Grafana datasource in the report designer

# v5.9.0 (2022-03-18)

### Features
	* Elasticsearch kibana 8.0 support
	* Added auto suggestion option for mail notification in distribution.
	* Added support for Grafana 8.4.3
	* Support For Security Onion 2.3.100
	* Added Support for Undo & Redo in report designer

### Bug fixes
	* Fixed incorrect messege in dialog box while removing user issue

### Minor changes
	* Added option to show visualisation name on hovering the chart element in the report designer
	* Fixed user experience issue in editing a report
	* Added guideline to create report in report designer
	* Improved user experience in timewindow selection.

# v5.8.0 (2022-02-18)

### Features
	* Support for latest version of ELK (7.16.3) and Grafana (8.3.4) given
	* Added Option to change the date time format
	* Redesign grafana datasource layout
	* Redesign kibana datasource layout

### Bug fixes
	* Fixed issue in excel report generation for specified chart generation
	* Fixed issue in rendering stat charts in Grafana
	* Fixed autoscaling issue in Grafana
	* Fixed minor issue in puppeteer url loading
	* Fixed the overlapping issue in Grfana chart's legend

### Minor changes
	* Fixed the user experience issue on selecting the dashboard time window for the report 

# v5.7.0 (2022-01-21)

### Features
	* Added support for png inline
	* Added support for ELK where spaces is not available

### Bug fixes
	* Fixed license deactivation issue on offline environment
	* Fixed charts not loading when user switch Dashboard layout into custom layout
	* Issue while generating report with custom time filter using invalid time
	* Fixed the help button disabled issue after closing Skedler tour pop-up tab
	* Fixed help and documentation option disabled issue in sign in page
	* Fixed issue with report generation count does not updated properly when license activated.
	* Fixed selecting any type of files for upload image option issue in designer modal
	* Fixed generating report without datasource issue
	* Handle Error messages properly in connecting Databases in grafana
	* Fixed issue in searching users in history module
	* Fixed issue in adding kibana no authentication datasource with ssl
	* Auto filled default password when user navigates from Create account page
	* Unchecking include recipients in distribution is not working

### Minor changes
	* Adding Grafana data source without authentication removed.
	* Product Tour added for Left Menu

# v5.6.0 (2021-12-23)

### Features
	* Added an option to choose holiday per week for schedule
	* Added autoscaling support for charts in Kibana
	* An option to configure the proxy url added
	* Added support for saved search more than 10000 rows
	* Added Grafana excel support for Postgres timescaledb.

### Bug fixes
	* Fixed the security onion report generation inconsistency issue
	* Fixed the chart rendering issue with dashboard layout in Grafana
	* Fixed issue while generating tabular report for data table
	* Fixed the license activation issue
	* Fixed applying color fill issue for line and arrow element
	* Fixed issue in connecting with secured elasticsearch as datastore for migration
	* Fixed the issue with Report counts not updated if reports are generated as per schedule
	* Verified Grafana URL is whether valid or not while saving data source
	* Displayed current org's users only in the admin settings
	* Fixed duplication issue while copying and pasting the elements
	* Fixed formatting issues in Frames element
	* Fixed - Report not generated for opendistro if multitenancy is disabled
	* Fixed issues in uploading burst filter as excel/json
	* Fixed issue while using colon(:) in burst filters
	* Fixed selecting any type of files for upload image option issue in report designer
	* Fixed issue on applying burst filter's custom param in the report template

### Minor changes
	* Changed license trail version from 30 days to 15 days
	* Spelling mistakes in log file corrected
	* Time format mismatch in Hourly report fixed

# v5.5.0 (2021-11-26)

### Features
	* Added an auto-scaling support for Grafana dashboard layout reports
	* Added a privilege to super admin users to change their email id
	* Generate reports using Grafana dashboard timezone if "use dashboard time" is selected
	* Provided support for using fiscal year time window in Grafana dashboards.
	* Support added to use MySQL version 8 as datastore 
	* Support added for ELK 7.15.2 and Grafana 8.2.4
	* Added support for Outlook SMTP 

### Bug fixes
	* Fixed deleting filter which is already applied to reports issue
	* Fixed the error while generating report with absolute time filter
	* Fixed quick time window always in Last 15 Minutes issue
	* Fixed the report rendering issue when table don't have header
	* Fixed AWS OpenSearch connectivity issue
	* Fixed font parsing error while report generation
	* Fixed the issue with report re-scheduling when restarting the server
	* Handled error case for unsupported datasource versions while generating report
	* Fixed the number of queries issue in filter listing
	* Fixed undefined issue in adding ${Filtername} param in distribution
	* Fixed report generation failure when a report has error charts
	* Fixed the duplicate chart issue
	* Fixed the issue in sending warning slack message
	* Fixed the AWS OpenSearch connection issue without authentication
	* Fixed migration issue for monthly and yearly scheduled report
	* Fixed the table column header missing issue with Kibana reports

### Minor changes
	* Improve logs in report distribution
	* Added zero to first ten number in dropdown while scheduling
	* Moved download logs functionality from setting to help icon.
	* Added the ability to preview the report based on filter query

# v5.4.14 (2021-11-24)

### Features
	* Added support for Outlook SMTP

### Bug fixes
	* Fixed the table column header missing issue with Kibana reports

# v5.4.13 (2021-11-22)

### Bug fixes
	* Fixed the AWS OpenSearch connection issue without authentication

# v5.4.12 (2021-11-19)

### Features
	* Support added to use MySQL version 8 as datastore

### Minor changes
	* Added the ability to preview the report based on filter query
	* Changed the rendering approach for Kibana

# v5.4.11 (2021-11-12)

### Features
	* Provided support for using fiscal year time window in Grafana dashboards.

# v5.4.10 (2021-11-11)

### Features
	* Added a support to change the email address for super admin users
	* Generate reports using Grafana dashboard timezone if \"use dashboard time\" is selected

### Bug fixes
	* Fixed the connection issue with AWS Managed Grafana

# v5.4.9 (2021-11-10)

### Bug fixes
	* Fixed the report rendering issue when table don't have header
	* Fixed AWS Opensearch connection issue

# v5.4.8 (2021-11-09)

### Bug fixes
	* Fixed the issue with sending report via mail

# v5.4.7 (2021-11-08)

### Features
	* Added an auto-scaling support for Grafana dashboard layout reports

# v5.4.6 (2021-10-29)

### Features
	* Added an option to skip SSL verification 
	* Support For Security Onion version 2.3.80

### Bug fixes
	* Fixed unable to resize the header issue in the dashboard layout
	* Fixed incorrect error message in while previewing report if license is not activated
	* Fixed incorrect error message in while report generation if license is not activated
	* Fixed the script issue while starting skedler in windows
	* Fixed - Data Mismatch in the generated Report due to incorrect Org Id
	* Fixed issue in displaying proper message for GRF0400
	* Fixed issue in displaying proper message for PUP0500
	* Fixed data set name gets cut off at 25 character
	* Fixed prolonged report generation after migration from skedler v4 to v5
	* Fixed issue while downloading reports with certain Grafana filters
	* Fixed the connection issue with AWS Managed Grafana

### Minor changes
	* Disabled skedler welcome email at account creation

# v5.4.5 (2021-10-14)

### Features
	* Added support to customize the dashboard layout report
	* Added support for Grafana 8.2.1
	* Added support for ELK v7.15

### Bug fixes
	* Fixed the user uploaded image streching issue
	* Improved the log messages severity
	* Unable to verify Kibana SSL certificate - Fixed
	* Fixed duplication of text element and drag and drop issue in Firefox
	* Fixed text/element transformation issue on resizing the element
	* Fixed the SSL options disabled issue while creating datasources
	* Fixed the uploaded SVG image spacing issue
	* Fixed page duplication issue in report
	* Fixed - Issue In Excel Reports Generation For Tabular Report
	* Fixed minor issue in log message
	* Fixed template issues in smart layout
	* Fixed not able to add any elements issue in the landscape report
	* Fixed the report generation issue when used images missing
	* Fixed the issue with pre-populating the selected data source in designer
	* Fixed the font is not applying issue with preview 

### Minor changes
	* Added a dropdown option with skedler version in help menu

# v5.4.4 (2021-10-01)

### Features
	* Added features to change text's font size, alignment and inline styles(B, I, U)
	* Support For Security Onion 2 

### Bug fixes
	* Fixed issue in updating timezone globally in site settings
	* Fixed duplicating charts issue in the available charts palette that allows user to add duplicating charts in the report
	* Handled proper error cases for report preview
	* Fixed text overflow issue when resizing the text area field
	* Fixed adding empty newline issue when resizing subheader field
	* Fixed report generation issue while using custom time filter
	* Fixed rendering inconsistency issue with grafana table
	* Fixed visualization undefined issue with ELK 7.14
	* Fixed text wrapping issue when resizing the text area
	* Fixed scheduled report stopping bug when user restarts the machine.
	* Fixed the visualization collapsing issue when resizing grafana charts
	* Fixed data mismatch with generated report and dashboard data while using time filter
	* Fixed the excel generation issue for specific dashboard
	* Fixed the text spacing issue with dashboard layout
	* Fixed login issue when user enters credentials with password manager
	* Fixed issue when using browser access option in Prometheus while configuring in Grafana
	* Fixed resizing elements issue

### Minor changes
	* Improved the error message, when grafana chart has an error while generating report 
	* Added a search support for charts in designer
	* Added the ability to download the report based on filter query
	* Added a new option for authentication type in kibana form

# v5.4.3 (2021-09-17)

### Bug fixes
	* Fixed Grafana and Kibana https login error
	* Fixed template preview generating for all templates issue when update happens on a single template
	* Added the proper error message when report generation fails, due to dashboard error
	* Fixed the license activation issue, when user submits the key with trailing white spaces
	* Fixed cannot able to retrieve template when applying same template to itself issue
	* Fixed the grafana charts resizing adoption issue
	* Fixed Grafana and Kibana Https login error

### Minor changes
	* Improved the logs details
	* Added skedler documentation link in the app header

# v5.4.2 (2021-09-07)

### Features
	* Added the Folder name option to store the reports with burst filter
	* Added auto scaling support for visualizations in Grafana 7 & above
	* Added support for ELK 7.14

### Bug fixes
	* Fixed issue in report generation when using dashboard time for grafana 7+
	* Fixed migrated report alignment issues
	* Fixed report generation issue when fresh grafana instance configured as datasource
	* Fixed the moment timezone browser issue with Grafana 6
	* Fixed charts collapsing issue while generating report as PNG with dashboard layout
	* Fixed the row title issue
	* Fixed timerange mismatch in charts in generated report

### Minor changes
	* Added support for Grafana 8.1.x
	* Redesigned the role base user authentication in skedler

# v5.4.1 (2021-08-17)

### Features
	* Added the support to render the custom parameter in report

### Bug fixes
	* "Fixed Grafana version undefined error for v7.5.4"
	* Fixed the issue with see filters action, which is forcing user to login again
	* Fixed template variable filter query issue for grafana reports
	* Fixed Error message is not displayed in the UI & generating loader keep on loading if the user generates the report when the elk or grafana datasource not running
	* Fixed the theme based rendering issue in ELK reports
	* Fixed chart duplication in saved search and Data table
	* Fixed logo alignment and report title parameter for report and template design in migration
	* Fixed incorrect time window issue on report
	* Fixed issue in report with burst filter
	* Fixed link issue in mail distribution
	* Fixed download type overriding issue when user add distribution
	* Filter query name for elk report fixed
	* Data mismatch when filter applied for the elk report

### Minor changes
	* Added the query name in report history listing
	* Added the ability to display the unsupported charts in report

# v5.4.0 (2021-08-02)

### Features
	* Added support to preview the template

### Bug fixes
	* Fixed email validation issue
	* Fixed Heading in the chart disappears after ungrouping it and applying template
	* Fixed Safari browser compatibility issue in skedler app
	* Fixed windows browser compatibility issue in skedler app
	* Fixed profile image update issue
	* Fixed prolonged loading of template preview in templates dashboard
	* Restructuring logger and log messages.
	* Fixed page navigation and number of rows to show per page filter in history 
	* Fixed chart alignment issue when resizing in desinger
	* Fixed report count increasing issue when report generation failed
	* Fixed distribution details reset issue 

### Minor changes
	* Added the ability to run the skedler with debug mode
	* Changed label in absolute time filter
	* Added the ability to prevent deleting the datasource assinged to a report
	* Change of label in Datasource delete warning modal
	* Minor fix in profile user name

# v5.3.0 (2021-07-19)

### Features
	* Added the support to delete assets
	* Added library checking script in deb & rpm
	* Added the support to delete the images in designer
	* Added support for Grafana 8 new charts
	* Added feature to download log files.

### Bug fixes
	* Fixed cancel button issue in both admin and account settings
	* "Removed download action in template designer"
	* Fixed changing roles from same organization of the current user in admin settings
	* Fixed generated report count mismatch issue
	* Fixed the issue with site settings logo

# v5.2.0 (2021-07-05)

### Features
	* Added the Ngnix proxy support

### Bug fixes
	* Fixed drag-and-drop alignment issue in designer

### Minor changes
	* Minor changes in script and service file in migration.

# v5.1.2 (2021-06-25)

### Features
	* Migration of data from Skedler 4.0 to Skedler 5.0
	* Added support for Grafana 8.0 and ELK 7.13

### Bug fixes
	* Support For Old Table in Grafana
	* Fixed the image uploading issue in designer
	* Fixed the chart not adding issue in designer
	* Fixed the chart adding outside of design page issue
	* Fixed chart duplicate issue in designer
	* Fixed the apply template conflicting issue in designer
	* Fixed the template thumbnail rendering issue
	* Database name change issue in new version of Skedler - fixed
	* Data table and saved search report generation issue fixed.
	* db renaming issue fixed;
	* History timewindow format issue fixed.
	* Kibana connectivitity check with wrong credentials issue fixed.
	* History module timewindow bug fixed.

### Minor changes
	* Tenant db name and accounts db name made configurable for MySQL datastore in reporting.yml file.
	* Migration folder structure changed
	* Added support for migrating Skedler 4.0 data from Mysql and ELK.
	* History query modified;timezone fetching issue in history fixed.

# v5.1.1 (2021-06-10)

### Bug fixes
	* Added support for old table in grafana

### Minor changes
	* Added ability to configure the accounts and tenants db for MySQL datastore

# v5.1.0 (2021-06-04)

### Features
	* Support for grafana stat panels.
	* Support for sending mail to admin for error reports in Grafana.

### Bug fixes
	* Fixed the pasue/resume status update issue in report listing
	* Resolved the license alert issue for Super admin
	* Fixed the bug in creating schedule for monthly and yearly when the day was given as 1
	* Fixed table pagination and schedule recurrence type issue
	* Added the ability to unselect the Excel / CSV export options
	* Custom url building functionality removed for dashboard layout reports in kibana; 
	* Fixed Grafana API key permission issue, Added org name in getDashboardsAndSearches API for Grafana.
	* Support to create SMTP Email Server without password
	* Notification service type name modified from 'others' to 'Others'.
	* Fixed reports generated with no data when generated with use dashboard time for kibana
	* Changed account creation logic from checkAccountExits API to server.ts
	* Fixed permission denied issue for non-admin users authenticating via username and password in grafana.
	* styles added to hide grafana page-toolbar while rendring, report listing sorted based on creation, unnecessary comments removed
	* Support for grafana piechart-v2
	* Fixed the issue while user creation.
	* Support for sending admin and warning mails for error and no data reports in Kibana.

### Minor changes
	* Sorting order changed to createdAt basis instead of last run value;
	* Changed the chart color code for custom and smart layout

# v5.0.0 (2021-05-21)

### Features
	* Released a stable Skedler Reports version 5

