---
title: CSA Mock Exam – Weak Areas (Exam 3 review)
description: 60-question ServiceNow Certified System Administrator (CSA) practice exam built from the questions missed in "Exam 3 – 2026", with an answer key that links to the matching pages in this repository.
locale: en-US
release: brazil
topic_type: reference
last_updated: "2026-10-06"
---

# CSA Mock Exam – Weak Areas

This practice exam targets the topics that were answered incorrectly in **Exam 3 – 2026** (source: `CSA_Question_Type.docx`). Every question tests one of those weak spots, often from a different angle than the original question, so that you check the concept rather than memorise an answer.

- **Questions:** 60 (single answer unless the question says "Select N")
- **Suggested time:** 90 minutes, like the real CSA exam
- **Passing target:** 70% (42 / 60)
- **Answer key:** at the end of the file, with a short explanation and a link to the relevant documentation page in this repository.

## Weak areas covered

| # | Domain | Weak spots from Exam 3 | Questions |
|---|--------|------------------------|-----------|
| 1 | CMDB & CSDM | Dependent CI retirement, CI Attestation, IRE related entries, Multisource CMDB, Intelligent Search, CMDB Workspace views, quick start tests, CSDM life cycle, ways to create CIs | 1–13 |
| 2 | Service Catalog | Request methods, RITM closure, fulfiller modules, Catalog Builder, Wizards, record producers, Now Assist | 14–22 |
| 3 | Knowledge Management | Word import, Publish behaviour, Can Contribute defaults, sitemap, favourites | 23–27 |
| 4 | Platform UI & navigation | Filter navigator, list context menus, wildcards, start page, Configuration Hub, Form Designer, templates, Sidebar, workspaces, Visual Task Boards | 28–39 |
| 5 | Security & user administration | Role delegation, admin/security_admin rules, group types, SSO, Shared Responsibility Model, Data Discovery | 40–45 |
| 6 | Notifications, email & SLA | Auto Opt-in, inbound watermarks, notification preferences, SLA escalation, SLA Timeline | 46–50 |
| 7 | Data, import & schema | Import set records, transform maps, Easy Import, coalesce, archiving, database views, field attributes | 51–57 |
| 8 | Reporting, Flow Designer & app development | Standard deviation, report designer tabs, Flow Designer benefits and data pills, Creator Studio, Application Collaboration, Proactive Triggers | 58–60 + bonus |

---

## Section 1 – CMDB & CSDM

**Question 1.** When a parent CI is set to Retired, Dependent CIs Management tries to cascade the update to every CI that depends on it. In which table are those dependent CIs recorded?

- A. cmdb_ci_related_retire
- B. cmdb_related_entry
- C. cmdb_dependent_ci_ledger
- D. cmdb_dependent_ci_extra_rels_config

**Question 2.** In CMDB Workspace, which capability lets owners systematically confirm, in bulk, that the IT infrastructure and applications they own actually exist?

- A. Multisource Report Builder
- B. Identification and Reconciliation Engine
- C. CI Attestation
- D. IntegrationHub ETL

**Question 3.** You must keep the history of every CI attribute update reported by every discovery source, not only the value that wins reconciliation. What do you do?

- A. Install the CMDB Mainframe plugin
- B. Enable Multisource CMDB
- C. Populate a CMDB group
- D. Use the CMDB CI Class Models store app

**Question 4.** Which tool do you use to add related entries to an Identification and Reconciliation Engine (IRE) identification rule for a CI class?

- A. CMDB Data Manager
- B. Service Graph connectors
- C. CI Class Manager
- D. CMDB Query Builder

**Question 5.** Tables such as Serial Number [cmdb_serial_number] do not extend cmdb_ci but reference a CI. Where are these related tables declared so the IRE can use them?

- A. Related Entries [cmdb_related_entry]
- B. CI Relationship [cmdb_rel_ci]
- C. Dependent CI Ledger [cmdb_dependent_ci_ledger]
- D. Suggested Relationships [cmdb_rel_type_suggest]

