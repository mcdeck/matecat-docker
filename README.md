# MateCat Docker

A dockerized version of MateCat (https://www.matecat.com/) - The CAT tool that works for you.

The documentation left me a bit wondering if it was possible to run this in containters - and it is.

## How to use

```bash
docker compose up -d
```

To upload file for translation, first sign up locally.
After clicking 'Sign Up' from the top-right user icon, enter the apache docker container:

```
docker-compose exec apache /bin/bash
```
and print the mail queue log file:

```
cat storage/log_archive/mail_queue.log
```
This will contain the mail body with the confirmation email link.
