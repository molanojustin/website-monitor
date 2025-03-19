# Website Monitor

Set `.env` variables. The following are required:
- PUSHOVER_TOKEN: str - An app specific token generated by Pushover.
- PUSHOVER_USER: str - A user specific key generated by Pushover.
- SOURCE_URL: str - The url the program should monitor.

Additional optional environment variables:
- CHECK_INTERVAL: int - The number of seconds between each check. Defaults to 60. 
- DEBUG_MODE: bool - Will print the hash values into the console. Defaults to False
- PULSE_CHECK: bool - Notifies less frequently and will give a push notification at a set interval. Defaults to False

Once the variables are set, run `monitor.py` and the program will run until a website change is detected.