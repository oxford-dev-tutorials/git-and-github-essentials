# Git Configuration

Git requires a couple of configuration options to be set to work smoothly with GitHub.

To do this, enter these two commands, replacing user name and email address.

These values will be stamped on every commit into a repo so you might want to consider anonymising your email address if you don't want it publicly disclsed.

```sh
git config --global user.name "YOUR-GITHUB-ACCOUNT-NAME"

git config --global user.email "YOUR-GITHUB-ACCOUNT-PRIMARY-EMAIL-ADDRESS"
```

Example:

```sh
git config --global user.name "oxford-dev-tutorials"

git config --global user.email "user@example.com"
```

# To see your current configuration

```sh
git config --global --list
```
