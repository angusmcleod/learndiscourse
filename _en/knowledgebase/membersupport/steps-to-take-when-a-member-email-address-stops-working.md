---
title: Steps to take when a member email address stops working
---

Often times, a member will become unreachable due to a change in email address, cancellation of membership, a death, or some other special circumstance. Bounce rates affect our Mailchimp score and clutter our directory with unreachable members, so it is important to keep this information up to date as best we can. Below find steps for what to do in each scenario.

# What Success Looks Like

* Each non-working email address is reviewed and dealt with in a timely manner, including: 
    - bounced email in Mandrill 
    - "cleaned" contact in Mailchimp 
    - autoreplies from mailings indicating person is no longer using email address/has left organization 

* Each contact with a non-working email has their network invitation field in Salesforce set to the appropriate status: 
    -  Former member (deceased)
    -  Former member (cancelled membership)
    -  Former member (no longer reachable)

* Inform @deylacurtis when handling any contacts with non-working email and contact type besides "Practitioner" 

* All members that request a cancellation of their accounts are removed from Wordpress, anonymized or deleted in Discourse (dependent on if they have contributed), and updated in salesforce accordingly

* If a Network Champion becomes unreachable, every reasonable effort is made to assign a new Network Champion and a PM sent to inform them of their new status

* If an organization becomes unreachable, it is removed from directory

# Step by step

### Case 1: Contact/Member provides alternate email address

Member's email address bounces, but they have provided an alternate email address:

* Manually update email address in Salesforce and Mailchimp. 

* If a network member, update email address in WordPress. Changing it in WordPress automatically changes it in Discourse and the member will receive a notification

### Case 2: Member is NOT affiliated with an organization and becomes unreachable

Contact has a Wordpress profile, no Discourse content, no org affiliation, no alternate email

1. Delete subscriber email address from mailchimp
2. Delete member from wordpress and discourse
3. If member has not posted to discourse, remove email from contact in salesforce
4. If member has posted to discourse, update member&rsquo;s email address in Wordpress to [community+unreachable@namati.org](mailto:community+unreachable@namati.org)
5. Turn off all email notifications for the member in discourse
6. Set Network Invitation field in salesforce to &ldquo;FORMER MEMBER (no longer reachable)&rdquo;

### Case 3: If a member IS affiliated with an organization and becomes unreachable

1. Delete subscriber email address from mailchimp
2. Remove email from Salesforce contact and set network invitation field to &ldquo;Former Member (no longer reachable)&rdquo;
3. Delete from Wordpress
4. If no discourse posts, delete from discourse
5. If discourse posts, update email address in wordpress to [community+unreachable@namati.org](mailto:community+unreachable@namati.org) and disable all email notifications in discourse
6. If unreachable member is the only member affiliated with their organization:
    1. make every reasonable attempt to contact the organization
    1. look at their website and email them inviting them to the Network and asking for a network champion
    2. Add link to org profile to monthly NGC email to ask if anyone knows who it is and can help contact the organization
    2. If a new member from that organization joins, PM them about their Network Champion status
    3. If no network champion can be located after all efforts exhausted, delete organization from directory
7. If member is the Network Champion and there are other members affiliated with org:
   1. PM all members affiliated with that organization explaining the situation and ask who is the most appropriate person to be the next network champion
   2. If there is only one other person affiliated with the organization, that member will become the Network Champion. Send them a PM on discourse informing them of their new title
8. Add notes in the “Admin Notes” box on the organization’s wordpress profile explaining updates to the profile

### Case 4: Contact has requested to cancel their membership

Within 72 hours: 
1. open up gravity forms entry to learn why they chose to cancel 
2. open up contact in wordpress, discourse and salesforce
1. In WordPress
   - if this contact network champion, investigate who might take over as network champion
   - delete wordpress account 
2. In Discourse:
   * Delete discourse account if member has no discourse content
   * Anonymize discourse account if member DOES have discourse conten (this is not reversible)
3. In Salesforce: 
   * Update salesforce network invitation field to "Former member (cancelled membership)"
4. Send a reply email to let the contact know their membership has been cancelled, along these lines: 

> Greetings,
> 
> We received your request to cancel your membership in the Global Legal Empowerment Network. Your account has now been deleted. 
> 
> Please note that it takes some time for network profiles to stop appearing in internet searches and this is beyond our control. Any contributions you might have made to the forum have been anonymized. You may still receive email communications from us - if you wish to unsubscribe from those please use the unsubscribe link at the bottom of every mailing. 
> 
> If you change your mind at any time you are very welcome to rejoin the network at https://namati.org/network. We will always be glad to have you back! 
> 
> Sincerely yours, <br>
> Tobias Eigen<br>
> Community Manager


### Case 5: Contact has passed away

1. Update wordpress profile to [community+unreachable@namati.org](mailto:community+unreachable@namati.org)
2. Disable all email notifications in discourse
3. Delete contact from mailchimp
4. Update sales network invitation field to &ldquo;Former member (deceased)&rdquo;
5. Post new topic about the tragic news, or ask someone who knows the deceased member well to post new topic (can be received by email and posted)
6. Time permitting and as needed/appropriate:
7. Update network champion for organization
8. Draft and send out tribute via Namati mailer (if NGC member or close partner)
9. Post replies to discourse post as appropriate

<small class="documentation-source">Source: [https://community.namati.org/t/steps-to-take-when-a-member-email-address-stops-working/41156](https://community.namati.org/t/steps-to-take-when-a-member-email-address-stops-working/41156)</small>
