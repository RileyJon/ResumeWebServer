# Resume Web Server

This repository contains the files necessary to host and serve your resume as a website.

## Overview

In today's digital age, having an online presence for your resume is crucial. This repository provides a simple yet effective solution for hosting your resume as a website. 

## Documentation

Create a git_pull.sh in your Root
```bash
#!/bin/bash

# Change directory to your Git repository
cd ../var/www/ResumeWebServer/

# Perform a Git pull
git pull

```
Set Script to Executable
```bash
chmod +x git_pull.sh
```

Set Cron Job

```bash
crontab -e
0 0 * * * /root/git_pull.sh >/dev/null 2>&1
```
