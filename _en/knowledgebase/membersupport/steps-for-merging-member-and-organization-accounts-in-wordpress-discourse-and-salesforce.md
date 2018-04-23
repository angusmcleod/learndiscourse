---
title: Steps for merging member and organization accounts in wordpress, discourse and salesforce
---

from time to time, we need to merge records. This happens when a member forgets they already have an account and sign up with a new one. 

- step 1: in your web browser, open up in separate tabs and review relevant members and organizations in wordpress, discourse and salesforce 
- step 2: salesforce: merge organizations (if needed) and then merge contacts. verify that contact and organization details are accurate and correct. 
- step 3: wordpress: move organization to trash (if needed) and delete user that is no longer needed. if prompted, choose the new user to own wordpress contact created by deleted user. verify that details are accurate and correct, including salesforce ID. 
- step 4: discourse: delete user account that is no longer needed. If user has authored any posts, you first need to set the new user as the owner of any topics/messages created by the old user. If user has been mentioned, follow [discourse admin procedure to remap mentions (requires ssh)](https://community.namati.org/t/discourse-admin-tasks-ssh/41128?u=tobiaseigen) 
- step 5: mailchimp: delete email address of deleted contact in mailchimp. 
- step 6: start ticket to member to let them know, and follow up until resolved. 
 

---- 
note: there is a new feature to merge users in discourse that may simplify the discourse step - not yet tested by me. 

https://meta.discourse.org/t/ability-to-merge-users/9220/89?u=tobiaseigen

<small class="documentation-source">Source: [https://community.namati.org/t/steps-for-merging-member-and-organization-accounts-in-wordpress-discourse-and-salesforce/42343](https://community.namati.org/t/steps-for-merging-member-and-organization-accounts-in-wordpress-discourse-and-salesforce/42343)</small>
