# Node-Sass

A containerized version of the none-sass project used to compile SCSS and SASS files to CSS

[Node-Sass Documentation](https://github.com/sass/node-sass)

## Using this image


### Run once while passing in reference to current directory

```
docker run --rm -v `pwd`:/usr/src/app cscheide/node-sass node-sass -r -o css/ sass/
```

### Run in a monitoring fashion while passing in reference to current directory

```
docker run --rm -v `pwd`:/usr/src/app cscheide/node-sass node-sass -rw -o css/ sass/
```


### Running interactively

```
docker run -ti --rm -v `pwd`:/usr/src/app -w /usr/src/app cscheide/node-sass sh
node-sass -o css/ sass/
```
