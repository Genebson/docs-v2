---
title: influx remote delete
description: Delete remote InfluxDB connections used for replicating data.
menu:
  influxdb_2_1_ref:
    name: influx remote delete
    parent: influx remote
weight: 102
influxdb/v2.1/tags: [write, replication]
related:
  - /influxdb/v2.1/reference/cli/influx/replication
---

The `influx remote delete` command delete an existing remote InfluxDB connection used for replication.

## Usage
```
influx remote delete [command options] [arguments...]
```

## Flags

| Flag |                   | Description                                                           | Input type | {{< cli/mapped >}}    |
| :--- | :---------------- | :-------------------------------------------------------------------- | :--------: | :-------------------- |
| `-i` | `--id`            | Remote connection ID to delete                                        |            |                       |
|      | `--host`          | InfluxDB HTTP address (default `http://localhost:8086`)               |   string   | `INFLUX_HOST`         |
|      | `--skip-verify`   | Skip TLS certificate verification                                     |            | `INFLUX_SKIP_VERIFY`  |
|      | `--configs-path`  | Path to `influx` CLI configurations (default `~/.influxdbv2/configs`) |   string   | `INFLUX_CONFIGS_PATH` |
| `-c` | `--active-config` | CLI configuration to use for command                                  |   string   |                       |
|      | `--http-debug`    | Inspect communication with InfluxDB servers                           |   string   |                       |
|      | `--json`          | Output data as JSON (default `false`)                                 |            | `INFLUX_OUTPUT_JSON`  |
|      | `--hide-headers`  | Hide table headers (default `false`)                                  |            | `INFLUX_HIDE_HEADERS` |
| `-t` | `--token`         | InfluxDB API token                                                    |   string   | `INFLUX_TOKEN`        |