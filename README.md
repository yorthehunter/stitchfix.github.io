# Doom Patrol
Stitch Fix Engineering & Analytics jobs site

![Doom Patrol](http://images2.wikia.nocookie.net/__cb20091015054813/marvel_dc/images/5/55/Doom_Patrol_008.jpg "DOOM PATROL")


> The Doom Patrol is a superhero team...

Enough said.

# Get Started
If you don't have jekyll 1.0+ installed yet run:

```
gem install jekyll
```

Once jekyll is installed, grab the repo from github:

```
git clone git@github.com:stitchfix/doom-patrol.git 
```

## Rake tasks

### rake dev
```
jekyll serve --watch
```

Sets up jekyll server for dev on port 4000. Site is regenerated everytime you save a file. 
NOTE: Changing _config.yml will require a restart of the jekyll server to see changes.
To restart server, go to terminal tab that server is running in then press
    ctrl+C ⇧  enter

### rake sass
```
sass --watch _sass:css 
```

### rake clean
```
rm -rf _site  
```
You'll want to kill the server before you run this. Removes _site folder. Note, _site
should not be commited and pushed...ever.


### rake minify
```
sass --watch _sass:css --style compressed
```
Outputs minified css from the compiler.
