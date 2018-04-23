---
title: "Using forum as ticket system - so no balls are dropped! :woman_juggling:"
---

# How it works

No balls are dropped when handling correspondence with a ticket system, because each ticket is assigned to someone, is given a priority level and progress status. Everyone knows when a ticket is closed because it is marked as resolved. 

Discourse is not designed explicitly to be used as a ticket system but it works quite well for it! We use the following features: 

- messages - title indicates what ticket is about. members and groups include the people involved. 
- tags - to indicate tickets and their status/priority
- assign - to indicate who is the "owner" of tickets
- reminders - to remind ourselves to follow up on tickets 
- whispers - to discuss amongst ourselves how to handle a ticket
- solved - to indicate that a ticket has been answered (optional) 

We have a tag for #ticket which "unlocks" the priority and status tag groups. These we only use for messages we want to use as tickets so we don't drop the ball. Only one priority and one status tag can be used at once. These tags are not visible to non-moderators and can't be used by them. 

# Using the ticket system

The member support team will continually be checking messages to make sure any that need responses will be made into tickets that are then taken through to resolution on a timely basis. Everyone else should be using the ticket system according to their role, responding quickly when asked to help the process along, and handling any tickets assigned to them. The assigned message list is a great place to check on a regular basis for tickets assigned to you. 

1. Start by **assigning** a message to yourself or someone else, who becomes the "owner" of the ticket and should pursue it until it is given the tag `status-resolved`. Once assigned, don't unassign the ticket without assigning to someone else. Even once resolved, every ticket remains assigned to someone.  
2. Next, use **tags** to turn messages into tickets by adding the `ticket`, `priority` and `status` tags. These are only visible to moderators - see below for explanation of how we use them. Adding tags is done by editing the title of an existing message. Start with the `ticket` tag, which unlocks the ability to also add `status` and `priority` tags. Start typing status and priority into the tags field and it will autocomplete. Just choose the tag you want and you’re done.  As you handle the ticket and move through the process from `status-new` to `status-resolved`, update the tags accordingly. 
3. use **whispers** to bring in other moderators to help with resolving whatever the message or topic is about, and to explain any details in private as needed for future reference. 
4. optionally use **solved** to select a reply that encapsulates the solution/resolution. This is very helpful for future reference. [color=red]**Note:** do not use the solved button on whispered replies as non-moderators cannot see those[/color]
5. use **reminders** when status is set to #status-waiting for reply, to follow up within a reasonable period.  The goal is to resolve topics as quickly as possible and to never drop any balls. 

# Status tags

- #status-new New. Nothing has happened yet. This ticket is available for you to assign to yourself if you want to take it on or to assign to someone else if you think they are a better fit.  

- #status-underway Has been assigned and is currently being worked on.  
 
- #status-triaging Assignee has asked for and is waiting for help with triaging the ticket, to determine the best approach and the best person to do it. 
 
- #status-waiting Has been assigned and the owner has taken action, and is now waiting for a response from the member or someone else. It's a good idea to set a reminder to follow-up in a week or so, depending on the priority. 

- #status-resolved  All done! :rocket: 

- #status-backburner On the backburner. You're not getting anywhere with this ticket or it's fine to take care of this in a few weeks or months from now. Do keep an eye on these tasks and take care of them, even if it means giving up and adding a note to the bottom that you are giving up and move it to #status-resolved. The backburner is not intended to be a graveyard.  

# Priority tags

- [color=red]#priority-immediate Drop everything and do this first.[/color]

- #priority-urgent Do this today, once you've finished the immediate priority tasks and before you take on high and normal priority tasks. 

- #priority-high More important than normal priority tickets, but can probably still wait a few days. 

- #priority-normal Most tickets have this priority. 

- #priority-low Not quite on the backburner but not as important as normal priority tickets.

# Reason tags

- #reason-coreapp 

- #reason-memberprofile

- #reason-orgprofile

- #reason-bademail

- #reason-forumpost     

# Known issues 

- It is possible to use the :mag: advanced search to drill down in messages as well as topics. The bulk admin actions tool (wrench in top right that appears when you select a few messages/topics) is intended for topics so don't use it for messages. [Reported to developers.](https://meta.discourse.org/t/advanced-search-and-admin-bulk-update-options-dont-make-sense-for-messages/53730?u=tobiaseigen) 
- The bulk actions available in message lists is too limiting - all you can do is archive. 
- Admin tags are showing up in the /tags page. 
- minor: when mentioning ticket tags in messages, the count of mentioned messages is zero in the pulldown autocomplete list. Meanwhile, mentioned tickets link to the /tags list. This is because it refers to topics not messages. 
- It's only possible to filter by one tag in message lists, but we want to filter by two tags (priority and status). To do that you have to use advanced search. Not sure what the UX answer is for this to propose - maybe add a second tag pulldown, or the ability to add multiple tags to the pulldown search. 
- It's possible to use ticket tags on topics as well, but it is not possible to hide them from view from anyone but moderators so I'm not sure we want to do that. 
- It's possible to use other tags in messages too, but I'm not yet sure of the implications. 

# Up next

- look into using ticket tags to not drop balls on topics as well as messages 
- look into using other tags (eg. themes, countries) on messages 
- figure out how to bulk add ticket tags to backlog of messages that might need handling/that have been resolved
- email-in to member support team (to start messages via email from community mailbox or staff email mailboxes) 
- staged users (to start messages with email correspondents who are not yet signed up. Can still be supported via this procedure. When they do sign up, they have access to the entire history of messages - as long as they use the same email address).

<small class="documentation-source">Source: [https://community.namati.org/t/using-forum-as-ticket-system-so-no-balls-are-dropped-woman-juggling/41971](https://community.namati.org/t/using-forum-as-ticket-system-so-no-balls-are-dropped-woman-juggling/41971)</small>
