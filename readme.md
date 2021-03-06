# About
This website is my personal sandbox and digital junk drawer. It was compiled using the [Jekyll static-site generator](http://jekyllrb.com).

See it live at: [www.tannerheffner.com](http://www.tannerheffner.com).

# Project Structure
    .
    ├── _includes
    ├── _layouts
    ├── _plugins
    ├── _posts
    ├── _projects
    ├── _sass
    ├── assets
    │   └── js
    └── css

- _includes and _layouts are templates that Jekyll uses to generate layout classes and page styles based on YAML Front Matter.
- _plugins is for any extra plugins used by jekyll. I've added a Gist plugin, so gists can easily be embedded.
- Each project and post get its own .md file in the appropriate folder.
- _sass files are compiled to the main css file in the css folder.
- Any custom or project-specific javascript is loaded on an as-needed basis from assets/js. Project files are stored in subfolders of /assets/.
- Standalone pages (about, blog list, connect, etc) have their own individual .md files in the project root.
- I'm using a modified version of BEM syntax and atomic design to separate my stylesheets. It helps keep selector scope sane, and avoids ugly !importants, @extends, and the like.

# Local Development
Clone the repository.
From the main directory:

    $ jekyll build -w
    $ jekyll serve

Visit localhost:4000 in your browser.

# TO DO
- write walkthrough for the file cabinet
- add audio-reactive stills & video for mike's sounds
  - is it possible to embed processing without using processing.js or p5?
- add short walkthrough about drupal helper classes
- do a project with d3
- atom plugin for css colors in editor gutter
