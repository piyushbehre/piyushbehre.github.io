
## Install and run this site locally

Install Jekyll
Reference: https://jekyllrb.com/docs/installation/macos/

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install chruby ruby-install xz
ruby-install ruby 3.1.3

echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version

source ~/.zshrc

ruby -v

gem install jekyll

```

### Running locally
```bash
bundle install
bundle exec jekyll serve
```