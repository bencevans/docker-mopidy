# docker-mopidy

Docker image for the [Mopidy](https://www.mopidy.com/) music service with [Mopify](https://github.com/dirkgroenen/mopidy-mopify#readme).

## Build

```
docker build -t bencevans/mopidy:latest .
```


## Run

```
docker run -v /dev/snd:/dev/snd --privileged -p 6680:6680 -v /usr/share/sounds/alsa/:/var/media -d bencevans/mopidy:latest
```
