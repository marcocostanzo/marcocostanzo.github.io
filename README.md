# Minimal Mistakes remote theme starter

Click [**Use this template**](https://github.com/mmistakes/mm-github-pages-starter/generate) button above for the quickest method of getting started with the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes).

Contains basic configuration to get you a site with:

- Sample posts.
- Sample top navigation.
- Sample author sidebar with social links.
- Sample footer links.
- Paginated home page.
- Archive pages for posts grouped by year, category, and tag.
- Sample about page.
- Sample 404 page.
- Site wide search.

Replace sample content with your own and [configure as necessary](https://mmistakes.github.io/minimal-mistakes/docs/configuration/).

---

## Troubleshooting

If you have a question about using Jekyll, start a discussion on the [Jekyll Forum](https://talk.jekyllrb.com/) or [StackOverflow](https://stackoverflow.com/questions/tagged/jekyll). Other resources:

- [Ruby 101](https://jekyllrb.com/docs/ruby-101/)
- [Setting up a Jekyll site with GitHub Pages](https://jekyllrb.com/docs/github-pages/)
- [Configuring GitHub Metadata](https://github.com/jekyll/github-metadata/blob/master/docs/configuration.md#configuration) to work properly when developing locally and avoid `No GitHub API authentication could be found. Some fields may be missing or have incorrect data.` warnings.

# Usage (Local)

## Setup

Install Ruby Version Manager [rvm](https://rvm.io/rvm/install)

Install Ruby:

```bash
rvm list known #List available ruby versions
rvm install ruby-2.7 #Install latest (change 2.7 with the latest)
rvm --default use ruby-2.7 #Set the installed version as default (change the version)
ruby -v #Check ruby version
```

RVM BUGFIX ruby 3.0 (check if this has been solved) 
https://github.com/rvm/rvm/issues/5209#issuecomment-1140506763
```bash
rvm pkg install openssl
rvm install ruby --with-openssl-dir=/usr/share/rvm/usr
```

Install some dependencies

```bash
sudo apt-get install build-essential zlib1g-dev
```

Optional (?) (Not sure if needed)
```bash
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt install -y nodejs
sudo apt install gcc g++ make
gem update --system
gem -v
gem install jekyll-include-cache
```

Finally, install Jekyll:

```bash
gem install jekyll bundler
gem update #update the gem dep
gem update --system
bundle install
```

## Run

In the project dir:

```bash
bundle exec jekyll serve
```
