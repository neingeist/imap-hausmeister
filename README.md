In today's edition of overt pedantry: The IMAP hausmeister

e.g. check or make sure
* that some folders do not exist
* or are empty
* contain only certain mails
* contain only unread mails
* that mails in "Sent" are moved to "Archives"

For now this is just the script I use for this purpose. If there's more interest
in this, I might turn this into something configurable or a library.

Example
-------
~~~
if 'INBOX.Archive' in folders():
    print('INBOX.Archive should not exist')
if number('INBOX.Archives') > 0:
    print('INBOX.Archives should be empty')
~~~
