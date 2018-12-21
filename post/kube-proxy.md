---
title: "Kube Proxy"
date: 2018-12-21T15:02:46+08:00
draft: true
tags: ["proxy", "k8s"]
---


- 每台机器上都运行一个 kube-proxy 服务，它监听 API server 中 service 和 endpoint 的变化情况，并通过 iptables 等来为服务配置负载均衡（仅支持 TCP 和 UDP）。

- kube-proxy 可以运行在物理机上， 也可以通过 static pod 和 daemonset 的方式运行



![proxy](https://raw.github.com/chase-cheng/resource/master/images/mysql.jpeg)