# telemetry-manifests

Minimal OpenTelemetry Collector manifests for pushing metrics to a central server.

## Directories
- `linux-hostmetrics` — Host-only metrics (CPU, load, memory, disk, network, filesystem).
- `linux-nvidia-gpu` — Host metrics + NVIDIA GPU metrics via dcgm-exporter.

## Key commands
```sh
docker compose up -d
```

## Optional: site labels
```sh
# Add labels for central querying (example)
export OTEL_RESOURCE_ATTRIBUTES="env=lab,site=lab1,role=compute"
```
