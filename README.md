# pool-share-counter

> share · accept · stub

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

Pool share counter — subscribe, scan, accept.

## Features

- Default algorithm ethash
- Role: pool
- Stratum job queue with stub notify/submit
- CPU backend with SHA-256 work loop
- Watchdog-style controller and share counter

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd pool-share-counter
python -m pip install -e .
python -m poolshare --help
```

## CLI Usage

```bash
poolshare bench --rounds 32
# Hash a stub job locally

poolshare status
# Print controller snapshot

poolshare submit --nonce 1
# Record a stub share
```

## Project Structure

```
poolshare/
  stratum/     client + job queue
  algo/        hasher
  device/      CPU backend
  core/        controller
  cli.py
tests/
```

## Configuration

See `poolshare/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `algo` | `ethash` | Hash algorithm id |
| `threads` | `1` | Worker count |
| `pool` | `stratum+tcp://localhost:3333` | Stub pool URL |

## Tests

```bash
python -m pytest -q
```

## Background

Pool Python hops name the repo pool-share-counter.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![pool](https://img.shields.io/badge/pool-111827?style=flat-square) ![share](https://img.shields.io/badge/share-111827?style=flat-square) ![counter](https://img.shields.io/badge/counter-111827?style=flat-square) ![pool-share-counter](https://img.shields.io/badge/pool%20share%20counter-111827?style=flat-square) ![miner](https://img.shields.io/badge/miner-111827?style=flat-square) ![cryptominer](https://img.shields.io/badge/cryptominer-111827?style=flat-square) ![stratum](https://img.shields.io/badge/stratum-111827?style=flat-square) ![mining](https://img.shields.io/badge/mining-111827?style=flat-square)

`pool` `share` `counter` `pool-share-counter` `miner` `cryptominer` `stratum` `mining` `hashrate` `mining-pool` `open-source` `python`

Search: pool-share-counter · share · accept · stub · Pool share counter — subscribe, scan, accept.

---

<sub>Pool share counter — subscribe, scan, accept.</sub>
