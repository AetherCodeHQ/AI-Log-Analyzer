# AI Log Analyzer

Intelligent log analysis powered by AI - detect anomalies, extract insights, and visualize log patterns.

[![Go Version](https://img.shields.io/badge/Go-1.23%2B-00ADD8?style=flat&logo=go)](https://go.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![CI](https://github.com/Qyroxen/ai-log-analyzer/actions/workflows/ci.yml/badge.svg)](https://github.com/Qyroxen/ai-log-analyzer/actions/workflows/ci.yml)

> Intelligent log analysis powered by AI - detect anomalies, extract insights, and visualize log patterns.

## What is it?

AI Log Analyzer is a command-line tool built with Go that helps developers intelligent log analysis powered by ai - detect anomalies, extract insights, and visualize log patterns. It's designed to be fast, reliable, and easy to use.

## Why?

Every developer needs ai log analyzer — but existing tools are either too complex, too slow, or require cloud dependencies. We built AI Log Analyzer to be:
- **Fast** — Written in Go for maximum performance
- **Offline** — No cloud dependencies, your data stays on your machine
- **Simple** — Clean CLI interface with sensible defaults
- **Extensible** — Easy to customize and integrate into your workflow

## Features

- **AI-powered anomaly detection** — AI-powered anomaly detection
- **Pattern recognition across log files** — Pattern recognition across log files
- **Real-time log streaming analysis** — Real-time log streaming analysis
- **Export insights to JSON/CSV** — Export insights to JSON/CSV
- **Support for common log formats** — Support for common log formats
- **Customizable alert rules** — Customizable alert rules

## Quick Start

### Prerequisites

- Go 1.23 or later

### Install

```bash
# Install with go install
go install github.com/Qyroxen/ai-log-analyzer@latest

# Or build from source
git clone https://github.com/Qyroxen/ai-log-analyzer.git
cd ai-log-analyzer
go build -o ai-log-analyzer .
```

### Usage

```bash
# Basic usage
.ai-log-analyzer --help

# Example
./ai-log-analyzer analyze --path /var/log --output insights.json
```

## Output

```
AI Log Analyzer v1.0.0

Scanning...

✓ Analysis complete
✓ Results ready

{
  "status": "success",
  "results": [...]
}
```

## Configuration

Create a `.config.yaml` file in your project root:

```yaml
# Configuration options
verbose: true
output: json
timeout: 30s
```

## CLI Flags

```
ai log analyzer [command]

Flags:
  --path string      Target path (default ".")
  --format string    Output format: json, text (default "text")
  --verbose          Enable verbose output
  --config string    Config file path
  --output string    Output file path
```

## Examples

### Basic Example

```bash
.ai-log-analyzer --path ./src
```

### Advanced Example

```bash
.ai-log-analyzer --path ./src --format json --output report.json --verbose
```

### CI/CD Integration

```yaml
# .github/workflows/ci.yml
- name: Run AI Log Analyzer
  run: |
    go install github.com/Qyroxen/ai-log-analyzer@latest
    ai-log-analyzer --path . --format json --output report.json
```

## Documentation

- [Getting Started](docs/getting-started.md)
- [Configuration](docs/configuration.md)
- [API Reference](docs/api-reference.md)
- [Examples](examples/)
- [Contributing](CONTRIBUTING.md)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**Qyroxen** - [GitHub](https://github.com/Qyroxen)

---

**Found this useful?** Give it a ⭐ on GitHub!
