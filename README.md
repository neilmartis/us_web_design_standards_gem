**This `gem` has been deprecated.**

# [`us_web_design_standards`](https://rubygems.org/gems/us_web_design_standards): U.S. Web Design Standards style assets gem

Provides the style assets from the [U.S. Web Design
Standards](https://playbook.cio.gov/designstandards) as a [Ruby
Gem](https://rubygems.org/).

Provides plugins for use with [Jekyll](https://jekyllrb.com/)-based web sites.
Other frameworks may be supported in the future.

## Usage

This gem is compatible with Jekyll. If you are looking for a Ruby on Rails
version, please see [the USWDS Rails gem](https://github.com/18F/uswds-rails-gem).

### Jekyll

In your [`Gemfile`](http://bundler.io/gemfile.html), include the following:

```ruby
group :jekyll_plugins do
  gem 'us_web_design_standards'
end
```

Add a `uswds.scss` file to your project in the asset directory of your
choosing that contains at least the following:

```scss
---
---

@import "us_web_design_standards";
```

Integrate the generated `uswds.css` file and its styles into your project's
layouts and templates, build the site per usual, and observe the results.

## Development

First, choose a Jekyll site you'd like to use to view the impact of your
updates and clone its repository; then clone this repository into the same
parent directory. For example, to use the 18F Guides Template:

```shell
$ git clone git@github.com:18F/guides-template.git
$ git clone git@github.com:18F/us_web_design_standards_gem.git
```

In the `Gemfile` of the Jekyll site's repository, include the following:

```ruby
group :jekyll_plugins do
  gem 'us_web_design_standards', :path => '../us_web_design_standards_gem'
end
```

## Public domain

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0
>dedication. By submitting a pull request, you are agreeing to comply
>with this waiver of copyright interest.
