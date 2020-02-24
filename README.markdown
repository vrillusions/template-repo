# Template Repo

Consider adding a [repostatus](https://www.repostatus.org/) tag here.  Such as [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

## Usage

- Create new repo using this as a template
- Add a [LICENSE](LICENSE) file from another repo.  Don't include multiples here since that may appear confusing from a legal standpoint.
- Update this readme file.

## Mkdocs action

If you don't want or need mkdocs integration then remove [publish_docs workflow](.github/workflows/publish_docs.yml).

To setup deployment of documentation using mkdocs and github pages:

- Edit first three lines of [mkdocs.yml](mkdocs.yml).
- Generate a [personal token](https://github.com/settings/tokens) with the `repo` privilege.
- Go to [this repo's secrets page](settings/secrets) and add the above token and call it `PERSONAL_TOKEN`.
- On next push to repo it will create the `gh-pages` branch with generated documentation.
- Go to [this repo's settings page](settings) and enable github pages using the `gh-pages` branch.
