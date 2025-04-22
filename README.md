# Jenkins
Building in workspace /var/lib/jenkins/workspace/Hello Jenkins
[Hello Jenkins] $ /bin/sh -xe /tmp/jenkins9832531463361122197.sh
+ mkdir -p /new
mkdir: cannot create directory ‘/new’: Permission denied
Build step 'Execute shell' marked build as failure
Finished: FAILURE

ChatGPT said:
It looks like your Jenkins build is failing due to a permission issue when trying to create the /new directory. Here's a breakdown and how you can fix it:

❌ Problem:
sh
Copy
Edit
mkdir: cannot create directory ‘/new’: Permission denied
You're trying to create a directory directly in the root (/) filesystem, which typically requires root (admin) privileges.

