## age

A simple, modern, secure file encryption tool.

age encrypts files with small explicit keys, no configuration options, and UNIX-style composability.

### No configuration

There is no config file, no keyring, no trust model.

Every operation is explicit: generate a key, encrypt to a key, decrypt with a key. The whole state is two short strings.

### Unix-style composability

age reads and writes streams, so it composes with pipes:

```
tar czf - ~/data | age -r age1... > data.tar.gz.age
age -d -i key.txt data.tar.gz.age > data.tar.gz
```

The format is specified at age-encryption.org and has independent implementations.

### Small keys

A public key is 63 characters, small enough to write down or send in chat.

That is the whole interface. There is nothing else to learn.

### Written in Go

A single static binary, audited crypto, no runtime dependencies.
