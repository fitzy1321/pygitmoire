# PyGitmoire

Riffing on Grimoire ...

I want an automated way of backing up my github repos, without spending a lot of time configuring a git repo and mirrors.

I'm thinking of using these technologies:

- Ansible, for server setup
  - need to figure out secret key management
- Python
  - PyGithub, maintained python package, automate all the github restapi stuff
  - automate pulling the latest from repos, syncing with local rpi server repos
- Cron Job?
  - Run python script at midnight or something

cron job example, run at midnight everyday

```py
0 0 * * * python3 home/pi/test.py
```
