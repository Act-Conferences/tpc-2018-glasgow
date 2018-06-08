# TPC 2018 - Glasgow

## Libraries used

* [Bootstrap 4][bootstrap]
* [jQuery 3.2.1][jquery]
* [Popper.js][popper-js]

[bootstrap]: http://getbootstrap.com/ "Bootstrap Homepage"
[jquery]: https://jquery.com/ "jQuery Homepage"
[popper-js]: https://popper.js.org/ "Popper.js Homepage"

## Contributing

This repo holds the configuration for the TPCiG 2018 Act site. The basic idea is, any changes which get to `production` branch, end up deployed on the main live site, and any that are in `master` branch are deployed to the testing environment. This happens every few minutes.

If you are unsure of a change, or want a second pair of eyes on it, commit it to a seperate branch and create a PR for it, and a member of the TPCiG website team will give you a hand with it!

If you are unsure of which branch to work from, create a new branch from `production` and things should work out - at present `master` is just kept in sync when someone remembers.

## Templating Notes

To use internationalisation text, put the text in `{{ ... }}` for it to be translated.

### `make_uri`

Creates a URI with query params.

```
make_uri( 'foo', 'bar',  { id => 42 } ) # /foo/bar?id=42
```

### `make_uri_info`

Creates a full path URI

```
make_uri( 'foo', 'bar',  'id/42' ) # /foo/bar/id/42
```
