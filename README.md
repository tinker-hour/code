<p align="center"><img src="https://github.com/tinker-hour.png" width="96" alt="Tinker Hour logo"></p>

# Tinker Hour: code for every episode

Companion code for the **[Tinker Hour](https://www.youtube.com/@TinkerHour)** YouTube channel.
*One hour. One idea. Finally clear.*

## Layout

```
code/
├── mqtt-from-zero/          📡 MQTT from Zero
├── postgres-finally-clear/  🐘 Postgres, Finally Clear
├── docker-in-an-hour/       🐳 Docker in an Hour
└── quick-tinkers/           ⚡ Short one-off builds
```

Each series folder holds one folder per episode, named `ep01-<slug>`, `ep02-<slug>`, and so on.
Each episode folder has a README with:

1. 🎥 a link to the video
2. 🧰 what you need installed
3. ▶️ the exact commands from the video

## Quick start

```bash
git clone https://github.com/tinker-hour/code.git
cd code/mqtt-from-zero/ep01-what-is-mqtt
```

## License

MIT. Use it, break it, tinker with it.
