# Image registry proxy

This repo is based of this https://github.com/rpardini/docker-registry-proxy.
I wanted to use the proxy as a registry and not with the usage of the HTTP_PROXY and HTTPS_PROXY env vars.
Also you do not need to handle certificates as it is only http and should be only used in a internal network.

You can also use the docker pull trough mirror but with this approach you can proxy any repository.

This repo was created to use with a k3s deployment.
Example configuration can be found [here](examples/k3s/registries.yaml).