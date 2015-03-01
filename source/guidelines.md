---
title: Guidelines
layout: page
---

# Guidelines

Everybody is welcome to contribute to DocBuilds, just fork the [Github repo](https://github.com/plaindocs/docbuilds) and send a pull request.

Each documentation generator is a markdown file in the `source/projects` directory.

Pull requests adding new documentation generators should abide by the following guidelines:

*   **Documentation Generation:** The focus is on documentation, not on static site generators. Those are already covered by [StaticGen](http://www.staticgen.com). Equally hosted documentation solutions are not relevant.
*   **Open Source:** The generator must be released under an open source license.
*   **Accessible on GitHub:** The generator must have a public repository on Github that we can link to and pull in stats from.
*   **Stick to the format:** Fill out all the same fields as the other static documentation generators in `source/projects`.

Many static documentation generators support different template engines. Don't list them all in the template field, just the one(s) used by default. Feel free to go into more details in the body text. There is also no need to list many example sites.