**Question 6.** Which CMDB feature lets a user type a simple natural-language phrase in a search string to return a set of CIs?

- A. Contextual Search
- B. CMDB Data Manager
- C. Intelligent Search
- D. Conditional Search

**Question 7.** Your CMDB is heavily customised. How do you verify that it still works after an upgrade or after deploying a new integration?

- A. Use the CMDB Health quick starter
- B. Run the out-of-the-box quick start tests unchanged; they also cover customisations
- C. Copy the CMDB quick start tests and configure them for your instance data
- D. Override the quick start tests through scripting

**Question 8.** Which CMDB Workspace view shows the overall CMDB health state together with recent activities and items such as duplicate CIs?

- A. Home
- B. CMDB 360
- C. Governance
- D. Management

**Question 9.** In CSDM, which pair of standard fields is used consistently across applications to track the life cycle of an asset or CI? (Select 2)

- A. Life Cycle Stage
- B. Install Status
- C. Life Cycle Stage Status
- D. Operational Status
- E. Hardware Status

**Question 10.** Which processes can create configuration items in the CMDB? (Select 3)

- A. Change management
- B. Incident management
- C. Asset management
- D. Service catalogue fulfilment
- E. Knowledge article publication

**Question 11.** Which IT challenges does a CMDB help solve? (Select 3)

- A. Consolidating disparate CI data into a single system
- B. Capturing only already-known CIs
- C. Regularly maintaining complex data for accuracy
- D. Making sense of data to drive decisions and services
- E. Replacing the need for a change process

**Question 12.** What is the main role of stakeholders when you implement and maintain the CMDB?

- A. Import CI data such as name, source and relationships
- B. Determine the specific CI information required to support capabilities and build organisational buy-in
- C. Create a go-forward strategy for configuration management responsibilities
- D. Build reports showing CI health for each department

**Question 13.** What does the IRE use to decide whether an incoming payload matches an existing CI before it inserts or updates it?

- A. Identification rules with identifier entries for the CI class
- B. Reconciliation rules only
- C. CI relationship types
- D. Data refresh rules

## Section 2 – Service Catalog

**Question 14.** What are the three request methods that can be configured on a catalogue item? (Select 3)

- A. Submit
- B. Wish List
- C. Request
- D. Order
- E. Save

**Question 15.** A fulfiller closes every catalogue task for one item in a request. What happens next in the default workflow?

- A. The request is automatically set to Closed Complete
- B. The requester is notified that the request is complete
- C. The requested item is automatically set to Closed Complete
- D. The requested item moves to the next phase of fulfilment

**Question 16.** Where can fulfillers find catalogue tasks assigned to them and to their groups? (Select 2)

- A. All > Service Catalog > My Work
- B. All > Service Desk > My Work
- C. All > Service Catalog > My Groups Work
- D. All > Service Desk > My Groups Work

**Question 17.** In Catalog Builder, where do you set a value or show a message for a question based on a set of conditions?

- A. Details
- B. Settings
- C. Dynamic behavior
- D. Review and submit

**Question 18.** What can administrators use to simplify a complex, multi-form input experience in the Service Catalog?

- A. Catalog Builder
- B. Service Catalog Wizards
- C. Declarative actions
- D. Custom actions

**Question 19.** Which of the following can you do with Catalog Builder? (Select 3)

- A. Configure the default value for a question
- B. Configure Catalog Builder so catalogue item editors can enter custom details
- C. Transfer catalogue items published through Catalog Builder using exclusive update sets
- D. Write catalogue client scripts in a code editor
- E. Create flows in Workflow Studio

**Question 20.** Which role lets an administrator create record producers so users can raise issues or enquiries directly from the Service Catalogue?

- A. itil_admin
- B. catalog_admin
- C. catalog_item_designer
- D. incident_manager

**Question 21.** As a catalogue admin, you must populate the Manager's name automatically whenever the "Requested for" value changes. Where do you define this relationship between the two questions without scripting?

