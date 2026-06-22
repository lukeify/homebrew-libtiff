# Lukeify Libtiff

## Why this tap exists

Homebrew core builds `libtiff` without LERC support. This tap provides an
otherwise identical `libtiff` that adds a `liblerc` dependency and configures
with `--enable-liblerc`, so TIFF and GeoTIFF files using LERC compression can
be read and written. It is intended for raster and DEM workflows where
LERC-compressed GeoTIFFs are common.

## How do I install these formulae?

`brew install lukeify/libtiff/<formula>`

Or `brew tap lukeify/libtiff` and then `brew install <formula>`.

Or, in a `brew bundle` `Brewfile`:

```ruby
tap "lukeify/libtiff"
brew "<formula>"
```

## Documentation

`brew help`, `man brew` or check [Homebrew's documentation](https://docs.brew.sh).
