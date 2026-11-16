# Ep 1: What is MQTT?

🎥 Video: *coming soon* on [@TinkerHour](https://www.youtube.com/@TinkerHour)

## You'll need
- [Docker](https://docs.docker.com/get-docker/), or Mosquitto installed locally
- A terminal

## Run a broker

```bash
docker network create tinker
docker run -it --rm --name broker --network tinker -p 1883:1883 eclipse-mosquitto:2 mosquitto -c /mosquitto-no-auth.conf
```

## Subscribe (terminal 1)

```bash
docker run -it --rm --network tinker eclipse-mosquitto:2 mosquitto_sub -h broker -t "tinker/#" -v
```

## Publish (terminal 2)

```bash
docker run -it --rm --network tinker eclipse-mosquitto:2 mosquitto_pub -h broker -t "tinker/hello" -m "It's Tinker Hour!"
```

You should see `tinker/hello It's Tinker Hour!` appear in terminal 1. 🎉
