# AWS Monitoring Stack using Prometheus and Grafana

A hands-on cloud operations project built to monitor Linux server health and infrastructure metrics using AWS EC2, Prometheus, Node Exporter, and Grafana.

This project demonstrates basic infrastructure monitoring, cloud operations support, Linux server visibility, troubleshooting workflow, and dashboard-based monitoring useful for Cloud Support, AWS Support, Infrastructure Support, and Production Support roles.

## Project Overview

In real production and support environments, cloud and infrastructure teams need to monitor server health, system performance, resource utilization, and availability. This project simulates a basic monitoring setup for an AWS-hosted Linux server using open-source monitoring tools.

The goal of this project was to understand how monitoring systems collect server metrics, visualize infrastructure health, and support troubleshooting activities.

## Architecture

The monitoring setup includes:

* AWS EC2 instance as a Linux server
* Node Exporter installed on the monitored Linux server
* Prometheus configured to scrape metrics from Node Exporter
* Grafana connected to Prometheus as a data source
* Grafana dashboard used to visualize CPU, memory, disk, network, and uptime metrics

## Tech Stack

* AWS EC2
* Linux
* Prometheus
* Node Exporter
* Grafana
* Security Groups
* SSH
* Basic Shell Commands

## Monitoring Components

### Node Exporter

Node Exporter was installed on the Linux server to expose system-level metrics such as:

* CPU usage
* Memory usage
* Disk utilization
* Network traffic
* System uptime
* Filesystem metrics

Node Exporter exposes metrics on port `9100`.

### Prometheus

Prometheus was configured to scrape metrics from Node Exporter.

Prometheus was used to:

* Collect infrastructure metrics
* Verify target health
* Query metrics
* Confirm whether the monitored server was reachable

Prometheus runs on port `9090`.

### Grafana

Grafana was used to create dashboard-based visualization for server metrics.

Grafana dashboard helped visualize:

* CPU utilization
* Memory usage
* Disk usage
* Network activity
* Server uptime
* System performance trends

Grafana runs on port `3000`.

## AWS Configuration

AWS EC2 was used to host the monitoring setup.

AWS activities included:

* Launching EC2 Linux instance
* Connecting using SSH
* Configuring security group inbound rules
* Allowing required ports for Prometheus, Grafana, and Node Exporter
* Validating service accessibility through browser and command-line checks

## Ports Used

| Service       | Port |
| ------------- | ---: |
| SSH           |   22 |
| Node Exporter | 9100 |
| Prometheus    | 9090 |
| Grafana       | 3000 |

## Verification Steps

The setup was verified using:

* SSH access to EC2 instance
* System service status checks
* Browser access to Prometheus
* Browser access to Grafana
* Prometheus target health check
* Node Exporter metrics endpoint check
* Grafana dashboard validation

## Skills Demonstrated

* AWS EC2 instance setup
* Linux server configuration
* SSH-based server access
* Security group configuration
* Prometheus setup and basic configuration
* Node Exporter installation
* Grafana dashboard setup
* Infrastructure monitoring
* Resource utilization checks
* Troubleshooting and validation
* Documentation for cloud operations

## Project Summary

This project demonstrates a basic monitoring stack for cloud infrastructure using AWS EC2, Prometheus, Node Exporter, and Grafana. It shows how a cloud support or operations engineer can monitor server health, validate metrics collection, check target availability, and use dashboards for operational visibility.

This project is aligned with Cloud Support Engineer, AWS Support Engineer, Cloud Operations Engineer, Infrastructure Support Engineer, Production Support Engineer, and Junior DevOps Support roles.
