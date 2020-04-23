# NU CoSMO

This repo serves as the homepage for Northeastern University's CS Mentoring Club (CoSMO).

## Usage

This site uses the static site generator `Jeykll`. Please install it in order to develop this website.

Jekyll works by taking a template that you write and generating HTML and CSS from it. If you're trying to modify the site,
you'll want to start at the root level files:
  - index.html
  - eboard.html
  - mentors.html
  - contact.html

You'll notice they contain lines like `{% include mentors.html %}`. That line imports sections of the site from the `_includes` directory.
You'll likely find what you need to change in there. `_includes` may in turn access yaml data files in `_data`. Finally, to change CSS,
look at the `assets` folder.

After editing these files, run the Jekyll command to generate the site (e.g. `jekyll serve`). You'll be able to navigate to a local version
of the new website in your browser, likely at `localhost:4000`.

*Important: When you're ready to commit your changes to master, be sure to include the `_site` folder. This is the code that Jekyll generates.*

 Note that you should never need to edit the `_site` folder yourself.

## Adding events

Events added to `_/data/upcoming.yaml` will be reflected on the front page of the site. Please follow the following format:

```yaml
- title: Linux CLI "WarGames" Workshop
  dateTime: 4/1/19 @ 7pm
  fbID: 2222960244431411  # The end part of a facebook.com/events/XXXX URL
  description:   <p>
      Linux is an operating system that sits the at core of much of the technology we interact with daily.
      Linux is free, secure, and having to work with it on the job is unavoidable.
    </p>
    <p>
      Join CoSMO this Monday as we demystify the linux command line!We'll start the workshop by reviewing some common and good-to-know linux commands.
      We'll then move into Bandit "War Games", an interactive shell-based game that reinforces basic commands
      and teaches security concepts.
      </p>
```

Multiple events can be listed, and will be rendered in the order they exist in the data file.

## Acknowledgments
This site is based of off the Jekyll theme Compass. See here for more info: https://excentris.github.io/compass/
