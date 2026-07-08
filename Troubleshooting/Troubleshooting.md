# Troubleshooting



##### \# Day 4:

###### Issue 1: Unable to connect to EC2 instance through host PC Terminal using SSH.

* Symptoms: When trying to establish connection to my EC2 instance using SSH, PowerShell replies with 'ssh: connect to host <publicIP> port 22: Connection timed out'.
* Cause: Instance status checks not confirmed before SSH.
* Fix: Restarted EC2 instance, and on reboot, all 3 status checks were passed.
* Result: SSH connection to EC2 instance through PowerShell is established - remote access to server is confirmed.

