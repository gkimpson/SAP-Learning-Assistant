> Source: https://learning.sap.com/courses/exploring-the-authorization-concept-for-sap-fiori-on-sap-s-4hana/explaining-sap-fiori-authorization-model

Explaining SAP Fiori Authorization Model 
Learning
Browse By product
SAP S/4HANA Cloud Public Edition
SAP S/4HANA Cloud Private Edition
SAP Business Technology Platform
Supply chain management
Financial management
Human capital management
Spend management
Customer experience
Transformation management
View all products By role
Administrator
Architect
Business user
Consultant
Data analyst
Data scientist
Developer
View all roles By industry
Agribusiness
Automotive
Consumer products
Life sciences
Public sector
Professional services
Retail
Utilities
View all industries By learning type
Learning journeys
Courses
Videos
Live sessions
Hands-on practice
Instructor-led training opens in a new tab
Reference architectures opens in a new tab Exclusive content
For partners
For students
For Enterprise Support Featured
Autonomous Enterprise
SAP Business Data Cloud
Artificial Intelligence
Get certified SAP Certification
Browse certifications
Get and stay certified
Manage your certification
My Learning My profile ">
My activity
My certifications
My subscription
My instructor-led training Exclusive content
For partners
For students
For Enterprise Support
Subscribe
Explore SAP
Explore all areas of SAP
Products ">
Autonomous Enterprise
Artificial intelligence
Data and analytics
Autonomous Suite
Technology platform
Transformation management
Midsize business solutions
Financial management
Spend management
Supply chain management
Human capital management
Customer experience
Enterprise resource planning
Business network
Sustainability management
SAP Store
Try SAP
View all industries
Partners
Services
Learning and support
Learning and certification
Support
Documentation
Community
About
Company information
Careers
Customer stories
Ethics and compliance
Events
Investor Relations
News center
SAP Trust Center
Browse ">
Get certified ">
My Learning ">
Subscribe
Explore SAP ">
/
Browse /
Courses /
Exploring the Authorization Concept for SAP Fiori on SAP S/4HANA /
Explaining SAP Fiori Authorization Model
Understanding the SAP Fiori Concept
Outlining the SAP Fiori Concept 20 min
Understanding SAP Fiori Application Types 40 min
Understanding SAP Fiori Architecture with SAP S/4HANA 20 min
Quiz
Describing SAP Fiori Authorization
Explaining SAP Fiori Authorization Model 40 min
Quiz
Managing SAP Fiori Authorizations
Creating SAP Fiori Business Catalogs 35 min
Creating Business Roles for SAP Fiori Content 50 min
Creating SAP Fiori Spaces and Pages 1 hr 10 min
Checking and Adjusting Launchpad Content 35 min
Appendix: Creating Roles for SAP Fiori Front-End Server Standalone Scenario 20 min
Quiz
Implementing SAP Fiori Applications
Using Additional Features for Role Maintenance 20 min
Understanding Rapid Activation 10 min
Quiz
Maintaining Special Authorizations for SAP Fiori Launchpad
Understanding SAPUI5 Runtime Adaptation 10 min
Restricting the Enterprise Search 20 min
Quiz
Understanding Authorization concept for ABAP Core Data Services (CDS)
Describing the Authorization Concept for ABAP CDS 40 min
Quiz
Analyzing Authorizations in SAP Fiori Applications
Analyzing SAP Fiori Applications in Roles 20 min
Analyzing Missing Authorizations 20 min
Analyzing CDS View Results in the Authorization Trace 25 min
Quiz
Understanding Options for Transporting Authorizations
Describing Transport Authorization Components 10 min
Quiz
Describing Integration Scenarios
Understanding SAP Fiori Launchpad Deployment Options 10 min
Understanding Central SAP Fiori Launchpad 20 min
Quiz
Appendix: Defining Authorizations in SAP S/4HANA Projects
Listing Authorizations for SAP S/4HANA Project Users 10 min
Quiz
Understanding the SAP Fiori Concept
Outlining the SAP Fiori Concept 20 min
Understanding SAP Fiori Application Types 40 min
Understanding SAP Fiori Architecture with SAP S/4HANA 20 min
Quiz
Describing SAP Fiori Authorization
Explaining SAP Fiori Authorization Model 40 min
Quiz
Managing SAP Fiori Authorizations
Creating SAP Fiori Business Catalogs 35 min
Creating Business Roles for SAP Fiori Content 50 min
Creating SAP Fiori Spaces and Pages 1 hr 10 min
Checking and Adjusting Launchpad Content 35 min
Appendix: Creating Roles for SAP Fiori Front-End Server Standalone Scenario 20 min
Quiz
Implementing SAP Fiori Applications
Using Additional Features for Role Maintenance 20 min
Understanding Rapid Activation 10 min
Quiz
Maintaining Special Authorizations for SAP Fiori Launchpad
Understanding SAPUI5 Runtime Adaptation 10 min
Restricting the Enterprise Search 20 min
Quiz
Understanding Authorization concept for ABAP Core Data Services (CDS)
Describing the Authorization Concept for ABAP CDS 40 min
Quiz
Analyzing Authorizations in SAP Fiori Applications
Analyzing SAP Fiori Applications in Roles 20 min
Analyzing Missing Authorizations 20 min
Analyzing CDS View Results in the Authorization Trace 25 min
Quiz
Understanding Options for Transporting Authorizations
Describing Transport Authorization Components 10 min
Quiz
Describing Integration Scenarios
Understanding SAP Fiori Launchpad Deployment Options 10 min
Understanding Central SAP Fiori Launchpad 20 min
Quiz
Appendix: Defining Authorizations in SAP S/4HANA Projects
Listing Authorizations for SAP S/4HANA Project Users 10 min
Quiz
Explaining SAP Fiori Authorization Model
Objective
After completing this lesson, you will be able to understand the Classical and SAP Fiori Authorization Models.
Classical Authorization Model
Typical SAP GUI transactions are called using the role menu. On the back-end server, the ABAP program behind the transaction code is defined in transaction SE93.
After you have added the transaction code to the role menu in the PFCG role, the role will contain the start authorization and data access authorization.
SAP Fiori Content Model
SAP Fiori App
Technically, apps are represented by the following:
KPI tiles to launch the app.
App launcher tiles to launch the app.
Target mappings referencing the actual navigation targets. 
Tiles and Target Mapping
Tiles represent the visual part of a tile such as a title, subtitle, information, icon and the semantic object and action for the intent-based navigation.
Target mappings define the target application which is launched when an intent (semantic object/action) is triggered.
Target mapping is part of the SAP Fiori launchpad configuration. It defines the target application, which is launched when clicking on a tile, on a link, or within an app-to-app navigation. 
SAP Fiori Content Model - SAP S/4HANA
The apps that are displayed to the users are organized using the following SAP Fiori launchpad content:
Catalog
A catalog is a set of apps that you want to make available for your users to authorize them to work with the apps. The users can browse through the catalog, choose apps from the catalog, and add them to the home page of their SAP Fiori launchpad.
SAP delivers technical catalogs which contain apps per application area. In addition, SAP delivers business catalogs as sample collection of apps relevant for a business role. You can also create you own custom business catalogs. You can use the SAP Fiori launchpad content manager or the SAP Fiori launchpad designer.
Technical catalogs (TC) provide tiles and target mappings cut by solution area, but not by technology. In technical catalog, legacy apps as well as SAPUI5 Fiori apps are available.
Business catalogs (BC) reference tiles and target mappings of technical catalogs (TC) according to segregation of duty. A business catalog can reference tiles and target mappings from one or several technical catalogs.
Group
The SAP Fiori launchpad home page is the central part of the launchpad, which structures the SAP Fiori launchpad content. Here, users access all applications relevant to their business case. The apps can be SAP Fiori app or classic applications. Business catalog groups (BCG) define the SAP Fiori launchpad home page. The apps in the group are a subset of apps that are referenced from one or several catalogs. The tiles which are displayed on a user's home page are dependent on the catalogs and groups that are assigned to the user's roles. If a group contains apps that are not assigned to the user via catalogs, the app is not displayed on the user's home page. In addition, if configured, the user can personalize the home page by adding or removing apps to predelivered groups or self-defined group.
SAP also delivers business catalog groups as sample collection of apps relevant for a business role. You can also create your own custom groups. You can maintain these entities using the SAP Fiori launchpad designer.
From SAP S/4HANA 2021, groups mode is officially deprecated, meaning that while groups currently still exist, they will be removed in a future release.
For details on migrating from groups to spaces and pages see SAP Note 3322675 - Guidelines on Migrating from Groups to Spaces and Pages
Space and Pages
Spaces and pages represent an alternative option to structure the layout of the home page of SAP Fiori launchpad compared to the group-based home page. A space is the unit that holds one or more pages. It is assigned to the user based on the work profile (user role). Users may see several spaces on their launchpad home page. The spaces are displayed in the navigation bar and if more than one page is available, a drop down appears under the corresponding space and the user can navigate to a given page. If there is only one page in a space, when clicking on the space, user gets directly to that page.
Spaces and pages are maintained in the Manage Launchpad Spaces Fiori app and the Manage Launchpad Pages Fiori app.
PFCG Roles
Business roles (BR) combine multiple business catalogs (BC) and business catalog groups (BCG) and/or Spaces.
By adding the catalogs to the role menu, the user gets access to the apps included in the catalog. By adding spaces or groups, you define the SAP Fiori launchpad home page.
In the following, you will find an overview of naming conventions and short definitions.
| Element | Short | Naming Schema | Description |
| --- | --- | --- | --- |
| Business Role | BR | Z_BR_ | Role for topic |
| Space | SP | Z_SP_ | Tiles based on the work profile |
| Page |  | Z_PG_ | Tiles based duties in work profile |
| Business Catalog Group | BCG | Z_BCG_ | Describe contents of group |
| Business Catalog | BC | Z_BC_ | Tiles for duty |
| Technical Catalog | TC | Z_TC_ | Tiles for area |
Business catalogs (BC) reference tiles and target mappings of technical catalogs (TC) according to segregation of duty. Business catalog groups (BCG) now contain apps from various business catalogs (BC), making a subtopic. Business roles (BR) replace business catalog roles (BCR), combining multiple business catalogs (BC) and business catalog groups (BCG) in one topic.
In this example from the SAP Fiori app reference library, you see content model elements under Technical Configuration, starting with TC and continuing with BC, BCG, and BR. BC and BCR have the name of the topic in common, whereas the BR contains the end user role name. 
SAP Fiori Authorization Model
SAP Fiori apps adopt the user management and authorization concepts provided by ABAP Platform (Application Server ABAP).
The security recommendations and guidelines for user and role administration and authorization as described in the SAP NetWeaver ABAP Platform Security Guide also apply for the SAP Fiori apps.
To use SAP Fiori apps, users need app-specific SAP Fiori user interface (UI) entities and authorizations. You use PFCG roles to assign these types of entities to users.
SAP Fiori launchpad is the access point to apps on mobile or desktop devices. To use SAP Fiori apps, users need the following app-specific types of entities:
UI: The SAP Fiori UI entities that define which SAP Fiori apps are displayed to the user. The apps are organized through catalogs and spaces and pages.
Authorizations: The authorizations that are required to use SAP Fiori launchpad, to start SAP Fiori apps, and to use the business logic and data of the apps.
To see the tile, launch the SAP Fiori app, and get business data from the OData service, a specific OData authorization is necessary. This is provided through a PFCG role that contains a catalog and a space.
Note
Please be aware, that the standard scenario in this training is the embedded front-end server (FES) deployment option. In this scenario, only one PFCG role is required in the SAP S/4HANA system as back-end server.
For the stand-alone FES deployment option, a PFCG front-end server and a back-end server roles are necessary. PFCG front-end server role with the catalog and group needs the OData start authorization to call the back-end server (BES). The PFCG back-end server role contains the execute and access authorization of the OData service.
However, this is not subject of this training.
PFCG Roles
You use PFCG roles to assign the UI entities and authorizations to the users:
PFCG roles
To get the authorizations for Fiori Apps, you add the OData services to the PFCG role menu. By adding the catalogs to the role menu, you include the apps in the catalog that is available to the users. The system determines the OData services for a catalog and automatically includes the authorizations.
Hint
If available, we recommend adding the catalog to the role menu to automatically determine the OData services that are included in the catalog. With that, you can organize the update of authorizations when the catalog changes.
The OData services that the SAP Fiori apps use are implemented in the SAP S/4HANA system. The users need to have start authorizations for the OData services' data provider and start authorizations for the model provider of the activated OData services (embedded FES functionality). Also, users needs all the business authorizations for accessing the business data that is displayed in the app.
For object pages, the authorization defaults also include the authorizations for the SAP Fiori search connectors. The OData services carry the authorization defaults for the business authorizations as suggested by SAP. This adds the start authorizations and the authorization defaults for the business authorizations of the applications to the role.
In case of legacy apps, you can add the transaction code or the WebDynpro application to the PFCG role menu. This adds the start authorizations and the authorization defaults for the business authorizations of the applications to the role. However, legacy apps are also included in the Fiori catalog, so it is more efficient to add a catalog to the role menu. The system automatically determines the authorizations objects to be checked.
By adding spaces to the role menu, you define the SAP Fiori launchpad home page.
Sequence When Starting an SAP Fiori App
When the user starts the SAP Fiori launchpad, the launchpad displays the app tiles that are assigned to users via catalogs and organized in spaces and pages. A launchpad-specific OData service resolves the catalogs and spaces a user is assigned to: This service resolves the user's catalog and space assignments using the PFCG roles the user belongs to on front-end server (FES), by collecting the corresponding catalog and space entries in the PFCG role menu.
To start an SAP Fiori app, the user chooses a tile. The tile resolves the technical SAP Fiori app implementation to be started using a target mapping.
When a user's browser loads an SAP Fiori app, the app retrieves its dynamic data from the HTTP endpoint of the app-specific OData service on the FES. SAP Gateway translates the HTTP request to a trusted RFC call to the SAP Gateway enablement of the BES, which then retrieves the data by calling the relevant business logic. The user requires authorizations for the app-specific OData service, that is, the start authorizations for the service and the business authorizations required by the business logic. In the case of legacy apps, where the tile with its target mapping points to a SAP GUI transaction or a WebDynpro application, the SAP Fiori launchpad calls the application in the back-end server system directly without using an OData service.
Authorization Proposals for OData Services
When adding a catalog to a PFCG role, the start authorizations for the implemented and activated OData services for the catalog are included in the role menu as sub-nodes below the catalog entry.
The behavior of the role maintenance ( PFCG) and the authorization checks that are to be performed are defined by authorization proposals which can be maintained in transaction SU24 ( Maintain Authorization Default Values). Among other application types, SU24 defines the authorization proposal values for transactions, WebDynpro applications, and OData Services. 
When you add a catalog to a PFCG role, make sure to choose the Include Applications check box. The start authorizations for the activated OData services and start authorizations for the OData service data providers are then included in the role menu as sub-nodes below the catalog entry. In addition, the authorization defaults delivered by SAP for these services and applications are added to the role.
In both, SU24 and PFCG, you will find the object types of the activated OData services and OData services data providers since they are TADIR objects. Activated OData services have the object type IWSG – Gateway: Service Groups Metadata. The implemented OData services as data providers have the type SAP Gateway Business Suite Enablement - Service. In a system with the embedded FES, both object types will appear in a single PFCG role.
Authorization Values in Role Maintenance
Authorization default values for non-transactional services are stored using a hash code-based key entry. You can see the hash code, for example, as a technical name in the SU24 when displaying the authorization defaults. 
On the Authorizations tab of the role maintenance the hash code-based key entry is shown too. The original application name can be shown by displaying the Define Values window. 
The connection between the hash code-based key entry and the original application name is saved in the table USOBHASH. The content of this table is the basis for the input help and existence validation of these applications. 
Practice System Exercise: Check Authorization Proposals for OData Services
Select Start Exercise to start the simulation.
Exercise Start Exercise
Note
If you have access to a practice system, you can now execute this exercise.
Business Example
You want to find out which OData services the user requires PFCG authorization for by using the SAP Fiori Apps Reference Library. You also want to check the authorization proposals of an OData service in the back-end SAP S/4HANA system.
Steps
In Google Chrome, open the SAP Fiori Reference Library.
In the Microsoft Windows start menu, choose Google Chrome.
In Google Chrome, go to Bookmarks.
In Bookmarks, choose SAP Fiori → SAP Fiori Apps Reference Library.
Search for the app Display G/L Account Balances and check for which OData service the user will require PFCG authorization.
In the SAP Fiori Apps Reference Library, choose SAP Fiori Apps for SAP S/4HANA.
Choose All Apps.
In the Search field, enter Display G/L Account Balances.
Choose Display G/L Account Balances (New).
Below the subtitle, select the release version SAP S/4HANA 2023 latest FPS.
Select the IMPLEMENTATION INFORMATION tab.
Expand Configuration.
Check for which OData service the user requires the PFCG authorization .
Result
The user requires PFCG authorization for the UI_GLACCOUNT_BALANCES OData service.
Task 1: Check the OData Service Activation
You want to make sure that OData service UI_GLACCOUNT_BALANCES of the Display G/L Account Balances app has been activated.
Steps
Log on to the SAP GUI of the system S4D.
| Field | Value |
| --- | --- |
| User | train-## |
| Password | Custom password |
```
1. Choose *SAP Logon*.
2. Select *10 Development* → *S4D SAP GUI non-SNC [PAS]*.
3. Choose *Log On*.
```
In transaction IWFND/MAINT_SERVICE, check if the OData service ZUI_GLACCOUNT_BALANCES has been activated in the SAP S/4HANA back-end system S4D.
Start the transaction IWFND/MAINT_SERVICE. In the OK field of SAP GUI, enter /n/iwfnd/maint_service.
On the Activate and Maintain Services, choose Find.
In the search term field, enter UI_GLACCOUNT_BALANCES and choose OK.
Close the Find dialog box.
Result
The OData service could be found, which means the service has been activated. In the Technical Service Name column, you will see the name of the activated OData service: ZUI_GLACCOUNT_BALANCES.
Task 2: Check the authorization proposals for the Activated OData Service
You want to check the authorization proposals for the activated OData service ZUI_GLACCOUNT_BALANCES in back-end system S4D.
Steps
Check the authorization proposals for the activated OData service ZUI_GLACCOUNT_BALANCES.
Start the transaction SU24.
In filed Select By keep the selected entry Application Types.
In the Type of Application field, choose SAP Gateway: Service Groups Metadata.
In the Object Name field, choose the input help (F4).
Expand the Restrictions area.
In the Object Name field, enter ZUI_GLACCOUNT_BALANCES*.
Choose Start Search.
Select the search result R3TR IWSG ZUI_GLACCOUNT_BALANCES 0001.
Choose Copy.
Choose Execute (F8).
Result
An empty list is shown indicating that no authorization proposals for the activated OData service exist. Here, a proposal for the start authorization ( S_SERVICE object) is sufficient, however, it is not displayed in SU24. This is the reason why there is a warning displayed. 11. Choose Back.
Task 3: Use Table USOBHASH to evaluate the Object Name of an OData Service
Steps
Use Table USOBHASH to find out which OData service has the hash code 48FB54446180787A3209C13AD5F9D7.
Start the Data Browser transaction SE16 on the system S4D.
In the Table Name field, enter USOBHASH.
Choose Table Contents.
In the NAME field, enter 48FB54446180787A3209C13AD5F9D7.
Choose Execute.
Result
The resulting table shows the hash code in the Name column, the object type, and the name of the OData Service in the Object Name column .
| Name | Object Type | Object Name |
| --- | --- | --- |
| 48FB54446180787A3209C13AD5F9D7 | IWSV | UI_GLACCOUNT_BALANCES 0001 |
```
6. Choose *Back (F3)* 3 times.
```
Personalize your learning.
Log in and track your growth over time.
Register Log in
Was this lesson helpful?
Yes No
Continue to quiz
SAP Logo Learning
Quick links
Learning Support
About SAP
Site Information
  