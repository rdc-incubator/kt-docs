# 介绍

![](../_media/demo-1.gif)

## 特性

* 直接访问Kubernetes集群

开发者通过KT可以直接连接Kubernetes集群内部网络，在不修改代码的情况下完成本地开发与联调测试

* 转发集群流量到本地

开发者可以将集群中的流量转发到本地，从而使得集群中的其它服务可以联调本地

* 基于SSH的轻量级VPN网络

KT使用shhuttle作为网络连接实现，实现轻量级的SSH VPN网络

* 作为kubectl插件，集成到Kubectl

开发者也可以直接将ktctl集成到kubectl中

## 更新日志

### 0.0.2

* 修复当Namespace启用Istio自动注入后，exchange无法转发请求到本地问题
* exchange命令支持独立运行

### 0.0.1

* 拆分connect与exchaneg子命令，支持多应用转发请求到本地