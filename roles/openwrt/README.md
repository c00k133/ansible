[OpenWRT](https://openwrt.org/) routers do not have Python installed by default, meaning that Ansible cannot be used to its full potential.
As I want to have my router running on minimal software, I have to ensure each task can run without Python.
This include setting `gather_facts` to `false` in the corresponding playbook for this role.

### References

AdBlock configuration options:
> [github.com/openwrt/packages/blob/master/net/adblock/files/README.md#adblock-config-options](https://github.com/openwrt/packages/blob/master/net/adblock/files/README.md#adblock-config-options)
