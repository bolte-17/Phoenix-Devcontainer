# Phoenix DevContainer

Contains .devcontainer folder for running a Elixir + Postgres development environment in Docker.

For use with 
* [Visual Studio Code](https://code.visualstudio.com/)
* [Visual Studio Code Remote - Containers](https://code.visualstudio.com/docs/remote/containers) extension
* [Docker](https://www.docker.com/)
* [Elixir](https://elixir-lang.org/)
* [Phoenix Framework](http://www.phoenixframework.org/)

See [microsoft/vscode-dev-containers](https://github.com/microsoft/vscode-dev-containers) for examples of other devcontainer setups.

## Project setup

To create a new project, start by launching the devcontainer in codespaces or locally.

Run `mix phx.new homepage`

Press enter to confirm installing dependencies

    cd homepage

change database hostname from `localhost` to `db` in `test.exs` and `dev.exs`

Finally, launch the server. By default it launches on port 4000 - use the vscode prompt to open a browser on the correct url.

    mix phx.server

To watch and rebuild on changes, use

    iex -S mix phx.server
