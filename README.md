# Torbit
A stateless, local cryptographic tool for standard BIP39/BIP32 space mapping and ledger auditing.

## 🚀 Live Preview
Run the stateless client directly via GitHub Pages:
👉 https://btctorbit.github.io/torbit

## 🔒 Security Posture
- **Pure Client-Side**: No backend servers, no analytics trackers, zero data telemetry.
- **Stateless Operation**: All cryptographic calculations occur completely within your local browser memory instance.
- **Production Edition Available**: The public version runs on Testnet parameters. For unminified, zero-dependency Mainnet production sources with advanced key-shuffling components, check the unlock anchor on the live page.

---

## 📡 Escalation Routing
For mainnet license delivery failures, invoice verification mismatches, or PGP-encrypted technical custom integrations, route your cryptographic payload to:
👉 `btctorbit@protonmail.com`

---

## 📂 Source Architecture
The core functionality operates entirely as a zero-dependency, monolithic pure-JavaScript cryptographic engine. Users auditing the script pipeline can trace each layered module within the distribution file sequentially according to its execution order:

```text
<script>
├── buffer@5.7.1.js        # Raw byte array management, low-level hex encoding/decoding, and endianness handling
├── ripemd160@0.2.0.js     # Pure-JS RIPEMD-160 (Paul Johnston / CryptocoinJS Legacy Edition)
├── sha256@1.1.7.js        # Native SHA-256 Engine (Fedor Indutny / hash.js Monolithic Variant)
├── sha512@2.4.11.js       # Simulative 64-bit SHA-512 Engine (Dominic Tarr / sha.js Variant)
├── bs58check@3.0.1.js     # Base58Check encoding layer for legacy and nested script address checksum structures
├── bech32@2.0.0.js        # Bech32/Bech32m encoding layer for native SegWit (P2WPKH) and Taproot (P2TR) layouts
├── ecc.js                 # Low-level elliptic curve (secp256k1) math, point validation, and keypair operations
├── bip39@3.0.0.js         # Mnemonic entropy decoding, PBKDF2 key stretching, and English wordlist mapping
├── bip32@4.0.0.js         # Hierarchical Deterministic (HD) framework supporting extended keys (xprv/xpub) and paths
└── torbit.js              # Main application orchestration layer. [Notice: This public instance deploys minified runtime logic; unminified offline production sources must be deployed locally via the offline anchor package.]
```

## 📄 License
This project is released under the ISC License.

ISC License

Copyright (c) 2026 Torbit contributors

Permission to use, copy, modify, and distribute this software for any purpose
with or without fee is hereby granted, provided that the above copyright notice
and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHORS DISCLAIM ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHORS BE LIABLE
FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION
OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
