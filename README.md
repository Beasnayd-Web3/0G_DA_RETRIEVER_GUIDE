# 0G_DA_RETRIEVER_GUIDE
This repository explains how to put DA Retriever up simply and quickly. Just follow the simple steps outlined here and you'll be good to go!

## Hardware Requirement
|Key|Value|
|:--|:----|
|RAM|8 GB|
|CPU|2 cores|
|BandWidth|100 MBps|

## Installation
```bash
sudo apt-get update
sudo apt-get install cmake build-essential protobuf-compiler
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
git clone https://github.com/0glabs/0g-da-retriever.git
cd 0g-da-retriever
cargo build --release
```

## Configuration

|Field|Value|
|:--|:------|
|log_level|Set log level.|
|grpc_listen_address|Server listening address.|
|eth_rpc_endpoint|JSON RPC node endpoint for the blockchain network.|

## Run
```bash
./target/release/retriever --config ./run/config.toml
```
