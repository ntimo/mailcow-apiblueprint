# mailcow-apiblueprint

This project aims to provide the API documention for the [mailcow: dockerized](https://github.com/mailcow/mailcow-dockerized) API.

## How to generate the API documention

To generate the API documention from the apiary.apib file, you can simply execute following one-liner:
```
docker build . -t snowboard:latest
docker run -it --rm -v $PWD:/doc snowboard:latest snowboard html -o output.html -c config.yaml apiary.apib
```
