mutt2omnifocus
==============
mutt2omnifocus is a tiny ruby script to create OmniFocus tasks from 
messages in mutt.  
Actually it will read any RFC compliant message on stdin that rubys mail gem 
can decoded.

I created this so that I could easily convert mails into task to aid GTD. 
The subject of the e-mail is used for the name of the task, and the content 
of the email converted to text and stored in the note. 

Usage
=====

Clone the repo and go a bundle 

Use the following in your mutt configuration files:

    macro index,pager \cL "<pipe-message>pathto/mutt2omnifocus<enter>" \
        "Create OmniFocus task from message"
