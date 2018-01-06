## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/doxic/doxic.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/doxic/doxic.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

# My way

https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/
http://jmcglone.com/guides/github-pages/
https://jekyllrb.com/docs/quickstart/
https://x-team.com/blog/build-a-free-website-with-jekyll-and-github-pages/
https://yous.be/whiteglass/about/
https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/

sudo apt-get install libcurl4-openssl-dev

## Setup in WSL
Jekyll on Windows | jekyll: https://jekyllrb.com/docs/windows/

Run Bush on Windows and update repo and packages `sudo apt-get update -y && sudo apt-get upgrade -y`

Install ruby from Brightbox rep. Additionally, we need libcurl -> libcurl4-openssl-dev

```
sudo apt-add-repository ppa:brightbox/ruby-ng
sudo apt-get update
sudo apt-get install -y ruby2.3 ruby2.3-dev build-essential libcurl4-openssl-dev
```

update Ruby gems `sudo gem update` and install jekyll `sudo gem install jekyll bundler`

Check if Jekyll installed properly by running `jekyll -v`

## creating a new site

To install the Jekyll site into the directory you’re currently in, run `bundle exec jekyll new . --force`

Replace gem "jekyll" with `gem "github-pages", group: :jekyll_plugins`

Run `bundle update` and verify that all gems install properly.

Add `remote_theme: "mmistakes/minimal-mistakes"` to your _config.yml file. Remove any other theme: or remote_theme: entry.