- A. Catalog Item Templates
- B. Service Designer
- C. Catalog Builder
- D. Service Catalog Wizards

**Question 22.** Which records can AI generate in ServiceNow through Now Assist skills? (Select 2)

- A. Catalogue items
- B. User records
- C. Configuration items
- D. Knowledge articles

## Section 3 – Knowledge Management

**Question 23.** What is mandatory to select when you import Microsoft Word documents as knowledge articles?

- A. Category
- B. Knowledge Base
- C. Publish
- D. Short description

**Question 24.** What happens when you select **Publish** on knowledge articles created manually or by import?

- A. The articles move straight to the Published state
- B. The publish workflow assigned to the knowledge base is triggered
- C. The articles are always sent for approval
- D. The articles are deleted from the draft list

**Question 25.** No user criteria are defined for **Can Contribute** on a knowledge base (default property values). Who can contribute?

- A. Only Knowledge Base Managers
- B. All users, including users without roles
- C. All users that have at least one role
- D. No one

**Question 26.** You want public search engines to index your knowledge article URLs. What do you configure for the Knowledge Portal?

- A. Contextual Search – Service Portal
- B. A Sitemap Generator record
- C. Next Experience UI for knowledge articles
- D. Service Portal Analytics

**Question 27.** How can users quickly reference their most frequently used articles in the Service Portal?

- A. By rating them or marking them as helpful
- B. By flagging them
- C. By marking them as favourites
- D. By creating a shortcut link

## Section 4 – Platform UI & navigation

**Question 28.** Which component do you use to see which applications and modules contain the keyword "task"?

- A. Global search
- B. Filter navigator
- C. Help sidebar
- D. Database view

**Question 29.** Which menu gives access to actions such as creating quick reports, configuring the list and exporting data?

- A. List context menu
- B. Column context menu
- C. Record context menu
- D. Value context menu

**Question 30.** Which wildcard returns list records whose value contains the search term anywhere in the string?

- A. ! (exclamation mark)
- B. % (per cent sign)
- C. * (asterisk)
- D. = (equal sign)

**Question 31.** Which start page preference options are available besides the default landing page? (Select 3)

- A. Continue my last session
- B. Continue where I last left off
- C. Use the page that I'm on now
- D. Use Dashboards
- E. Use my last search

**Question 32.** Where do you go to quickly find tables, configurations and metadata records for any application installed on your instance?

- A. Analytics Hub
- B. Integration Hub
- C. Configuration Hub
- D. Manager Hub

**Question 33.** In Form Designer, which part of the interface do you use to add a field to both the table and the form?

- A. Field Formatter
- B. Form Views
- C. Form Settings
- D. Field Navigator

**Question 34.** Different form templates are applied to a form from the:

- A. Template creator
- B. Template bar
- C. Toggle template views
- D. Template editor

**Question 35.** How can you open Form Builder? (Select 3)

- A. From Related Links on a table's configuration page
- B. From Catalog Builder
- C. From Table Builder (Forms tab)
- D. From a form on the platform (Configure > Form Builder)
- E. From the Service Portal designer

**Question 36.** What can agents do with the Sidebar in the Next Experience UI? (Select 2)

- A. Communicate directly with the caller or requester
- B. Create, open and search for discussions about their work
- C. Integrate with other workspaces to show related records
- D. Collaborate in real time with others from a workspace interaction-based record

**Question 37.** Which features help team members collaborate on tasks? (Select 4)

- A. Connect chat / Sidebar
- B. Additional comments
- C. User presence
- D. Activity stream
- E. Work notes

**Question 38.** Which options are available to workspace users when they send email from a workspace? (Select 2)

- A. Schedule emails for later delivery
- B. Auto-save email drafts
- C. Track the delivery status of sent emails
- D. Add email addresses into recipient fields

**Question 39.** Which option lets the board owner sort a Visual Task Board using criteria they create?

- A. Load Filter
- B. Breakdown Element
- C. Interactive Filter
- D. Edit Filter and Sort

