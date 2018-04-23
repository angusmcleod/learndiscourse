---
title: Invite members with dormant accounts to return to network (Q2 2018)
---

Many members have dormant accounts. That is, they have not logged into the network website since we relaunched with discourse in 2015. We invited them all to come and log in again back then but alot of people ignored the invitation. 

Let's do one final round now to invite them to come back. We can then disable or remove those that are confirmed to be unreachable, without causing a huge drop in our numbers all at once or kicking people out who should be in the network.

### What success looks like 

- members who want to return are given every opportunity to do so, and are warmly welcomed! 
- those members who are unreachable (bad email addresses) are immediately removed from wordpress and mailchimp, marked "former member - unreachable" (or something like that) in salesforce 
- those members who are reachable but do not respond to invitation after 3 attempts are removed from wordpress but are left in mailchimp (where auto cleaned, and they can unsubscribe themselves as they see fit) and salesforce. Marked "former member - no response" (or some such) in salesforce 
- the member list does not drop significantly. number of old members removed roughly match number of new members joining. 
- we do our best to avoid landing in spam inboxes. 
  - monitor mandrill carefully to avoid sending again to bad addresses
- process limits lift on staff. 
  - step 1: mass email via mailchimp to all old members
  - step 2: bulk PM (are ticket tags possible?) to remaining old members (30 days later?)
  - step 3: mail merge (gmail? salesforce?) to remaining old members (30 days later?) 
  - step 4/ongoing: follow up on mandrill bounces, replies by email/tickets etc 

### Todos: 
- [] update/revise existing invite procedure now that we have tickets, make sure this process fits within the existing procedure 
- [] update bulk PM tool to allow messaging staged users
- [] draft invite messages, circulate for review
- [] create lists of people to contact (those with no 'last seen' in insight dashboard, export to csv, import to google sheets for manipulating) 
  - [] decide if segmenting list is at all useful (eg by language, level of engagement) 
- [] set up mailchimp mailing and schedule sending 
- [] set up bulk PM mailing and plan when to send
- [] set up plan for removing members on schedule, so not 
- [] handle onboarding of returning members as usual

<small class="documentation-source">Source: [https://community.namati.org/t/invite-members-with-dormant-accounts-to-return-to-network-q2-2018/42753](https://community.namati.org/t/invite-members-with-dormant-accounts-to-return-to-network-q2-2018/42753)</small>
