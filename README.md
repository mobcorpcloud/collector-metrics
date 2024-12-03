# Metrics Collector

A lightweight metrics collector written in Go for system monitoring and metrics reporting.

## Getting started

### Pre-requisites

- Go 1.16 or later
- Linux/macOS operating system

### Installation

```bash
go get github.com/mobcorpcloud/collector-metrics
```

### Configuration

The collector accepts the following environment variables:

```
BACKEND_URL=https://your-metrics-backend.com
COLLECTION_INTERVAL=60  # In seconds
API_KEY=your-api-key    # Optional
```

### Running the collector

```bash
metrics-collector
```

## Metrics collected

The collector gathers the following system metrics:

- System metrics
  - CPU usage percentage
  - Load average (1, 5, 15 minutes)
  - Memory usage (total, used, free)
- Network metrics
  - Bytes received
  - Bytes transmitted
- Disk metrics
  - Usage per mountpoint
  - IO operations

## Development

### Building from source

```bash
git clone github.com/mobcorpcloud/collector-metrics 
cd collector-metrics 
go build
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - see LICENSE file for details