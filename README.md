# lxc-terraform-cloud-agent

A Debian LXC image containing the [Terraform Cloud Agent](https://developer.hashicorp.com/terraform/cloud-docs/agents).

## Configuration

Set the following in `/opt/tfc_agent/.env`

```
TFC_AGENT_TOKEN=your-token
TFC_AGENT_NAME=your-agent-name
```

And restart the service

```
systemctl restart tfc-agent.service
```

## Why?

I run a Home Lab on Proxmox and my preference is to manage CTs rather than a VM or CT running Docker images (with something like Portainer).