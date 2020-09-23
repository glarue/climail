```
usage: climail [-h] -sadd SERVER_ADDRESS -fadd FROM_ADDRESS -pw PASSWORD -tadd
               TO_ADDRESS [-p PORT] [-s [SUBJECT]] [-b [BODY]] [--ID ID]
               [--no_host_tag] [--suffix_tag]

Send an email over SSL from the command line

optional arguments:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  Port to use on email server (default: 587)
  -s [SUBJECT], --subject [SUBJECT]
                        A subject line for the email, wrapped in single quotes
                        ('') (default: None)
  -b [BODY], --body [BODY]
                        The body of the email, wrapped in single quotes ('')
                        (default: None)
  --ID ID               Arbitrary string to include in host tag (if present)
                        (default: None)
  --no_host_tag         disable host tag (time/server string) in subject
                        (default: False)
  --suffix_tag          place host tag at end of subject rather than beginning
                        (default: False)

required named arguments:
  -sadd SERVER_ADDRESS, --server_address SERVER_ADDRESS
                        Server address for outgoing email using the SSL
                        protocol (default: None)
  -fadd FROM_ADDRESS, --from_address FROM_ADDRESS
                        Full email address from which to send email (default:
                        None)
  -pw PASSWORD, --password PASSWORD
                        Account password for the 'from' address. Wrap in
                        single quotes ('') (default: None)
  -tadd TO_ADDRESS, --to_address TO_ADDRESS
                        Destination email address (default: None)
```
