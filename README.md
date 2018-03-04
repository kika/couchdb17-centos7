# couchdb17-centos7

You absolutely need to install these ASAP if you are still running 1.6.x. It has 2 CVEs listed with remote code execution.
https://www.cvedetails.com/cve/CVE-2017-12636/

https://www.cvedetails.com/cve/CVE-2017-12635/

1. Add `erlang-solutions.repo` to `/etc/yum.repos.d`

2. Install Erlang 20.2 to check that the repo works:
   `yum install -y erlang-erts`

3. Install files in the release section. These files were rebuilt from Fedora 28 packages: https://github.com/kika/couchdb17-centos7/releases/tag/1.0
