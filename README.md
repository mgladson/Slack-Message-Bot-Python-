# Slack Message Bot Python

This script is intended to be a template to build atop to scrape server log files and/or operating information and alert devOp teams utilizing Slack.

### Requirements:
(1) Slack Channel Webhook

### Linux Deployment Instructions:

After copying the script to the linux server, make the script executable:

```
chmod a+x slackMessageBot.py
```

Then run the script via:

```
./slackMessageBot.py
```

#### Scheduling the Slack Message Bot using `crontab`

Open the servers crontab via:
```
crontab -e
```

Add the following to schedule the Slack Message Bot to send automated messages everyday at midnight:
```
0 0 * * * ./slackMessageBot.py
```
