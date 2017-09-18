# TPC 2018 - Glasgow

## Libraries used

* [Bootstrap 4][bootstrap]
* [jQuery 3.2.1][jquery]
* [Popper.js][popper-js]

[bootstrap]: http://getbootstrap.com/ "Bootstrap Homepage"
[jquery]: https://jquery.com/ "jQuery Homepage"
[popper-js]: https://popper.js.org/ "Popper.js Homepage"

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
