Before deployment please check this checklist:
    1. Don't expose any credentials in seetings.py create .env folder and fetch data from there.
    2. In settings.py make the following changes
        DEBUG = False
        Allowed_host = <Add the ip adress/ DNS address>
         