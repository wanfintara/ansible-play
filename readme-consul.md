# Setup Consul

## Reference

- [Getting Started](https://learn.hashicorp.com/consul/getting-started/install)
- [Deployment Guide](https://learn.hashicorp.com/consul/advanced/day-1-operations/deployment-guide)

> Try __Getting Started__ for the basic understading of consul,
> the __Deployment Guide__ is for setting up in production

## Important

When starting __Deployment Guide__, there are some basic it is better to be know

- Add `username` to `sudo` group

    ```usermod -aG sudo username```

- There are 2 types file format, `.json` and `.hcl` use any one of them

- in __Configure systemd__ section, make sure `User` and `Group` value is correct

- the filename in `consul.d` doesn't really matter, can use any name, but remember consul will load it alphabetically

## Install Consul Ubuntu

- sudo apt-add-repository ppa:ansible/ansible
- sudo apt update
- sudo apt install ansible