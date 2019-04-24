# heroku-buildpack-qgtunnel

**:warning: This is an unofficial Heroku Buildpack.**

Heroku Buildpack to install [qgtunnel](https://devcenter.heroku.com/articles/quotaguardstatic#setting-up-socks5-tunnel)

`qgtunnel` allows you to create a local tunnels of SOCKS5 on heroku dyno. It's related to [Heroku Add-on QuotaGuard Static](https://devcenter.heroku.com/articles/quotaguardstatic).

## How it works

Installs from official [qgtunnel binary](https://s3.amazonaws.com/quotaguard/qgtunnel-latest.tar.gz) on Amazon S3.

`qgtunnel` installation ends in `/app/bin` directory.

## Configure from CLI

```
$ heroku buildpacks:add https://github.com/masutaka/heroku-buildpack-qgtunnel.git
```

## Configure from app manifest

```json
{
  "buildpacks": [
    {
      "url": "https://github.com/masutaka/heroku-buildpack-qgtunnel.git"
    }
  ]
}
```
