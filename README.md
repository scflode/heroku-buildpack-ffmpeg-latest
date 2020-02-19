# heroku-buildpack-ffmpeg-latest

>This fork provides the possiblity to define a `FFMPEG_VERSION` config variable in Heroku or Dokku to fetch a
specific version. See https://www.johnvansickle.com/ffmpeg/old-releases/ for a list of available ones.

>*Note*: This buildpack does currently not create a merged `.release` file. Please put it before the ones that do.

A Heroku buildpack for ffmpeg that always downloads the latest [static build](http://johnvansickle.com/ffmpeg/).
Unlike other build packs, I never compile anything.

## Usage

Add the following to your `.buildpacks`:

```
https://github.com/scflode/heroku-buildpack-ffmpeg-latest.git
```

Or run the following from the heroku command line:

```
heroku buildpacks:add https://github.com/scflode/heroku-buildpack-ffmpeg-latest.git
```
