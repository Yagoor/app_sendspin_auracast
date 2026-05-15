# Sendspin Auracast

Sendspin Auracast is a Home Assistant app that starts the `sendspin-auracast` service with user-configurable stream and transport settings.

## Configuration

- `music_assistant_url`: The URL of the music assistant stream.
- `transport`: The transport method for the Auracast device, for example `serial:/dev/ttyACM0,1000000`.
- `extra_args`: Additional arguments passed to `sendspin-auracast`.
- `name`: The name of the Auracast transmitter or service.

## Defaults

The default configuration values are defined in `config.yaml`.

## Supported architectures

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
