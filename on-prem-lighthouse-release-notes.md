---
layout: page
title: "On-Prem Lighthouse Release Notes"
keywords: portworx, px-enterprise, px-lighthouse, release notes
sidebar: home_sidebar
---

To get access to Portworx PX-Lighthouse docker repository, contact us at support@portworx.com from your company email address.

## Lighthouse 1.1.3 Release notes

In order to use Lighthouse 1.1.3 with authentication, please download and install PX-Enterprise 1.1.2 as well. 

### Key Features

* Support for authenticated etcd2. Refer to [Lighthouse with Secure etcd] (/run-lighthouse-with-secure-etcd.html)

### Known issues

* This version does not support clear alerts. This will be fixed in the upcoming release along with the addition of “Clear All Alerts” capability
* Email server setup with TLS does not work with certificates signed by private CA
* Lighthouse container requires restart, if it has lost connectivity to etcd2

## Lighthouse 1.1.2 Release notes


### Key Fixes

* Handle kvdb access failures and show banner alerts to indicate access issues
* Handle influxDB access timeouts and show banner alerts to indicate access issues
* Improve feedback on Consul and influxDB container restarts
* Fix panics around influx or consul being down and when customer does first login after initial setup
* Fix inability to create new clusters after a node is added to a cluster

### Known issues

* This version does not support clear alerts. This will be fixed in the upcoming 1.1.3 release along with the addition of "Clear All Alerts" capability.

