# github-docker-package-example

Example to use container registory of GitHub Packages (docker.pkg.github.com), not GitHub container registry (ghcr.io)

Be sure that docker.pkg.github.com cannot upload using personal access token like ghcr.io. **You have to setup GitHub Actions, and can access only from GitHub Actions.**

GitHub Actions setup
---------------------

See [GitHub Actions setting](./.github/workflows/docker.yml). This action uploads the following container:

```
docker pull docker.pkg.github.com/termoshtt/github-docker-package-example/hello-world:latest
```
