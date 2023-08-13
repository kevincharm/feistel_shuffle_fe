# Feistel Shuffle (Fe Edition)

Generalised Feistel cipher (format-preserving encryption) implemented in [Fe](https://fe-lang.org).

JS Spec: https://github.com/kevincharm/gfc-fpe

## Usage

```fe
use feistel_shuffle::encrypt

// Shuffle an NFT token id `x`
let x: u256 = 0
let domain: u256 = 10_000
let random_seed: u256 = 0xc7a5d737993796fccf3e283c501bbe000e61d1129dbf31a712d75d1de219ce47
let rounds: u256 = 6
let x_prime: u256 = 1 + encrypt(x - 1, domain, random_seed, rounds)
```
