# Seasick Brewing

To check spelling:

``` sh
cat Seasick-Brewing.md | ispell -p brewing.en_US -l
```

The file `brewing.en_US` contains words not in the standard dictionary that
we need.

``` sh
docker run -v $PWD:/workdir ghcr.io/igorshubovych/markdownlint-cli:latest --disable MD040 -- "*.md"
```
