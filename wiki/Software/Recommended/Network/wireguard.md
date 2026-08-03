## WireGuard

A fast, modern, and auditable VPN.

WireGuard encrypts traffic between peers with state-of-the-art cryptography, built into the Linux kernel.

### A kernel module, not a daemon

WireGuard lives in the kernel. There is no userspace daemon to crash, restart, or configure.

The interface is a network device; configuring it is done with `wg` and standard tools like `ip`.

### The whole config is a keypair

```
[Interface]
PrivateKey = ...
Address = 10.0.0.1/24

[Peer]
PublicKey = ...
AllowedIPs = 0.0.0.0/0
Endpoint = vpn.example.com:51820
```

That is the entire setup. No X.509 certificates, no plugin system, no enterprise UI.

### Minimal and auditable

WireGuard is a few thousand lines of C, designed to be audited by one person.

It follows the philosophy of this wiki: the smallest thing that does the job, done carefully.

### Composable

`wg-quick` is a thin shell script over `wg` and `ip`, easy to read and adapt.

WireGuard composes with the rest of a Unix system instead of hiding behind its own layer.
