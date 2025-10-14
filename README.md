Guix signature attestations for https://github.com/Sjors/sv2-tp releases.

For the general process see:
- https://github.com/bitcoin-core/guix.sigs
- https://github.com/Sjors/sv2-tp/tree/master/contrib/guix


```sh
contrib/guix/guix-build
```

And then for codesigning:

Since there's currently no Windows release, it's necessary to enumerate all hosts:

```sh
HOSTS="arm64-apple-darwin x86_64-apple-darwin" contrib/guix/guix-codesign
```

The detached signatures are here: https://github.com/Sjors/sv2-tp-guix.sigs

Attestation:

```sh
env SIGNER=Sjors NO_SIGN=1 ./contrib/guix/guix-attest
```
