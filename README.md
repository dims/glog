# glog

This repo contains a package that exposes an API subset of the [glog](https://github.com/golang/glog) package.
All logging state delivered to this package is shunted to the global [klog logger](https://github.com/dims/klog).

This package makes it so we can intercept the calls to glog and redirect them to zap and thus produce
a consistent log for our processes.

This repository was forked from https://github.com/istio/glog/
