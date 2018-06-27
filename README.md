# iCanCode Club Website

This site uses [Gutenberg](https://github.com/Keats/gutenberg).  It is a static site generator similar to Jekyll or Hugo.  

Gutenberg is written in a compiled language, so it requires no extra dependencies and only needs the binary installed and added to a path.

Documentation and installation instructions are available [here](https://www.getgutenberg.io/documentation/getting-started/installation/).

# 1. How do I view the site locally?
After installing Gutenberg and adding it to your path, navigate to its directory with your terminal of choice (works on Win, Mac, Linux, etc.)

Next, run 

```sh
gutenberg serve
```

You should see it spawn a server at [localhost:1111](http://localhost:1111).  Here, you can view the site.  It will also auto-update when changes are made.

# 2. How do I change content?
It depends on what you want to change.  You will find most things in the `content` directory as a `markdown` file.  

If you are looking to change something like a phone number or address, look in the root directory for a file called `config.toml`.

If you need to change some structure of the site, check out the `templates` directory.

> Tip: search for text you want to change in order to easily find its source file.

# 3. Where do I add media?
Use the `static` folder for images, audio files, and other media.  

# 4. Where do I add CSS and JS?
You may also use the `static` folder for JavaScript files.  CSS files are preprocessed from `SASS` and are put in the `sass` directory.

# 5. How do I edit page or site settings?
Please check the front matter (the stuff in-between `+++ ... +++`) in the content folder, or the `config.toml` file.

# 6. How do I push to production?
This site uses Netlify for free hosting.  Pushing to production is as easy as pushing to the master branch of the GitHub repository.  Branches will not be pushed to production.

# 7. I need user-input data, e.g. forums, etc.
You will need to embed that.  Being a static site generator, this code is unable to connect to a database.  At this time, none of those features are required.  You may wish to look at the older Rails implementation if you plan to create new services.

# 8. I need something else
Please check the [Gutenberg](https://www.getgutenberg.io/documentation/getting-started/installation/) documentation for other questions.  If you are completely stumped, email the original developer at alexanderpaullozada [at] gmail.

