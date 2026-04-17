# Devops-pay-api-ansible
This project was focused on learning Ansible, running playbooks, adding of roles etc.

Case Scenario - The Ticket
It's Monday morning. You're sipping zobo at your desk and your tech lead drops a message in Slack:
From: Tech Lead
To: You
Subject: New pay-api environment needed by Friday
Morning. We're launching the new pay-api microservice next sprint and we
need a fresh staging environment ready by EOD Friday:
- 2 web nodes (CentOS, running httpd)
- 1 database node (CentOS, MariaDB)
- All three need NTP locked down — audit team is still seeing
timestamp drift in transaction logs and it's failing compliance.
Oh, and one of the web nodes has to be Ubuntu. Don't ask. Long story.
Make it reproducible. We'll be spinning up the same thing for QA next month.
Thanks.

Your tech lead is back with one more request:
Hey, great work on the web servers! Now I need you to set up the
database node too. Install MariaDB on pay-db01, start it, and deploy
a status page on the web servers that also shows the database info.
Same rules: make it reproducible, use variables, and don't restart
anything unless you have to.

To fully run project: ssh into control server public IP, cd into pay-api-setup and run `ansible-playbook pay-api.yaml`
