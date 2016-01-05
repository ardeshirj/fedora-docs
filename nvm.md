# NVM - Node Version Manager

## General:
To install or update run following command
```shell
  # Replace the version below with most recent version
  curl https://raw.githubusercontent.com/creationix/nvm/v0.17.3/install.sh | bash
```

Above script will add the following lines
```shell
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"  # This loads nvm
```
to one of these files:
- ~/.bash_profile
- ~/.zshrc
- ~/.profile

## Install nodejs
```shell
# Show most recent nodejs versions to install
  nvm ls-remote
# Install stable nodejs stable version
  nvm install node
# This will set the node and stable aliases - Example:
  ->       v5.3.0
  node -> stable (-> v5.3.0) (default)
  stable -> 5.3 (-> v5.3.0) (default)
# You can confirm installation:
  node -v
  npm -v
```
## Install npm package
```shell
# To install package locally
  npm install [package-name]
# To setup local package.json for a project
  npm init

# To install package globally
  npm install -g [pacakge-name]
# Full path to global packages:
  ~/.nvm/versions/node/[node-version]/lib
```

## To remove
```shell
rm -rf ~/.nvm
# Also make sure to remove the config values from dot files
```