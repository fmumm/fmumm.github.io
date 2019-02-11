---
title: Jekyll
layout: page
---

### About

- [Jekyll](https://jekyllrb.com) is a blog-aware static site generator in Ruby
  - [GitHub Pages](https://jekyllrb.com/docs/github-pages/)
  - [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/)
- [Get started with GitLab CI/CD](https://gitlab.com/help/ci/quick_start/README)
  - [Creating and Tweaking GitLab CI/CD](https://docs.gitlab.com/ee/user/project/pages/getting_started_part_four.html)
  - [.gitlab-ci.yml](https://gitlab.com/jekyll-themes/default-bundler/blob/master/.gitlab-ci.yml)
- [GitLab Pages custom domains and SSL/TLS Certificates](https://docs.gitlab.com/ee/user/project/pages/getting_started_part_three.html)

### Installation (Ubuntu 18.04)

- [Jekyll on Ubuntu](https://jekyllrb.com/docs/installation/ubuntu/)
  - [Configuration](https://jekyllrb.com/docs/configuration/)

```shell
sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
gem install jekyll bundler
jekyll new test-blog
cd test-blog
bundle exec jekyll serve
```

### Installation (WSL)

- [Windows Subsystem for Linux Installation Guide for Windows 10](https://docs.microsoft.com/en-us/windows/wsl/install-win10)
  - [Ubuntu 18.04](https://aka.ms/wsl-ubuntu-1804)
  - [Install Manual](https://docs.microsoft.com/en-us/windows/wsl/install-manual)

```shell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1804 -OutFile Ubuntu.appx -UseBasicParsing
Add-AppxPackage -Path Ubuntu.appx
wslconfig /list /all
wsl --distribution Ubuntu
```
### Themes (Jekyll-Uno)

- [http://jekyllthemes.org/](http://jekyllthemes.org/)
- [https://jekyllthemes.io/](https://jekyllthemes.io/)
  - [Jekyll-Uno](https://github.com/joshgerdes/jekyll-uno.git) - a minimal, responsive theme for Jekyll based on Uno for Ghost


```shell
git clone https://github.com/joshgerdes/jekyll-uno.git
cd jekyll-uno
bundle install
bundle exec jekyll serve
```
