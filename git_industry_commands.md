GIT CONFIGURATION COMMANDS

git config is used to set, view, and manage Git configuration settings such as:

Username

Email

Default editor

Default branch name

Credential helper

SETTING A CONFIGURATION VALUE
SYNTAX
git config [--local | --global | --system] <key> <value>
PURPOSE

---> Used to set/save a configuration value.

EXAMPLE
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
VIEWING A CONFIGURATION VALUE
SYNTAX
git config <key>
PURPOSE

---> Used to view/display a specific configuration value.

EXAMPLE
git config user.name
LISTING ALL CONFIGURATION SETTINGS
SYNTAX
git config --list
PURPOSE

---> Used to display all configuration settings.

EXAMPLE
git config --global --list
REMOVING A CONFIGURATION VALUE
SYNTAX
git config --unset <key>
PURPOSE

---> Used to remove/delete a specific configuration value.

EXAMPLE
git config --global --unset user.name
REMOVING ALL VALUES OF A KEY
SYNTAX
git config --unset-all <key>
PURPOSE
---> Used to remove all values associated with a key.

![GIT CONFIG](screenshots/git_config.png)

REPOSITORY SETUP COMMANDS
GIT INIT
SYNTAX
git init
PURPOSE

---> Create a new Git repository.

EXAMPLE
git init
GIT CLONE
SYNTAX
git clone <repository-url>
PURPOSE

---> Copy an existing remote repository.

EXAMPLE
git clone https://github.com/username/project.git
GIT CLONE --BRANCH
SYNTAX
git clone --branch <branch-name> <repository-url>
PURPOSE

---> Clone a specific branch.

EXAMPLE
git clone --branch develop https://github.com/username/project.git
GIT CLONE --DEPTH
SYNTAX
git clone --depth <number> <repository-url>
PURPOSE

---> Clone with limited commit history (shallow clone).

EXAMPLE
git clone --depth 1 https://github.com/username/project.git

REPOSITORY STATUS AND INSPECTION
git add -p stages part by part not whole