## Section 5 – Security & user administration

**Question 40.** Which roles CANNOT be delegated? (Select 2)

- A. itil
- B. user_admin
- C. role_delegator
- D. admin

**Question 41.** Which statements about granting elevated roles are true? (Select 3)

- A. To grant the admin role to a user, the granting user must also have the admin role
- B. A user with only the user_admin role can grant the admin role
- C. Non-admin users cannot add users to a group that contains the admin role
- D. A user with only the admin role cannot grant the security_admin role
- E. A non-admin user with only security_admin can add a user to a group that contains security_admin

**Question 42.** Which group types are provided in the base system? (Select 3)

- A. survey
- B. catalog
- C. approval
- D. notification
- E. itil

**Question 43.** Which authentication method lets users sign in to ServiceNow through a social identity provider such as Google or Okta?

- A. SAML 2.0
- B. Digest authentication
- C. OpenID Connect
- D. LDAP

**Question 44.** Under the Shared Responsibility Model, who is responsible for securing instance configuration, authentication and authorisation, and data encryption at rest?

- A. The data processor (ServiceNow)
- B. The data centre provider
- C. The network provider
- D. The data controller (customer)

**Question 45.** Which application finds Personally Identifiable Information (PII) in the instance so that you can classify, report on or act on it?

- A. Data Classification
- B. Data Privacy
- C. Data Discovery
- D. Data Separation

## Section 6 – Notifications, email & SLA

**Question 46.** As an admin, which notification behaviour can you modify for a destination type?

- A. Mandatory Opt-out
- B. Sender preference
- C. Auto Opt-in
- D. Send to All

**Question 47.** How does ServiceNow process an inbound email that carries the watermark of an existing record?

- A. It clears the existing task and overwrites it with the new values
- B. It creates a copy of the task as a child record
- C. It ignores the email because the task already exists
- D. It updates the existing task according to the inbound email action script

**Question 48.** Where can a user filter system notifications by category and search their custom notifications? (Select 2)

- A. All > System Notification > Email > Notification Categories
- B. User Profile > Preferences > Notifications > Advanced Preferences
- C. All > System Notification > Email > Notification Filters
- D. All > Self-Service > My Notification Preferences > Advanced Preferences

**Question 49.** With the default SLA workflow, when is the resolution SLA first escalated to the assignee's manager with an automatic notification?

- A. At 50% elapsed time
- B. At 75% elapsed time
- C. At 100% elapsed time
- D. Never

**Question 50.** What can you do in the SLA Timeline for a task? (Select 3)

- A. View related task updates
- B. Identify why a task update triggered a specific stage in the task SLA
- C. View the progress of task SLAs, OLAs and underpinning contracts
- D. Send notifications to the assignment group members and manager

## Section 7 – Data, import & schema

**Question 51.** Which details can you find in the import set record after an import runs? (Select 3)

- A. Import Set Rows
- B. Concurrent Import Sets
- C. Import Set Runs
- D. Import Set API
- E. Import Log

**Question 52.** Data imported into the Choice table for Categories and Subcategories is missing values for mandatory fields that are not in the spreadsheet. What do you use in the transform map to set them?

- A. Coalesce
- B. Source script
- C. Map
- D. Target field

**Question 53.** In a transform map, what makes the import update an existing record instead of inserting a new one when the values match?

- A. Choice action
- B. Coalesce
- C. Run business rules
- D. Enforce mandatory fields

**Question 54.** Put the Easy Import steps in order.

- A. Download Excel template → Complete Excel template → Upload import data → Preview import data → Finalise import
- B. Upload import data → Download Excel template → Preview import data → Complete Excel template → Finalise import
- C. Complete Excel template → Download Excel template → Preview import data → Upload import data → Finalise import
- D. Download Excel template → Upload import data → Complete Excel template → Finalise import → Preview import data

**Question 55.** How do you delete related records from the archive log and the archive (ar_) tables?

- A. Restore archived records and related records
- B. Create archive destroy rules
- C. Re-archive restored records
- D. Delete archive record log entries

