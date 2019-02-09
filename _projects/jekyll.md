---
title: Jekyll on GitLab
layout: page
permalink: /:collection/:name
---

- Read about [Jekyll on GitLab](https://jekyllrb.com/docs/github-pages/)
- Read about [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/)
- Clone ["Jekyll-Uno"](https://github.com/joshgerdes/jekyll-uno.git) project

```shell
git clone https://github.com/joshgerdes/jekyll-uno.git
```

- Rename to `username`.gitlab.io
- Change directory to `username`.gitlab.io
- Install bundler and jekyll

```shell
sudo gem install bundler jekyll
```
- Install gems with bundle

```shell
bundle install
```

- Serve webpage

```shell
bundle exec jekyll serve
```

- [Configure](https://jekyllrb.com/docs/configuration/) Jekyll
- [Get started with GitLab CI/CD](https://gitlab.com/help/ci/quick_start/README)
- [Creating and Tweaking GitLab CI/CD](https://docs.gitlab.com/ee/user/project/pages/getting_started_part_four.html)
 - [.gitlab-ci.yml](https://gitlab.com/jekyll-themes/default-bundler/blob/master/.gitlab-ci.yml)
- [GitLab Pages custom domains and SSL/TLS Certificates](https://docs.gitlab.com/ee/user/project/pages/getting_started_part_three.html)
