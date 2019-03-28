# nuCoSMO

This repo serves as the homepage for Northeastern University's CS Mentoring Club (CoSMO).

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
