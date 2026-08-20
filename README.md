# AI Log Analyzer

![CI](https://github.com/Qyroxen/AI-Log-Analyzer/actions/workflows/ci.yml/badge.svg) ![Go](https://img.shields.io/badge/Go-1.23+-00ADD8?style=flat&logo=go) ![License](https://img.shields.io/badge/License-MIT-yellow.svg) ![Stars](https://img.shields.io/github/stars/Qyroxen/AI-Log-Analyzer?style=social)

> Analyze logs with AI - find issues before they become problems

[![Star Badge](https://img.shields.io/github/stars/Qyroxen/AI-Log-Analyzer?style=social)](https://github.com/Qyroxen/AI-Log-Analyzer/stargazers)

## What is it?

AI Log Analyzer reads your log files and identifies patterns, anomalies, and potential issues using machine learning.

## Why should you care?

Logs contain valuable insights but are hard to analyze manually. Let AI find the needle in the haystack.

## Demo

```bash
./ai-log-analyzer analyze --path /var/log/app.log
```

**Output:**
```
Log Analysis Report:
  - 1,247 errors detected
  - Top issue: Connection timeout (342 occurrences)
  - Anomaly: Memory spike at 02:30 AM
```

## Features

- Real-time log monitoring
- Anomaly detection
- Pattern recognition
- Alert generation
- Export to Prometheus/Grafana

## Quick Start

```bash
# Install
git clone https://github.com/Qyroxen/AI-Log-Analyzer.git
cd AI-Log-Analyzer
go build -o ai-log-analyzer .

# Run
./ai-log-analyzer --path /var/log/app.log
```

## CLI Flags

| Flag | Description | Default |
|------|-------------|---------|
| `--path` | Log file or directory | `.` |
| `--watch` | Real-time monitoring | `false` |
| `--alert` | Alert webhook URL | `none` |
| `--export` | Export format (prometheus, json) | `json` |

## Examples

# Analyze a log file
./ai-log-analyzer analyze --path /var/log/app.log

# Real-time monitoring
./ai-log-analyzer analyze --path /var/log/app.log --watch

# Export to Prometheus
./ai-log-analyzer analyze --path ./logs --export prometheus

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <a href="https://github.com/Qyroxen/AI-Log-Analyzer/stargazers">
    <img src="https://img.shields.io/github/stars/Qyroxen/AI-Log-Analyzer?style=social" alt="Star this repo">
  </a>
  <a href="https://github.com/Qyroxen/AI-Log-Analyzer/network/members">
    <img src="https://img.shields.io/github/forks/Qyroxen/AI-Log-Analyzer?style=social" alt="Fork this repo">
  </a>
  <a href="https://github.com/Qyroxen/AI-Log-Analyzer/issues">
    <img src="https://img.shields.io/github/issues/Qyroxen/AI-Log-Analyzer" alt="Issues">
  </a>
</p>
