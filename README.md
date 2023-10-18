# Osuny API

## Installation

Install the gem and add to the application's Gemfile by executing:

    $ bundle add osuny_api

If bundler is not being used to manage dependencies, install the gem by executing:

    $ gem install osuny_api

## Usage

```
osuny = OsunyApi.new  host: 'https://instance.osuny.org',
                      token: 'real_token'

post = {
  migration_identifier: "identifiant-unique"
  title: 'Titre importé'
}
osuny.communication
     .website('real_website_id')
     .post
     .import(post)
```
## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
