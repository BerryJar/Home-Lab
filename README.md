
## Home Lab Introduction

Welcome to the documentation of my home lab. This repository is the hub for my infrastructure, experiments, and projects. Hopefully you find it interesting and informative.

## Whose Lab Is It Really?

This project started as a collaboration between me and a good friend, Ben. He has a background in Computer Science, I just generally liked playing with computers and being the go to "IT Guy" for friends and family. We decided after some
discussion to begin a lab together. Ben provides the hardware, I am tasked with engineering the implementation however we both generally help out with both sides when we can.

## Technical Details

#### Hardware Specifications

The first iteration of the first server, Crisco, was a Lenovo Thinkcentre m910q. The current iteration of Crisco is a custom build. Both iterations run Unraid. The specifications are as follows:

- Motherboard: ASUSTeK STRIX Z270H GAMING
- CPU: Intel Core i7-7700k @ 4.20Ghz
- RAM: 64GB DDR4
- GPU: NVIDIA Tesla P40

The second server, Jojoba, is a [Minisforum MS-01](https://store.minisforum.com/products/minisforum-ms-01) running Proxmox. The specifications are as follows:

- Motherboard: We believe the motherboard is custom by Minisforum.
- CPU: Intel Core i9-13900H
- RAM: 96GB DDR5-SODIMM

We also have a few random machines and services hosted on Google Cloud Platform.

## Software Specifications

#### Networking

To provide remote access to our services, we used [Tailscale](https://tailscale.com/). Tailscale is an easy-to-use VPN service that is built on Wireguard. 


#### Virtualization and Containerization

For containers, we use [Docker](https://www.docker.com/).

For virtual machines, we use QEMU provisioned with the Proxmox Web UI. 

#### Services

##### Crisco

- Actual
- Appsmith
- Grafana
- Heimdall
- MageAI
- PgAdmin
- PostgreSQL
- Teamspeak 3

##### Canola (Jojoba VM)

- Actual
- Vikunja
- Heimdall
- Postgres
- Plane

##### Google Cloud Platform

- GitLab

## Going Forward

We have a loose plan in place for where we'd like to be with our servers. We will be migrating most services from Crisco to Jojoba. Crisco will remain as the AI server, and Jojoba will host everything else. Once we have the migration 
complete, we will be migrating services to Kubernetes. We would then be aiming to create a physical cluster, with a node at Ben's house, and a node at my house. A self-hosted home security and home automation system will come in the future.



