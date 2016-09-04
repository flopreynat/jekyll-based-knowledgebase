# Jekyll-based Knowledge Base

Inspired by the great Knowledge base made by wisecash
https://github.com/wisecash/wisecash-support

A kind of reset to this KB with a couple of fixes, as I did encounter issue with GraphicsMagick
error: Liquid Exception: ImageMagick/GraphicsMagick is not installed

Only ran this locally fyi. 

Just follow wisecash advices:
I'm adding their instructions below just in case their repo disappears.

Well done Guys, and thanks.

## How to run locally

* Clone this repository to your machine.
* Make sure to have Ruby installed (tested fine on Ruby 2.1.x).
* Install required dependencies with `bundle install`
* Run `jekyll serve`
* Go to [http://localhost:4000/help/](http://localhost:4000/help/)

## How to build in production

This is mostly:

```
cd wisecash-support-clone
bundle exec jekyll build --destination $target_folder -c _config.yml,_private_config.yml
```

Private config is used to avoid leaving it in the public repository. Nothing sensitive but I want to make sure nobody deploys it by mistake, in order to avoid affecting our own typekit quotas.
