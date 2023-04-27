# Chanster Blog

This is a repo of [chanster.github.io](https://chanster.github.io). Theme is based on [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) by [Cotes](https://github.com/cotes2020).

## Development

`serve` will watch for changes by default.

```
docker run -it --rm \
    --env JEKYLL_ENV=production \
    --volume="$PWD:/srv/jekyll" \
    --publish 4000:4000 \
    jekyll/jekyll \
    jekyll serve
```

## Build

GitHub Action will build and deploy on github.io, if testing locally, better to use the `serve` option.

```
docker run -it --rm \
    --env JEKYLL_ENV=production \
    --volume="$PWD:/srv/jekyll" \
    jekyll/jekyll \
    jekyll build
```