**Question 56.** Which statements are database view limitations? (Select 3)

- A. Database view tables cannot be added as a data preserver in clone requests
- B. The where clause of a database view cannot use indexed fields
- C. Database views cannot be created on tables that participate in table rotation
- D. Data cannot be edited in the database view output

**Question 57.** What are the three key attributes of every field? (Select 3)

- A. ID
- B. Field label
- C. Value
- D. Location
- E. Field name

## Section 8 – Reporting, Flow Designer & app development

**Question 58.** Which report aggregation shows how much the data varies from the average value of a field?

- A. Count distinct
- B. Average
- C. Standard deviation
- D. Sum

**Question 59.** What are benefits of Flow Designer? (Select 3)

- A. Subject matter experts can develop and share reusable actions
- B. It provides multiple environments to build and visualise processes
- C. It replaces every existing workflow automatically
- D. It provides configuration and runtime information to create, operate and troubleshoot flows from one interface
- E. It provides natural-language descriptions of flow logic

**Question 60.** How can you change data pill values in Flow Designer without writing scripts?

- A. Allow duplicate query parameter names
- B. Use the flow error handler
- C. Install data pill package plugins
- D. Use transform functions

### Bonus questions (also from the Exam 3 misses)

**Bonus 1.** Which ServiceNow product lets you create request fulfilment applications without writing code?

- A. App Engine Studio
- B. Creator Studio
- C. Guided Application Creator
- D. ServiceNow Studio

**Bonus 2.** Which application helps end users through the Virtual Agent or Agent Chat by offering helpful platform actions based on real-time data?

- A. Predictive Intelligence
- B. Natural Language Understanding
- C. Performance Analytics
- D. Proactive Triggers

**Bonus 3.** How does Application Collaboration help when you build applications with App Engine?

- A. Non-administrators can develop and deploy any application
- B. Administrators can delete applications
- C. Collaborator permissions can be managed per application
- D. Delegated developers get source control automatically

**Bonus 4.** Which business needs can Flow Designer address? (Select 3)

- A. Orchestrating business processes across services with little technical knowledge
- B. Redeveloping logic already built in the legacy workflow editor
- C. Integrating with third-party systems
- D. Reducing technical debt, for example less scripting to simplify upgrades

**Bonus 5.** On the Report Designer, under which tab do you define how a bar chart is grouped?

- A. Data
- B. Type
- C. Configure
- D. Style

---

## Answer key

| Q | Answer | Q | Answer | Q | Answer | Q | Answer |
|---|--------|---|--------|---|--------|---|--------|
| 1 | C | 16 | B, D | 31 | B, C, D | 46 | C |
| 2 | C | 17 | C | 32 | C | 47 | D |
| 3 | B | 18 | B | 33 | D | 48 | B, D |
| 4 | C | 19 | A, B, C | 34 | B | 49 | B |
| 5 | A | 20 | B | 35 | A, C, D | 50 | A, B, C |
| 6 | C | 21 | C | 36 | B, D | 51 | A, C, E |
| 7 | C | 22 | A, D | 37 | A, C, D, E | 52 | B |
| 8 | D | 23 | B | 38 | B, D | 53 | B |
| 9 | A, C | 24 | B | 39 | D | 54 | A |
| 10 | A, C, D | 25 | C | 40 | C, D | 55 | B |
| 11 | A, C, D | 26 | B | 41 | A, C, D | 56 | A, C, D |
| 12 | B | 27 | C | 42 | A, B, E | 57 | B, C, E |
| 13 | A | 28 | B | 43 | C | 58 | C |
| 14 | A, C, D | 29 | B | 44 | D | 59 | A, D, E |
| 15 | C | 30 | C | 45 | C | 60 | D |

Bonus: 1 B · 2 D · 3 C · 4 A, C, D · 5 C

## Explanations

### CMDB & CSDM

