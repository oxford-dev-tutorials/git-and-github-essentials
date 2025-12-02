# Git Configuration - User Identification

Git requires a couple of configuration options to be set to work smoothly with GitHub.

To do this, enter these two commands, replacing user name and email address.

These values will be stamped on every commit into a repo so you might want to consider anonymising your email address if you don't want it publicly disclsed.

Open up a Powershell terminal and run these two commands:

```sh
git config --global user.name "oxford-dev-tutorials"

git config --global user.email "user@example.com"

```

# Git Configuration - MacOS / Linux / Windows Compatibility for Long Paths

With some versions of Windows you can run in to problems if you are sharing a repo with MacOS or Linux users.

The first of these is to do with long paths to files.

These problems can be solved by making these two commands

Firstly, open up a Powershell terminal and run these two commands:

The first configures Git for long path lengths

```sh
git config --global core.longpaths true

```

And the second configures Windows for long path lengths:

```powershell
New-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control\FileSystem" -Name "LongPathsEnabled" -Value 1 -PropertyType DWORD -Force
```

# Git Configuration - MacOS / Linux / Windows Compatibility for Compatible line endings

Similarly, you need to configure Git for Windows to ensure it uses the same line endings as MacOS or Linux.

To do this Firstly, open up a Powershell terminal and run this command:

```sh
git config --global core.autocrlf true

```

# To see your current configuration

```sh
git config --global --list
```
