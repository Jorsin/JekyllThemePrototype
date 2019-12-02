# jekyll-theme-wand2 

A theme made for the wand website.

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-theme-wand2"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-wand2
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-theme-wand2

## Usage

### Use a layout from theme refer to it in metadata under "layout tag"
```md
---
layout: PREMADE-LAYOUT-NAME`
---
```

### Adding a link to nav bar, modify `_data/navigation.yml` with the format

```yml
- name:(eg People)
  link:(eg /people.html)
```

### Creating a new collection (eg collect/_people)

Modify `_config.yml` with the format

```yml
collections:
     people:
        output: true
     research:
        output: true
     example-collection:
        output: true(determines if each listing will generate a unique page under its url)
```

Create the directory for your new collection inside your collections folder with an underscore at the front of its name. eg `collection/_example-collection`

### Adding a collection dropdown to the nav menu

Make sure your collection's name(in `_config.yml`) is the same as your nav item's name(in `_data/navigation.yml`). Then simply add a drop variable to the navigation item with any value.

eg. (Assuming the _people collection exists with a true output value)
```yml
- name:(eg People)
  link:(eg /people.html)
  drop: yes
```

Beware, dropdown menus will not automatically provide links for mobile users. This must be provided by the nav items landing page.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

