# Anthropolog

**Anthropolog** is a daily journaling, knowledge-capture, and activity-tracking CLI tool designed specifically for technical professionals — software engineers, sysadmins, DevOps practitioners, SREs, and anyone whose day involves terminals, ideas, experiments, and commands.

It provides a structured way to capture:

* **Daily logs** (what you did today)
* **Notes** (organized by topics, automatically forming documentation)
* **Command history snippets** (searchable, contextual)
* **Search across everything**

```
alog
```

## Features

### Daily Activity Logging

Capture what you worked on throughout the day:

```
alog log "Investigated container startup delays"
```
Automatically timestamps entries and keeps them chronologically organized.

### Topic-Based Notes

```
alog note kubernetes "Kubelet eviction threshold notes"
```

Notes accumulate into topics, which can later be exported as standalone documentation.

### Command History Capture

Store useful command snippets so you can recall them later:

```
alog cmd "journalctl -u docker -f"
```

### Universal Search

Everything logged, noted, or stored becomes searchable through one simple interface:

```
alog search "git rebase"
```

## Installation

```
git clone https://github.com/gmherb/anthropolog
cd anthropolog
make install
```

This will build and install the `alog` binary.

## Usage Overview

### Logging your day

```
alog log "Debugged TLS issue with internal API"
```

### Adding notes to a topic

```
alog note docker-compose "Bind mount quirks on macOS"
```

### Saving useful commands

```
alog cmd "openssl x509 -in cert.pem -text -noout"
```

### Searching everything

```
alog search openssl
```
