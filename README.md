# SidraChain Sync Node

A lightweight and easy-to-deploy Docker-based node for synchronizing with the **SidraChain** blockchain. Ideal for developers, validators, or infrastructure operators needing a stable connection to the SidraChain network.

---

## Overview

**SidraChain** is an EVM-compatible, Shariah-compliant blockchain (ChainID: **97453**) designed for decentralized finance without riba (interest), gharar (excessive uncertainty), and non-halal sectors. Leveraging a PoW consensus model, it supports Ethereum-native tooling and aims for ethical, inclusive financial access. Learn more: **[Visit SidraChain Node Portal →](https://node.sldrachain.com)**

This repository provides all you need to run a syncing node using Docker Compose.

---

## Features

- **One-click setup** with Docker Compose  
- **RPC** interface (port 8545) for applications  
- **WebSocket** support (port 8546) for real-time updates  
- **Peer discovery** (enode + ports configured) for full node participation  
- Runs a fully synced node with recommended system requirements

---

## System Requirements

| Component | Requirement |
|-----------|-------------|
| **OS** | Ubuntu 20.04 or later |
| **CPU** | 4+ cores (x86_64) |
| **RAM** | 16 GB recommended |
| **Storage** | 500 GB+ SSD |
| **Network** | 10 Mbps+ bandwidth |
| **Docker** | Version 20.10.0 or newer |

:contentReference[oaicite:1]{index=1}

---

## Quick Start

```bash
# 1. Download the latest node package
wget https://node.sldrachain.com

# 2. Extract and navigate into the directory
tar -xzf node.tar.gz
cd node

# 3. Start the SidraChain node with Docker Compose
docker compose up -d

# 4. Monitor logs
docker compose logs -f
