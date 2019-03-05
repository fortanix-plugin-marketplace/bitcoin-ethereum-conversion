# Hierarchical Deterministic (HD) wallets Plugin
This plugin derive BIP32 child key (xprv) and convert it into ethereum private key from BIP32 master key
## Initial setup
* import BIP32 master key in SDKMS as secrete object in raw byte format

**Example BIP32 Master Key:** xprv9s21ZrQH143K2yLSxbXemfny4nZroqhpiXEQ1MYx8vo2k7HRXypsWesNr7GkWTuU9CeaW7QeR38NjjaSfZBAAZVkVEpXwEkxLLXP2q1iFUd

## Plugin input and output for key derivation for ethereum
Plugin takes master key-id and derivation path as json input and return child private as response

**Example: Input**

```
{
	"masterKeyId": "fbd70d51-9719-4da8-8f0f-1d304b78df44",
	"path": "m/2"
}
```
**Example: Output**
```
{
  "privateKey": "8806085EE7D0D7DDA5A96CC8B654C5C275980A5DBD462B64F0DBF5FA97C55B77",
}
```

# License

This project is primarily distributed under the terms of the Apache License, Version 2.0 (the "License"), see [LICENSE](./LICENSE) for details.
