> Source: https://books.espresso-tutorials.com/beginners-guide-to-sap-security-and-authorizations

Beginner`s Guide to SAP Security and Authorizations | SAP ebooks and videos - SAP finally explained | Espresso Tutorials GmbH
Start 
“Whereas I used to waste my time Googling... or sifting through the tables of contents of the giant's thousand-page references... now I do it this way: I check out Espresso Tutorials. I read through it in a reasonable amount of time—and get my tasks done.”
A. Stier
Beginner`s Guide to SAP Security and Authorizations
SAP has a wide range of built-in functionality to meet various security requirements, including network protection, data protection, and SAP authorizations. This book will focus on the application of SAP authorizations and how user access can be limited b...
Show more Reading sample
Learn for free for 7 days now
Table of content
Preface: Introduction to SAP Security and Authorizations concept
1 User maintenance overview
2 Role overview
3 Profile generator and role maintenance overview
4 Advanced topics for role maintenance
5 SAP Security and Authorizations trouble-shooting
6 Advanced topics for SAP authorizations
7 Acknowledgements
A About the author
B Disclaimer
More Information
Author:
Tracy Juran
Category:
Security & Identity Management
Language:
Englisch
Reading sample
2.1 Role types
There are two types of SAP roles: single and composite. Furthermore, single roles can be set up as reference-derived roles or enabler roles. This section provides a brief overview of each type of role and what each type is used for. Chapter 3 shows how to create each role and maintain it using the profile generator transaction (PFCG).
Single roles provide access to actions and permissions that make up a user's job or a subset of job responsibilities. Actions can be thought of as transactions and permissions thought of as authorization objects and associated field values. Single roles are the most common type of SAP role.
Actions and permissions example
```
<p class="BoxTipText"><img alt="Example" class="BoxImage" height="90" src="%%ATTACHMENT:127992%%" width="90" loading="lazy">Sales clerk Todd Levine needs to be able to create and maintain sales orders in SAP. This translates to transaction codes VA01 and VA02. However, Todd can only maintain certain sales doc types (he is not allowed to create return orders) and is only authorized to do so using company code 1000. These limitations are controlled by his explicit access to various authorization objects within his user roles.</p>
```
Referenced-derived roles are roles that inherit the menu structure, authorization objects, and authorization values from an existing role. Derived roles are often called child roles, whereas the imparting role may be called the parent or master role. A derived role is useful when you want to mirror the exact same functionality as the master role, but want to manipulate the organizational levels. When creating derived roles, organization levels and user assignments are not passed from the parent to the child. In fact, these are the only role attributes that should be maintained directly in the derived role, all other changes should be maintained in the master role and inherited by the children.
Reference-derived role example
```
<p class="BoxTipText"><img alt="Example" class="BoxImage" height="90" src="%%ATTACHMENT:127992%%" width="90" loading="lazy">As noted above, Todd Levine is a sales clerk for company XYZ. However, Todd only needs access to maintain and create sales orders for company code 1000. Marla Levine, however, needs access to maintain and create sales orders for company code 2000. Otherwise, their access should be identical. In this case, a master role, Z_MAINT_SALES_ORDERS_ALL would be created as the parent or imparting role. Two derived roles, Z_MAINT_SALES_ORDERS_1000 and Z_MAINT_SALES_ORDERS_2000 would be maintained as referenced-derived roles.</p>
```
Many companies use a reference-derived role as a tactical tool to reduce the time and resources necessary for ongoing role maintenance. Reference-derived roles are also used as a case for scalability because they can easily be mixed and matched to fit a business user's job responsibilities and organizational assignments.
An enabler role can be thought of as a bolt-on role. Unlike derived roles, enabler roles are created without any link to an already existing role. Enabler roles have manually added authorization objects added to them with only desired field values maintained.
Enabler role example
```
<p class="BoxTipText"><img alt="Example" class="BoxImage" height="90" src="%%ATTACHMENT:127992%%" width="90" loading="lazy">Release strategies are a common example of when enabler roles are useful. An example is when a company wants all purchasing administrators to have access to all purchasing-related activities, but wants to limit the team’s access to specific release strategies based on levels. Release strategy authorization is controlled by a single SAP authorization object: M_EINK_FRG which has two fields, Release Code and Release Group. This authorization object can be inactivated within the purchasing admin role and bolt-on enabler roles can be created, one for each Release Code and Release Group combination and assigned ad hoc to each purchasing admin.</p>
```
A composite role, also known as a collective role, is a grouping of two or more single roles. Composite roles are used for the purpose of simplifying the assignment of roles to users. Composite roles do not contain any authorization data, only other roles. Furthermore, composite roles can only be groupings of single roles, not other collective roles.
3 Profile generator and role maintenance overview
This chapter introduces the profile generator transaction, PFCG. The profile generator tool is responsible for enabling the SAP Security administrator to create specific user roles, which contain authorizations to various system functions. Chapter 4 identifies the relationship between profiles, roles, and authorizations and the basic maintenance features within the transaction.
All content - Learn for 7 days now, free of charge and with no obligation.
7 days of free and unlimited access to all learning content 1 und den Espresso Tutorials SAP-Copiloten Espressi.
1
Enter mail
2
Confirm mail
3
Learn 7 days
Email [-] By submitting this form, you agree to our terms and conditions , privacy policy and to receiving news by email. 1
I'm a human
Secured by Cap
Try 7 days free of charge
You can unsubscribe from the Espresso Tutorials newsletter at any time by clicking on Unsubscribe in an email from the newsletter.
Already have an account? Log in now. 1
You will have access to all learning content included in the Silver subscription. Certificates are part of the Gold subscription. Online training courses are NOT part of the Digital subscription.
10% discount
Get 10% off now! Sign up for our newsletter and receive a 10% discount on a digital subscription to our SAP learning platform!
Email
Subscribe now
Copyright © 2017 - 2026 Espresso Tutorials GmbH
All rights reserved.
Impressum
AGB
Datenschutz