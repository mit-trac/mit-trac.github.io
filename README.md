# TRAC-website

## How to push new code to production

- `ssh -i trac.pem -J CSAIL_USERNAME@jump.csail.mit.edu ubuntu@128.52.128.75`. __Note__ `trac.pem` is the private key. If you don't have it ask Guillaume. You might also have to input your **CSAIL** pasword to access CSAIL network first if you don't have active Kerberos tickets to authenticate you
-  `cd ~/mit-trac.github.io`
- `git pull` (or any git command to pull your code)
- `sudo systemctl restart nginx`
