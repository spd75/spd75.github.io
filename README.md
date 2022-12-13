Syynth Hero by spd75 and cea57.

Please note that we built this website using this jekyll template - this is why it has so many files.

*** IF YOU CANNOT RUN THIS ON YOUR LOCAL MACHINE, go to https://spd75.github.io - you should be able to find our website there. We imagine this is enough for grading,
but if you must run it on your local machine, we provided documentation below on how to run it.***

If you cannot run this, please email spd75@cornell.edu and cea57@cornell.edu. As we said, this website should be visible at https://spd75.github.io as a backup.

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.
