# Valet Install


* Open Terminal (command + space + "Terminal")

### Homebrew
* Test if Homebrew is installed  via Terminal `brew -v`
* Install Homebrew via Terminal `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
or
* Update Homebrew via Terminal `brew update`

### PHP

Via Terminal `brew install php`

### MySQL

* Via Terminal `brew install mysql@5.7`
* Via Terminal `brew services start mysql@5.7`

### Composer
* Via Terminal `cd ~` (~ = alt + n)
* Via Terminal 
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
* Via Terminal `echo 'export PATH="$PATH:$HOME/.composer/vendor/bin"' >> ~/.bashrc`

### Valet

* Download via Terminal `php composer.phar global require laravel/valet`
* Install via Terminal `valet install`
* Via Terminal `mkdir ~/Sites`
* Via Terminal `cd ~/Sites`
* Via Terminal `valet park`
