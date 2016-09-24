# keep-contributing
make your contributing full

### Why
Do you want your github account to look like [this](https://github.com/yyx990803)?

### Usage
Fork and clone this repo.  
It is better to clone this repo to a continuously running server.  
Add this line to your crontab.
```
0 0 * * * cd /root/keep-contributing && date | cat >> test && git commit -a -m 'daily contributing' && git push origin master >> /var/log/crontab/keep-contributing.log 2>&1
```

You can adjust the path and frequence. Make sure you have configged the global git user.
```
git config --global user.name=sample
git config --global user.email=sample@sample.com
```

Have fun!

