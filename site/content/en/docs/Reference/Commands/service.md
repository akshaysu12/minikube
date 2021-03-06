---
title: "service"
linkTitle: "service"
weight: 1
date: 2019-08-01
description: >
  Gets the Kubernetes URL(s) for the specified service in your local cluster
---

### Overview

Gets the Kubernetes URL(s) for the specified service in your local cluster. In the case of multiple URLs they will be printed one at a time.

### Usage

```
minikube service [flags] SERVICE
```

### Subcommands

- **list**: Lists the URLs for the services in your local cluster

### Options

```
      --format string      Format to output service URL in. This format will be applied to each url individually and they will be printed one at a time. (default "http://{{.IP}}:{{.Port}}")
  -h, --help               help for service
      --https              Open the service URL with https instead of http
      --interval int       The time interval for each check that wait performs in seconds (default 6)
  -n, --namespace string   The service namespace (default "default")
      --url                Display the kubernetes service URL in the CLI instead of opening it in the default browser
      --wait int           Amount of time to wait for a service in seconds (default 20)
```

### Options inherited from parent commands

```
      --alsologtostderr                  log to standard error as well as files
  -b, --bootstrapper string              The name of the cluster bootstrapper that will set up the kubernetes cluster. (default "kubeadm")
      --log_backtrace_at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log_dir string                   If non-empty, write log files in this directory
      --logtostderr                      log to standard error instead of files
  -p, --profile string                   The name of the minikube VM being used. This can be set to allow having multiple instances of minikube independently. (default "minikube")
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          log level for V logs
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```

## minikube service list

Lists the URLs for the services in your local cluster

```
minikube service list [flags]
```

### Options

```
  -h, --help               help for list
  -n, --namespace string   The services namespace
```

