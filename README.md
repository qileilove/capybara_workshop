# capybara_workshop
## ruby env
### install brew

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
### install rbenv
```
$ brew update
$ brew install rbenv
```
### install ruby
```
# list all available versions:
$ rbenv install -l

# install a Ruby version:
$ rbenv install 2.2.2
# check already install ruby verison
$ rbenv vesions
```
### install bundler
```
$ gem install bundler

```
#### create and edit Gemfile
```
source 'https://rubygems.org'
gem 'capybara'
```
### run bundle install
```
$ bundle install
```
if you met some issue like below
```
Errno::EACCES: Permission denied @ rb_sysopen - /Users/lqi/.rbenv/versions/2.3.0/lib/ruby/gems/2.3.0/gems/nokogiri-1.7.1/.autotest
Using rack-test 0.6.3
Using childprocess 0.6.3
An error occurred while installing nokogiri (1.7.1), and Bundler cannot continue.
Make sure that `gem install nokogiri -v '1.7.1'` succeeds before bundling.
```
- first install xcode-select
```
$ xcode-select --install
```

- second install nokogiri
```
$ sudo gem install nokogiri -v '1.7.1'
```
- third run bundle install again
```
$ bundle install
```
## session1
 install nodejs
  - install nvm

 ```
 $ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash

 ```
 -  The script clones the nvm repository to ~/.nvm and adds the source line to your profile (~/.bash_profile, ~/.zshrc, ~/.profile, or ~/.bashrc).

```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" # This loads nvm
```
- source your (~/.bash_profile, ~/.zshrc, ~/.profile, or ~/.bashrc) file

```
$ source ~/.bashrc
```
- nvm
```
nvm  ls-remote
nvm install v6.0.0
nvm use v6.0.0
```
## install geckodriver
```
$ gem install geckodriver-helper
```
