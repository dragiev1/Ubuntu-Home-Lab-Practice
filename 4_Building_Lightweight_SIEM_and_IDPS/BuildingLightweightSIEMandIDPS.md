# Building Lightweight SIEM and IDPS

## 1. Setup

Today, we will go through the core components of a modern SIEM and IDPS, install and configure Suricata, configure Promtail and send logs to Loki, query and correlate alerts using LogCLI,
and lastly reflect on the detection pipelin and incidient-response concepts.

### Suricata -- IPS

The purpose of this chapter is to understand an open-source intrusion detection and prevention system that inspects packets and emits alerts. 

The documentation of this technology can be found here:
[https://suricata.io/documentation/
]


### Loki -- Log Database

This is a lightweight log aggregation system. It simply stores logs with helpful labels instead of indicies. 

Loki is our "SIEM-like" backend by centralizing and indexing log data for searching and correlation. 

### Promtail -- Log Shipper

Small agent that tails log files and sends them to Loki  (our backend).

### LogCLI -- Query Tool

Command-line client for Loki queries, helpful for runnning searches, extracting JSON fields, and performing quick analyses. 

### Docker -- Container Platform

Docker is a lightweight virtualization platform that lets you run apps in isolated containers. Essential for allowing multiple developers run tests in development with the exact same environment. 

## 2. Preparing the System

To start, make sure `curl`, `jq`, `unzip`, and `docker` are installed. 




