# Changelog

## 1.1.0 - 2026-06-16

### Added
- `disable_reporting` option to suppress Alloy's anonymous usage telemetry to `stats.grafana.com` via the `--disable-reporting` CLI flag (resolves #4, credit @matheusfaustino in #8)

### Changed
- Telemetry is now disabled by default. Existing installs will stop emitting usage reports on upgrade — set `disable_reporting: false` to opt back in.

## 1.0.0 - 2026-02-21

### Added
- Initial release
- Grafana Alloy v1.13.1
- Systemd journal log shipping to Loki
- Journal field relabeling (unit, hostname, syslog_identifier, transport, container_name, level)
- Debug UI on port 12345
- Configurable Loki URL, log level, and additional config
- Watchdog health check via Alloy's `/-/ready` endpoint
- Support for amd64 and aarch64 architectures
