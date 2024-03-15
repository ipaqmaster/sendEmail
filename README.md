# sendEmail

## About this script

This is a small bash script for testing relaying on mailservers without having to go through the whole 'mail from:' 'rcpt to:' payload process by hand. 


## Arguments

### Required

`-remote`

  The SMTP remote to connect to

`-from`

  The 'From:' address

`-to`

  The 'To:' address

`-subject`

  The 'Subject:' line

`-body`

  The message Body

### Optional

`-attachment`
  Attach a file

`-starttls`
  Use openssl s_client with `-starttls smtp` and `-crlf` for the remote.
  Includes `-verify_return_error` which will error and exit if we cannot verify the remote certificate.
