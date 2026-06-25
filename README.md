# internet-speed-test

Runs an Ookla Speedtest every 10 minutes and logs download/upload/ping to a CSV.

## How it works
- `./install_speedtest.sh` — downloads the [Ookla Speedtest CLI](https://www.speedtest.net/apps/cli) build into `bin/speedtest`
- `auto_speed_test.py --device` — automated speed test script for 2 hours, runs every 2 mins


## Run a single test manually

```sh
python3 speed_test.py
```



## Reinstall the CLI binary (if `bin/` is missing)

```sh
curl -sL -o /tmp/ookla.tgz https://install.speedtest.net/app/cli/ookla-speedtest-1.2.0-macosx-universal.tgz
mkdir -p bin && tar -xzf /tmp/ookla.tgz -C bin speedtest && chmod +x bin/speedtest
```
