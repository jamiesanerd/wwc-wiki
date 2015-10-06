To add new documentation to the wiki, please follow the steps below.

### Adding the wiki remote

All GitHub repositories have a second, hidden repository associated with them: the `wiki` repository. To add files to the wiki, we simply need to push markdown files to this repo.

Add the `wiki` remote to your local repository using the following command:

```bash
git remote add wiki git@github.com:jamiesanerd/wwc-wiki.wiki.git
```

### Deploying to the wiki

Before you add to the `master` branch first pull to see if there are any changes made remotely:

```bash
git pull wiki master
```

Then you can push it to the wiki using:

```bash
git push wiki master
```

_Only the master branch should be pushed to the `wiki` repository, to make sure that experimental changes don't affect the existing wiki!_

For more information use these docs: https://help.github.com/articles/adding-and-editing-wiki-pages-locally/
