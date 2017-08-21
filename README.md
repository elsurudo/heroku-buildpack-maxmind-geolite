# Heroku Buildpack MaxMind GeoLite (Legacy)

Buildpack for the free MaxMind GeoLite (Legacy) database packages.

**Note:** If possible, you should be using the newer DB format, and [this buildback](https://github.com/physiovia/heroku-buildpack-maxmind-geolite2) instead.

## Configuration

Add the buildpack:

```
heroku buildpacks:add https://github.com/elsurudo/heroku-buildpack-maxmind-geolite
```

Decide which package (City or Country) you need and set up your environment accordingly:

```
heroku config:add MAXMIND_DB_NAME=City
# or
heroku config:add MAXMIND_DB_NAME=Country
```

Then deploy and start using the database.

## Credits

Copyright (c) 2017 Ernest Surudo

Heavily inspired by https://github.com/physiovia/heroku-buildpack-maxmind-geolite2, which was in turn inspired by https://github.com/mantisadnetwork/heroku-buildpack-maxmind. Check out this buildpack if you're using the paid versions of MaxMind.

This product includes GeoLite data created by MaxMind, available from http://www.maxmind.com.