1. **C.** Dependent CIs Management lists the dependent CIs of a retiring parent in the CMDB Dependent CI Ledger [cmdb_dependent_ci_ledger] table and then processes their life cycle updates. *Watch out:* `cmdb_ci_related_retire` does not exist; an AI chat answer in the source document claimed it was correct. See [Manage dependent CIs](../markdown/servicenow-platform/configuration-management-database-cmdb/manage-dependent-ci.md) and [CMDB Data Manager components](../markdown/servicenow-platform/configuration-management-database-cmdb/components-cmdb-data-manager.md).
2. **C.** CI Attestation (a CMDB Data Manager policy type) asks owners to confirm that the CIs they manage really exist. Multisource Report Builder reports on source data, and the IRE identifies and reconciles payloads. See [Run an attestation policy on demand](../markdown/servicenow-platform/configuration-management-database-cmdb/run-attestation-policy-ondemand.md).
3. **B.** Multisource CMDB stores every value reported by every source, not only the reconciled one. See [Multisource CMDB](../markdown/servicenow-platform/configuration-management-database-cmdb/multisource-cmdb.md).
4. **C.** CI Class Manager is where you configure a class's identification rules, identifier entries and related entries. CMDB Data Manager handles life cycle policies (retire, archive, delete, attest). See [CI Class Manager](../markdown/servicenow-platform/configuration-management-database-cmdb/ci-class-manager-landing-page.md).
5. **A.** Related tables that reference a CI are specified in Related Entries [cmdb_related_entry]. See [Configuration management and CMDB](../markdown/servicenow-platform/configuration-management-database-cmdb/cnfig-mgmt-and-cmdb.md).
6. **C.** Intelligent Search for CMDB turns a natural-language phrase into a CI query. Contextual Search suggests knowledge articles on forms. See [Intelligent Search for CMDB](../markdown/servicenow-platform/configuration-management-database-cmdb/intelligent-search-cmdb.md).
7. **C.** Copy the CMDB quick start tests and customise them so they pass with your instance-specific data. The out-of-the-box tests do not know your customisations. See [CMDB quick start tests](../markdown/servicenow-platform/configuration-management-database-cmdb/quick-start-tests-cmdb.md).
8. **D.** The Management view shows recent key activities and health indicators (including duplicates). Home is for searching and urgent actions, and CMDB 360 compares discovery sources. See [Set up CMDB Workspace](../markdown/servicenow-platform/configuration-management-database-cmdb/setup-cmdb-workspace.md).
9. **A, C.** CSDM tracks the life cycle with the Life Cycle Stage and Life Cycle Stage Status pair. See [CSDM life cycle standard values](../markdown/servicenow-platform/common-service-data-model-csdm/csdm-life-cycle-standard-values.md).
10. **A, C, D.** CIs come from change management, asset management, service catalogue fulfilment, Discovery, integrations, imports and manual creation. Incident management consumes CIs and does not create them.
11. **A, C, D.** A CMDB consolidates disparate CI data, keeps complex data accurate, and turns data into decisions.
12. **B.** Stakeholders (process owners, process managers and SMEs) determine which CI information is needed to support capabilities, and they build buy-in.
13. **A.** The IRE matches incoming data with the identification rules (identifier entries, and related entries when needed) of the CI class. Reconciliation rules decide which source may update which attributes.

### Service Catalog

14. **A, C, D.** The request methods are Submit, Request and Order. Wish List is a portal feature, not a request method.
15. **C.** When all of an item's catalogue tasks are closed, the requested item (RITM) moves to Closed Complete. The request closes only when all of its RITMs are closed.
16. **B, D.** Catalogue tasks for fulfillers are under **Service Desk > My Work** and **Service Desk > My Groups Work**. The Service Catalog application has no My Work modules.
17. **C.** Catalog Builder's dynamic behaviour step lets you set values or show messages based on conditions. See [Create UI policies in Catalog Builder](../markdown/servicenow-platform/service-catalog/create-ui-policies-in-catalog-builder.md).
18. **B.** Service Catalog Wizards chain several catalogue items and forms into one guided experience. See [Catalog wizard](../markdown/servicenow-platform/service-catalog/catalog-wizard.md).
19. **A, B, C.** Catalog Builder can set default question values, be configured so editors enter custom details, and move published items with exclusive update sets. See [Catalog Builder overview](../markdown/servicenow-platform/service-catalog/catalog-builder-overview.md).
20. **B.** catalog_admin manages catalogue items, including record producers.
21. **C.** Define the dependency between "Requested for" and "Manager" in Catalog Builder (dynamic behaviour), with no script needed.
22. **A, D.** Now Assist can generate catalogue items and knowledge articles. See [Create a catalog item using Now Assist](../markdown/servicenow-platform/service-catalog/create-catalog-item-using-now-assist.md).

