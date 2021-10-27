# Kube-Vip - Carvel package for Tanzu

This project defines a [Carvel package](https://carvel.dev/kapp-controller/docs/latest/packaging/)
for [Kube-Vip](https://kube-vip.io), a load balancer implementation for
Kubernetes clusters.

Use this package when your underlying infrastructure does not allocate IP addresses
for `LoadBalancer` services.

## How to use it?

This package is part of the
[Tanzu Extra package repository](https://github.com/alexandreroman/tanzu-extra-repo).
Please refer to this page for installation instructions.

Here are the configuration parameters for this package:

| Key                         | Description                     |
|-----------------------------|---------------------------------|
| kubevip.addresses           | Array of IP address ranges      |

Configuration example:

```yaml
kubevip:
  addresses:
  - 192.168.10.100-192.168.10.150
```

## Contribute

Contributions are always welcome!

Feel free to open issues & send PR.

## License

Copyright &copy; 2021 [VMware, Inc. or its affiliates](https://vmware.com).

This project is licensed under the [Apache Software License version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
