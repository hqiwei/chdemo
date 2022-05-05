chdemo
=============

Deploy chdemo to [Heroku](https://www.heroku.com/).

### Getting started

Use this button [![Heroku Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/hqiwei/chdemo)

Or create a Heroku app manually:

```
$ heroku create
$ heroku stack:set container
$ heroku config:set CHISEL_AUTH=user:pass
$ git push heroku main
...
remote: Verifying deploy... done.
To https://git.heroku.com/chdemo.git
 * [new branch]      main -> main
```

Connect your chdemo client:

```
$ chdemo --version
1.7.7
$ chdemo client --keepalive 10s --auth user:pass https://chdemo.herokuapp.com socks
...
2019/02/05 02:16:33 client: Connected (Latency 263.548181ms)
```
