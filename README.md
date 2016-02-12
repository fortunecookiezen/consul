# consul

#### Table of Contents

1. [Description](#description)
1. [Setup - The basics of getting started with consul](#setup)
    * [What consul affects](#what-consul-affects)
    * [Setup requirements](#setup-requirements)
    * [Beginning with consul](#beginning-with-consul)
1. [Usage - Configuration options and additional functionality](#usage)
1. [Reference - An under-the-hood peek at what the module is doing and how](#reference)
1. [Limitations - OS compatibility, etc.](#limitations)
1. [Development - Guide for contributing to the module](#development)

## Description

This puppet module installs [Hashicorp Consul](https://consul.io)

## Setup

### What consul affects 

This module simply installs consul with a sane default configuration. To configure
consul, please consult the [Consul documentation](https://www.consul.io/intro/getting-started/install.html)

### Setup Requirements 

The one caution I would warn, is that this modules bundles the rpms for the installation with the module.
Yes, that is a definite anti-pattern. I acknowledge that. It will be fixed in later releases of this

### Beginning with consul


After installation, to access the consul service, type: `curl localhost:8500/v1/catalog/nodes`

The consul web ui will be available at http://127.0.0.1:8500/ui

## Usage

This section is where you describe how to customize, configure, and do the
fancy stuff with your module here. It's especially helpful if you include usage
examples and code samples for doing things with your module.

## Reference

Here, include a complete list of your module's classes, types, providers,
facts, along with the parameters for each. Users refer to this section (thus
the name "Reference") to find specific details; most users don't read it per
se.

## Limitations

This is a hack, let's be real. I know the best answer would be to put the rpms
into a yum repo, but I don't have one for the initial release. Also, this has only
been tested on RHEL/Centos 6

## Development

This module lives at https://github.com/fortunecookiezen/consul

## Release Notes/Contributors/Etc. 

v.0.1.0	Feb 12 2016 - Initial Release