### Knowledge Management

23. **B.** A target knowledge base is mandatory when you import Word documents. See [Import a Word document](../markdown/servicenow-platform/knowledge-management/import-word-platform.md).
24. **B.** Publish starts the publish workflow of the article's knowledge base. With an approval workflow, the article goes to Review first and does not jump straight to Published.
25. **C.** With no Can Contribute criteria, all users with at least one role can contribute (and all users can read). This is controlled by `glide.knowman.block_access_with_no_user_criteria`. See [User access to knowledge](../markdown/servicenow-platform/knowledge-management/user-access-knowledge.md).
26. **B.** Create a Sitemap Generator record for the Knowledge Portal. See [Configure the sitemap generator](../markdown/servicenow-platform/knowledge-management/config-sitemap-generator.md).
27. **C.** Marking articles as favourites gives quick access to them. Rating and "helpful" feedback improve article quality but do not create shortcuts.

### Platform UI & navigation

28. **B.** The filter navigator (application navigator filter) shows every application and module matching the keyword. Global search searches records, not menus. You can also type `table.list` or `table.do` there.
29. **B.** The column context menu (right-click a column header) holds quick reports (Bar/Pie chart), Configure, Export and more.
30. **C.** `*term` means contains, `%` at the start or end means ends with or starts with, `=` means equals, and `!*` and `!=` mean does not contain and does not equal. See [Wildcards](../markdown/platform-administration/search-administration/c_Wildcards.md).
31. **B, C, D.** The options are Use Dashboards, Use the page that I'm on now, and Continue where I last left off. See [Configure the start page preference](../markdown/platform-user-interface/configure-user-selected-start-page-preference.md).
32. **C.** Configuration Hub groups an application's tables, configurations and metadata. See [Configuration Hub](../markdown/platform-administration/admin-center/ac-configuration-hub.md).
33. **D.** In Form Designer, the Field Navigator (Fields and Field Types tabs) lets you drag a new field type onto the form, which also creates it on the table. See [Form Designer overview](../markdown/integrate-applications/form-designer-overview.md).
34. **B.** Templates are applied from the template bar at the bottom of the form.
35. **A, C, D.** Form Builder opens from Table Builder (Forms tab), from Configure > Form Builder on a form, from Related Links on the table configuration, and from UI Builder (Edit form). Catalog Builder is for catalogue items only.
36. **B, D.** The Sidebar is for internal discussions: you create, open and search them, and collaborate in real time from an interaction-based record. It is not used to talk to the caller.
37. **A, C, D, E.** Connect/Sidebar, user presence, the activity stream and work notes are internal collaboration tools. Additional comments are customer-visible.
38. **B, D.** Workspace email auto-saves drafts and lets you add addresses to the recipient fields.
39. **D.** Board owners create sort criteria and later change them with **Edit Filter and Sort**. See [Sort Visual Task Boards](../markdown/platform-user-interface/visual-task-boards/sort-visual-task-boards.md).

### Security & user administration

