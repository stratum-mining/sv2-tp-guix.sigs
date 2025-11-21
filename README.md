Guix signature attestations for https://github.com/stratum-mining/sv2-tp releases.

For the general process see:
- https://github.com/bitcoin-core/guix.sigs
- https://github.com/stratum-mining/sv2-tp/tree/master/contrib/guix


```sh
contrib/guix/guix-build
```

And then for codesigning:

```sh
contrib/guix/guix-codesign
```

The detached signatures are here: https://github.com/stratum-mining/sv2-tp-guix.sigs

Attestation:

```sh
env SIGNER=Sjors NO_SIGN=1 ./contrib/guix/guix-attest
```
