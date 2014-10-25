# DocBuilds

[DocBuilds.com](http://www.docbuilds.com), a leaderboard of top open-source static documentation generators.

## Contributing

Missing a documentation generator here? Just fork the repo and add your generator
as a `<name>.md` in the `source/projects` folder.

Make sure to follow the following rules:

*   **Static Documentation Generation:** The focus is on documentation, not on static site generators. Those are already covered by [StaticGen](http://www.staticgen.com).
*   **Open Source:** The generator must have a public repository on Github that we can link to and pull in stats from.
*   **Stick to the format:** Fill out all the same fields as the other static site generators in `source/projects`.
*   **Short description:** Keep all the details for the body text, keep the description for the overview page short and sweet.

## Running locally

DocBuilds is built with Middleman. To install and run locally:

    git clone https://github.com/plaindocs/docbuilds.git
    cd staticgen
    bundle install
    bundle exec middleman

You'll run into GitHub's API limits very quickly if you just do this. To avoid this we recommend you create a Github API token with permissions to access public repositories and Gist.

Then create a Gist with a single file `data.json` with an empty javascript object literal as content: {}

Then set these environment variables before running middleman:

    export GITHUB_TOKEN=YOUR_TOKEN
    export GIST_ID=ID_OF_YOUR_GIST

Then middleman will use the Gist you specified to archive stats (stars, forks and issues) for the repositories.

## Plaindocs

DocBuilds is built and maintained by [Plaindocs](https://www.plaindocs.com), creator of quality API documentation.

## License
This project is licensed under the [MIT license](http://opensource.org/licenses/MIT).