40. **C, D.** Elevated roles such as admin, security_admin and role_delegator itself cannot be delegated. itil and user_admin can be.
41. **A, C, D.** Only an admin can grant admin, non-admins cannot add members to a group that holds admin, and admin alone cannot grant security_admin (that needs elevated security_admin).
42. **A, B, E.** The base system types are **catalog**, **itil** and **survey**. See [Configure assignment group types](../markdown/platform-administration/user-administration/c_ConfigGroupTypesForAssignGroups.md).
43. **C.** OpenID Connect is the SSO protocol for social and OIDC identity providers such as Google and Okta. SAML 2.0 is enterprise SSO, and LDAP is directory authentication.
44. **D.** The customer, as data controller, owns instance configuration, authentication and authorisation, and data encryption at rest.
45. **C.** Data Discovery [sn_data_discovery] runs jobs over tables to find sensitive data such as card numbers and emails. Data Classification groups data by type, Data Privacy anonymises it, and Data Separation restricts access by lens hierarchy. See [Data Discovery](../markdown/platform-security/data-discovery).

### Notifications, email & SLA

46. **C.** Admins can modify the Auto Opt-in behaviour for a destination type. See [Notification provider](../markdown/platform-administration/notification-provider.md).
47. **D.** A matching watermark makes the email a reply, and the matching inbound email action script updates the record. See [Working with watermarks](../markdown/platform-administration/c_WorkingWithWatermarks.md) and [Inbound email actions](../markdown/platform-administration/actions-inbound-email.md).
48. **B, D.** Both paths open Advanced Preferences, where notifications can be filtered by category and searched. See [User notification preferences](../markdown/platform-administration/user-notification-preferences.md).
49. **B.** At 50% the assignee is notified, at 75% the assignee's manager is notified for the first time, and at 100% the breach is notified.
50. **A, B, C.** The SLA Timeline shows related task updates, why an update triggered a stage, and the progress of SLAs, OLAs and UCs. It does not send notifications. See [Verify an SLA definition using the SLA Timeline](../markdown/it-service-management/service-level-management/Verify-sla-definition-using-sla-timeline.md).

### Data, import & schema

51. **A, C, E.** The import set record has Import Set Rows, Import Set Runs and Import Log related lists.
52. **B.** A field map source script returns a value for target fields that are not in the source file.
53. **B.** Coalesce fields act as a unique key, so a match updates the record and no match inserts one. See [Import set coalesce](../markdown/integrate-applications/system-import-sets/c_ImportSetCoalesce.md).
54. **A.** The steps are download the template, complete it, upload, preview, then finalise. See [Easy Import](../markdown/integrate-applications/easy-import).
55. **B.** Archive destroy rules delete archived records and their related records from the archive log and the ar_ tables.
56. **A, C, D.** Option B is false, because where clauses should use indexed fields for performance. See [Database views](../markdown/platform-administration/table-administration-and-data-management/c_DatabaseViews.md).
57. **B, C, E.** Every field has a label, a name and a value.

### Reporting, Flow Designer & app development

58. **C.** Standard deviation measures how much values vary from the average.
59. **A, D, E.** Flow Designer lets SMEs build reusable actions, gives one interface for configuration and runtime troubleshooting, and describes flow logic in natural language.
60. **D.** Transform functions change data pill values with no script. See [Transform functions](../markdown/build-workflows/workflow-studio/transform-functions.md).

**Bonus 1. B.** Creator Studio builds request-fulfilment apps with no code. See [Creator Studio](../markdown/application-development/creator-studio).
**Bonus 2. D.** Proactive Triggers suggest actions in Virtual Agent and Agent Chat from real-time data. See [Proactive triggers](../markdown/conversational-interfaces/product-support-for-technology/proactive-triggers.md).
**Bonus 3. C.** Application Collaboration lets you manage collaborator permissions per application. See [Manage app collaborators](../markdown/application-development/servicenow-studio-classic/manage-app-collab-servicenow-studio.md).
**Bonus 4. A, C, D.** Flow Designer orchestrates processes across services, integrates third-party systems, and reduces scripting. It is not meant for rebuilding existing legacy workflows.
**Bonus 5. C.** Grouping is set on the Configure tab. Data holds the name and source, Type holds the visualisation, and Style holds colours and titles.
