# couchdb17-centos7

You absolutely need to install these ASAP if you are still running 1.6.x. It has 2 CVEs listed with remote code execution.
https://www.cvedetails.com/cve/CVE-2017-12636/

https://www.cvedetails.com/cve/CVE-2017-12635/

1. Add `erlang-solutions.repo` to `/etc/yum.repos.d`
```dosini
[erlang-solutions]
name=Centos $releasever - $basearch - Erlang Solutions
baseurl=http://packages.erlang-solutions.com/rpm/centos/$releasever/$basearch
gpgcheck=0
gpgkey=http://packages.erlang-solutions.com/debian/erlang_solutions.asc
enabled=1```

2. Install Erlang 20.2 

3. Install files in the release section. These files were rebuilt from Fedora 28 packages.
