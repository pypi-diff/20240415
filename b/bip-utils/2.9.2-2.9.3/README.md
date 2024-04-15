# Comparing `tmp/bip_utils-2.9.2.tar.gz` & `tmp/bip_utils-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bip_utils-2.9.2.tar", last modified: Wed Mar  6 22:41:20 2024, max compression
+gzip compressed data, was "bip_utils-2.9.3.tar", last modified: Mon Apr 15 19:28:40 2024, max compression
```

## Comparing `bip_utils-2.9.2.tar` & `bip_utils-2.9.3.tar`

### file list

```diff
@@ -1,454 +1,454 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.594919 bip_utils-2.9.2/
--rw-rw-rw-   0        0        0     1085 2024-02-13 10:42:52.000000 bip_utils-2.9.2/LICENSE
--rw-rw-rw-   0        0        0      122 2024-02-13 10:42:52.000000 bip_utils-2.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14324 2024-03-06 22:41:20.589902 bip_utils-2.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    10993 2024-03-06 22:30:03.000000 bip_utils-2.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.069897 bip_utils-2.9.2/bip_utils/
--rw-rw-rw-   0        0        0     8783 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/__init__.py
--rw-rw-rw-   0        0        0       28 2024-03-06 22:36:03.000000 bip_utils-2.9.2/bip_utils/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.442756 bip_utils-2.9.2/bip_utils/addr/
--rw-rw-rw-   0        0        0     7422 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/P2PKH_addr.py
--rw-rw-rw-   0        0        0     6130 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/P2SH_addr.py
--rw-rw-rw-   0        0        0     7404 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/P2TR_addr.py
--rw-rw-rw-   0        0        0     4171 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/P2WPKH_addr.py
--rw-rw-rw-   0        0        0     3486 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/__init__.py
--rw-rw-rw-   0        0        0    18678 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/ada_byron_addr.py
--rw-rw-rw-   0        0        0    11188 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/ada_shelley_addr.py
--rw-rw-rw-   0        0        0     4791 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/addr_dec_utils.py
--rw-rw-rw-   0        0        0     6010 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/addr_key_validator.py
--rw-rw-rw-   0        0        0     4658 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/algo_addr.py
--rw-rw-rw-   0        0        0     4036 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/aptos_addr.py
--rw-rw-rw-   0        0        0     3546 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/atom_addr.py
--rw-rw-rw-   0        0        0     5773 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/avax_addr.py
--rw-rw-rw-   0        0        0     2377 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/bch_addr_converter.py
--rw-rw-rw-   0        0        0     3666 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/egld_addr.py
--rw-rw-rw-   0        0        0     4831 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/eos_addr.py
--rw-rw-rw-   0        0        0     6397 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/ergo_addr.py
--rw-rw-rw-   0        0        0     5229 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/eth_addr.py
--rw-rw-rw-   0        0        0     6871 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/fil_addr.py
--rw-rw-rw-   0        0        0     1881 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/iaddr_decoder.py
--rw-rw-rw-   0        0        0     1982 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/iaddr_encoder.py
--rw-rw-rw-   0        0        0     3824 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/icx_addr.py
--rw-rw-rw-   0        0        0     3756 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/inj_addr.py
--rw-rw-rw-   0        0        0     5459 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/nano_addr.py
--rw-rw-rw-   0        0        0     3416 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/near_addr.py
--rw-rw-rw-   0        0        0     4363 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/neo_addr.py
--rw-rw-rw-   0        0        0     3713 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/okex_addr.py
--rw-rw-rw-   0        0        0     3702 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/one_addr.py
--rw-rw-rw-   0        0        0     3387 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/sol_addr.py
--rw-rw-rw-   0        0        0     6173 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/substrate_addr.py
--rw-rw-rw-   0        0        0     3742 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/sui_addr.py
--rw-rw-rw-   0        0        0     4055 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/trx_addr.py
--rw-rw-rw-   0        0        0     5891 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/xlm_addr.py
--rw-rw-rw-   0        0        0    10588 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/xmr_addr.py
--rw-rw-rw-   0        0        0     3454 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/xrp_addr.py
--rw-rw-rw-   0        0        0     4592 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/xtz_addr.py
--rw-rw-rw-   0        0        0     3807 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/addr/zil_addr.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.446941 bip_utils-2.9.2/bip_utils/algorand/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.510473 bip_utils-2.9.2/bip_utils/algorand/mnemonic/
--rw-rw-rw-   0        0        0      688 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_entropy_generator.py
--rw-rw-rw-   0        0        0     1994 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic.py
--rw-rw-rw-   0        0        0     5234 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     3907 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     4297 2024-02-13 10:42:52.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py
--rw-rw-rw-   0        0        0     3852 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py
--rw-rw-rw-   0        0        0     2144 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py
--rw-rw-rw-   0        0        0     2779 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.542110 bip_utils-2.9.2/bip_utils/base58/
--rw-rw-rw-   0        0        0      219 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/base58/__init__.py
--rw-rw-rw-   0        0        0     7113 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/base58/base58.py
--rw-rw-rw-   0        0        0     1247 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/base58/base58_ex.py
--rw-rw-rw-   0        0        0     5462 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/base58/base58_xmr.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.584957 bip_utils-2.9.2/bip_utils/bech32/
--rw-rw-rw-   0        0        0      287 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bech32/__init__.py
--rw-rw-rw-   0        0        0     6863 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bech32/bch_bech32.py
--rw-rw-rw-   0        0        0     7472 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bech32/bech32.py
--rw-rw-rw-   0        0        0     8249 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bech32/bech32_base.py
--rw-rw-rw-   0        0        0     1247 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bech32/bech32_ex.py
--rw-rw-rw-   0        0        0     6264 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bech32/segwit_bech32.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.588842 bip_utils-2.9.2/bip_utils/bip/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.650186 bip_utils-2.9.2/bip_utils/bip/bip32/
--rw-rw-rw-   0        0        0     1354 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.682954 bip_utils-2.9.2/bip_utils/bip/bip32/base/
--rw-rw-rw-   0        0        0      222 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/base/__init__.py
--rw-rw-rw-   0        0        0    20926 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/base/bip32_base.py
--rw-rw-rw-   0        0        0     3130 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/base/ibip32_key_derivator.py
--rw-rw-rw-   0        0        0     1897 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py
--rw-rw-rw-   0        0        0     1835 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_const.py
--rw-rw-rw-   0        0        0     1318 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_ex.py
--rw-rw-rw-   0        0        0    14058 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_key_data.py
--rw-rw-rw-   0        0        0     2694 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_key_net_ver.py
--rw-rw-rw-   0        0        0    10535 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_key_ser.py
--rw-rw-rw-   0        0        0    15183 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_keys.py
--rw-rw-rw-   0        0        0     7428 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_path.py
--rw-rw-rw-   0        0        0     2346 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/bip32_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.719507 bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/
--rw-rw-rw-   0        0        0      418 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py
--rw-rw-rw-   0        0        0     4850 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py
--rw-rw-rw-   0        0        0     8071 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py
--rw-rw-rw-   0        0        0     4899 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.783824 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/
--rw-rw-rw-   0        0        0      728 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/__init__.py
--rw-rw-rw-   0        0        0     3058 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py
--rw-rw-rw-   0        0        0     1905 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py
--rw-rw-rw-   0        0        0     7631 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py
--rw-rw-rw-   0        0        0     6708 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py
--rw-rw-rw-   0        0        0     3070 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py
--rw-rw-rw-   0        0        0     3066 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.820096 bip_utils-2.9.2/bip_utils/bip/bip38/
--rw-rw-rw-   0        0        0      194 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip38/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip38/bip38.py
--rw-rw-rw-   0        0        0     2665 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip38/bip38_addr.py
--rw-rw-rw-   0        0        0    21343 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip38/bip38_ec.py
--rw-rw-rw-   0        0        0    11382 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip38/bip38_no_ec.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:17.901103 bip_utils-2.9.2/bip_utils/bip/bip39/
--rw-rw-rw-   0        0        0      656 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/__init__.py
--rw-rw-rw-   0        0        0     3376 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_entropy_generator.py
--rw-rw-rw-   0        0        0     3559 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic.py
--rw-rw-rw-   0        0        0     7931 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     3997 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     4021 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_generator.py
--rw-rw-rw-   0        0        0     3809 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_utils.py
--rw-rw-rw-   0        0        0     1850 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_validator.py
--rw-rw-rw-   0        0        0     3486 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/bip39_seed_generator.py
--rw-rw-rw-   0        0        0     2228 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/ibip39_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.220563 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/
--rw-rw-rw-   0        0        0    10240 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/chinese_simplified.txt
--rw-rw-rw-   0        0        0    10240 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/chinese_traditional.txt
--rw-rw-rw-   0        0        0    16993 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/czech.txt
--rw-rw-rw-   0        0        0    15164 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/english.txt
--rw-rw-rw-   0        0        0    18825 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/french.txt
--rw-rw-rw-   0        0        0    18081 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/italian.txt
--rw-rw-rw-   0        0        0    39880 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/korean.txt
--rw-rw-rw-   0        0        0    17719 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/portuguese.txt
--rw-rw-rw-   0        0        0    16044 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/spanish.txt
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.253888 bip_utils-2.9.2/bip_utils/bip/bip44/
--rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip44/__init__.py
--rw-rw-rw-   0        0        0     8919 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip44/bip44.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.291797 bip_utils-2.9.2/bip_utils/bip/bip44_base/
--rw-rw-rw-   0        0        0      235 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip44_base/__init__.py
--rw-rw-rw-   0        0        0    21706 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip44_base/bip44_base.py
--rw-rw-rw-   0        0        0     1255 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip44_base/bip44_base_ex.py
--rw-rw-rw-   0        0        0     7297 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip44_base/bip44_keys.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.308127 bip_utils-2.9.2/bip_utils/bip/bip49/
--rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip49/__init__.py
--rw-rw-rw-   0        0        0     8919 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip49/bip49.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.322275 bip_utils-2.9.2/bip_utils/bip/bip84/
--rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip84/__init__.py
--rw-rw-rw-   0        0        0     8919 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip84/bip84.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.337611 bip_utils-2.9.2/bip_utils/bip/bip86/
--rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip86/__init__.py
--rw-rw-rw-   0        0        0     8917 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/bip86/bip86.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.343844 bip_utils-2.9.2/bip_utils/bip/conf/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.371701 bip_utils-2.9.2/bip_utils/bip/conf/bip44/
--rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip44/__init__.py
--rw-rw-rw-   0        0        0     3565 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip44/bip44_coins.py
--rw-rw-rw-   0        0        0    46079 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip44/bip44_conf.py
--rw-rw-rw-   0        0        0     6996 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip44/bip44_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.403871 bip_utils-2.9.2/bip_utils/bip/conf/bip49/
--rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip49/__init__.py
--rw-rw-rw-   0        0        0     1879 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip49/bip49_coins.py
--rw-rw-rw-   0        0        0    15216 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip49/bip49_conf.py
--rw-rw-rw-   0        0        0     3404 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip49/bip49_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.446620 bip_utils-2.9.2/bip_utils/bip/conf/bip84/
--rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip84/__init__.py
--rw-rw-rw-   0        0        0     1493 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip84/bip84_coins.py
--rw-rw-rw-   0        0        0     4218 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip84/bip84_conf.py
--rw-rw-rw-   0        0        0     2542 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip84/bip84_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.481105 bip_utils-2.9.2/bip_utils/bip/conf/bip86/
--rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip86/__init__.py
--rw-rw-rw-   0        0        0     1439 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip86/bip86_coins.py
--rw-rw-rw-   0        0        0     2963 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip86/bip86_conf.py
--rw-rw-rw-   0        0        0     2420 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/bip86/bip86_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.532862 bip_utils-2.9.2/bip_utils/bip/conf/common/
--rw-rw-rw-   0        0        0      437 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/common/__init__.py
--rw-rw-rw-   0        0        0     4411 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py
--rw-rw-rw-   0        0        0     7042 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/common/bip_coin_conf.py
--rw-rw-rw-   0        0        0     1260 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/common/bip_coins.py
--rw-rw-rw-   0        0        0     1400 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/common/bip_conf_const.py
--rw-rw-rw-   0        0        0     5101 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/bip/conf/common/bip_litecoin_conf.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.579190 bip_utils-2.9.2/bip_utils/brainwallet/
--rw-rw-rw-   0        0        0      216 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/brainwallet/__init__.py
--rw-rw-rw-   0        0        0     4829 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/brainwallet/brainwallet.py
--rw-rw-rw-   0        0        0     5254 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/brainwallet/brainwallet_algo.py
--rw-rw-rw-   0        0        0     2749 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/brainwallet/brainwallet_algo_getter.py
--rw-rw-rw-   0        0        0     1874 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/brainwallet/ibrainwallet_algo.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.585748 bip_utils-2.9.2/bip_utils/cardano/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.625244 bip_utils-2.9.2/bip_utils/cardano/bip32/
--rw-rw-rw-   0        0        0      165 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/bip32/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py
--rw-rw-rw-   0        0        0     4290 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py
--rw-rw-rw-   0        0        0     4426 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py
--rw-rw-rw-   0        0        0     1975 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_icarus_bip32.py
--rw-rw-rw-   0        0        0     4150 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.644089 bip_utils-2.9.2/bip_utils/cardano/byron/
--rw-rw-rw-   0        0        0       77 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/byron/__init__.py
--rw-rw-rw-   0        0        0     9560 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/byron/cardano_byron_legacy.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.659542 bip_utils-2.9.2/bip_utils/cardano/cip1852/
--rw-rw-rw-   0        0        0       55 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/cip1852/__init__.py
--rw-rw-rw-   0        0        0     8713 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/cip1852/cip1852.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.694773 bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/
--rw-rw-rw-   0        0        0      222 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/__init__.py
--rw-rw-rw-   0        0        0     1495 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/cip1852_coins.py
--rw-rw-rw-   0        0        0     3791 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/cip1852_conf.py
--rw-rw-rw-   0        0        0     2652 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.722608 bip_utils-2.9.2/bip_utils/cardano/mnemonic/
--rw-rw-rw-   0        0        0      205 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     2656 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py
--rw-rw-rw-   0        0        0     2513 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.744977 bip_utils-2.9.2/bip_utils/cardano/shelley/
--rw-rw-rw-   0        0        0      182 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/shelley/__init__.py
--rw-rw-rw-   0        0        0     7138 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/shelley/cardano_shelley.py
--rw-rw-rw-   0        0        0     6383 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/cardano/shelley/cardano_shelley_keys.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.764668 bip_utils-2.9.2/bip_utils/coin_conf/
--rw-rw-rw-   0        0        0      106 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/coin_conf/__init__.py
--rw-rw-rw-   0        0        0     2258 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/coin_conf/coin_conf.py
--rw-rw-rw-   0        0        0    23559 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/coin_conf/coins_conf.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.777910 bip_utils-2.9.2/bip_utils/ecc/
--rw-rw-rw-   0        0        0     2046 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.801808 bip_utils-2.9.2/bip_utils/ecc/common/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/common/__init__.py
--rw-rw-rw-   0        0        0     5993 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/common/dummy_point.py
--rw-rw-rw-   0        0        0     6654 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/common/ikeys.py
--rw-rw-rw-   0        0        0     4819 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/common/ipoint.py
--rw-rw-rw-   0        0        0     1315 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/conf.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.825761 bip_utils-2.9.2/bip_utils/ecc/curve/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/curve/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/curve/elliptic_curve.py
--rw-rw-rw-   0        0        0     3135 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/curve/elliptic_curve_getter.py
--rw-rw-rw-   0        0        0     1486 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/curve/elliptic_curve_types.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.830633 bip_utils-2.9.2/bip_utils/ecc/ecdsa/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ecdsa/__init__.py
--rw-rw-rw-   0        0        0     1659 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ecdsa/ecdsa_keys.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.867929 bip_utils-2.9.2/bip_utils/ecc/ed25519/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/__init__.py
--rw-rw-rw-   0        0        0     1828 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519.py
--rw-rw-rw-   0        0        0     1761 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_const.py
--rw-rw-rw-   0        0        0     7409 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_keys.py
--rw-rw-rw-   0        0        0     6701 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_point.py
--rw-rw-rw-   0        0        0     2307 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.876217 bip_utils-2.9.2/bip_utils/ecc/ed25519/lib/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/lib/__init__.py
--rw-rw-rw-   0        0        0    10382 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519/lib/ed25519_lib.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.905868 bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py
--rw-rw-rw-   0        0        0     1571 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py
--rw-rw-rw-   0        0        0     7358 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py
--rw-rw-rw-   0        0        0     1646 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.932179 bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/__init__.py
--rw-rw-rw-   0        0        0     1980 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py
--rw-rw-rw-   0        0        0     1576 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py
--rw-rw-rw-   0        0        0     5303 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py
--rw-rw-rw-   0        0        0     1642 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.966987 bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/__init__.py
--rw-rw-rw-   0        0        0     1980 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero.py
--rw-rw-rw-   0        0        0     1780 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py
--rw-rw-rw-   0        0        0     4174 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py
--rw-rw-rw-   0        0        0     1642 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:18.994195 bip_utils-2.9.2/bip_utils/ecc/nist256p1/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/nist256p1/__init__.py
--rw-rw-rw-   0        0        0     1876 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1.py
--rw-rw-rw-   0        0        0     1606 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1_const.py
--rw-rw-rw-   0        0        0     7231 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1_keys.py
--rw-rw-rw-   0        0        0     6984 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1_point.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.047150 bip_utils-2.9.2/bip_utils/ecc/secp256k1/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/__init__.py
--rw-rw-rw-   0        0        0     1783 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1.py
--rw-rw-rw-   0        0        0     2974 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_const.py
--rw-rw-rw-   0        0        0     7065 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py
--rw-rw-rw-   0        0        0     7301 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py
--rw-rw-rw-   0        0        0     6190 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py
--rw-rw-rw-   0        0        0     7030 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.078501 bip_utils-2.9.2/bip_utils/ecc/sr25519/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/sr25519/__init__.py
--rw-rw-rw-   0        0        0     1828 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519.py
--rw-rw-rw-   0        0        0     1562 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519_const.py
--rw-rw-rw-   0        0        0     6641 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519_keys.py
--rw-rw-rw-   0        0        0     1638 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519_point.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.107552 bip_utils-2.9.2/bip_utils/electrum/
--rw-rw-rw-   0        0        0      136 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/__init__.py
--rw-rw-rw-   0        0        0    10454 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/electrum_v1.py
--rw-rw-rw-   0        0        0    12764 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/electrum_v2.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.190456 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/
--rw-rw-rw-   0        0        0      770 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py
--rw-rw-rw-   0        0        0     2149 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py
--rw-rw-rw-   0        0        0     3685 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     3162 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     4396 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py
--rw-rw-rw-   0        0        0     3890 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py
--rw-rw-rw-   0        0        0     2181 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py
--rw-rw-rw-   0        0        0     3621 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.202098 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/wordlist/
--rw-rw-rw-   0        0        0    12120 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/wordlist/english.txt
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.283003 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/
--rw-rw-rw-   0        0        0      795 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/__init__.py
--rw-rw-rw-   0        0        0     4300 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py
--rw-rw-rw-   0        0        0     2937 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py
--rw-rw-rw-   0        0        0     4499 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     4249 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     5966 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py
--rw-rw-rw-   0        0        0     4266 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py
--rw-rw-rw-   0        0        0     2205 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py
--rw-rw-rw-   0        0        0     3308 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.319578 bip_utils-2.9.2/bip_utils/monero/
--rw-rw-rw-   0        0        0      237 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.355917 bip_utils-2.9.2/bip_utils/monero/conf/
--rw-rw-rw-   0        0        0      256 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/conf/__init__.py
--rw-rw-rw-   0        0        0     3770 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/conf/monero_coin_conf.py
--rw-rw-rw-   0        0        0     1386 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/conf/monero_coins.py
--rw-rw-rw-   0        0        0     1748 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/conf/monero_conf.py
--rw-rw-rw-   0        0        0     2508 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/conf/monero_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.451877 bip_utils-2.9.2/bip_utils/monero/mnemonic/
--rw-rw-rw-   0        0        0      718 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     3191 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_entropy_generator.py
--rw-rw-rw-   0        0        0     3753 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic.py
--rw-rw-rw-   0        0        0     4355 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     6520 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     5109 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_generator.py
--rw-rw-rw-   0        0        0     4600 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_utils.py
--rw-rw-rw-   0        0        0     1872 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_validator.py
--rw-rw-rw-   0        0        0     2545 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.774099 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/
--rw-rw-rw-   0        0        0     8130 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt
--rw-rw-rw-   0        0        0    14346 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/dutch.txt
--rw-rw-rw-   0        0        0    13093 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/english.txt
--rw-rw-rw-   0        0        0    12524 2024-02-13 10:42:53.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/french.txt
--rw-rw-rw-   0        0        0    13960 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/german.txt
--rw-rw-rw-   0        0        0    14400 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/italian.txt
--rw-rw-rw-   0        0        0    21054 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/japanese.txt
--rw-rw-rw-   0        0        0    14765 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/portuguese.txt
--rw-rw-rw-   0        0        0    22376 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/russian.txt
--rw-rw-rw-   0        0        0    12524 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/spanish.txt
--rw-rw-rw-   0        0        0    10682 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/monero.py
--rw-rw-rw-   0        0        0     1244 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/monero_ex.py
--rw-rw-rw-   0        0        0     8202 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/monero_keys.py
--rw-rw-rw-   0        0        0     6050 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/monero/monero_subaddr.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.790627 bip_utils-2.9.2/bip_utils/slip/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.797198 bip_utils-2.9.2/bip_utils/slip/slip173/
--rw-rw-rw-   0        0        0       52 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip173/__init__.py
--rw-rw-rw-   0        0        0     2138 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip173/slip173.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.821751 bip_utils-2.9.2/bip_utils/slip/slip32/
--rw-rw-rw-   0        0        0      227 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip32/__init__.py
--rw-rw-rw-   0        0        0    11214 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip32/slip32.py
--rw-rw-rw-   0        0        0     2085 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip32/slip32_key_net_ver.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.835240 bip_utils-2.9.2/bip_utils/slip/slip44/
--rw-rw-rw-   0        0        0       49 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip44/__init__.py
--rw-rw-rw-   0        0        0     2557 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/slip/slip44/slip44.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.852897 bip_utils-2.9.2/bip_utils/solana/
--rw-rw-rw-   0        0        0       49 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/solana/__init__.py
--rw-rw-rw-   0        0        0     6588 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/solana/spl_token.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.872044 bip_utils-2.9.2/bip_utils/ss58/
--rw-rw-rw-   0        0        0      112 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/ss58/__init__.py
--rw-rw-rw-   0        0        0     5967 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/ss58/ss58.py
--rw-rw-rw-   0        0        0     1243 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/ss58/ss58_ex.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.914162 bip_utils-2.9.2/bip_utils/substrate/
--rw-rw-rw-   0        0        0      343 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.951092 bip_utils-2.9.2/bip_utils/substrate/conf/
--rw-rw-rw-   0        0        0      292 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/conf/__init__.py
--rw-rw-rw-   0        0        0     3031 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/conf/substrate_coin_conf.py
--rw-rw-rw-   0        0        0     1606 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/conf/substrate_coins.py
--rw-rw-rw-   0        0        0     3116 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/conf/substrate_conf.py
--rw-rw-rw-   0        0        0     3179 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/conf/substrate_conf_getter.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.962879 bip_utils-2.9.2/bip_utils/substrate/mnemonic/
--rw-rw-rw-   0        0        0      101 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     2973 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:19.999653 bip_utils-2.9.2/bip_utils/substrate/scale/
--rw-rw-rw-   0        0        0      509 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/scale/__init__.py
--rw-rw-rw-   0        0        0     1628 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_base.py
--rw-rw-rw-   0        0        0     1948 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_bytes.py
--rw-rw-rw-   0        0        0     3082 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_cuint.py
--rw-rw-rw-   0        0        0     4954 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_uint.py
--rw-rw-rw-   0        0        0    12628 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/substrate.py
--rw-rw-rw-   0        0        0     1349 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/substrate_ex.py
--rw-rw-rw-   0        0        0     8752 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/substrate_keys.py
--rw-rw-rw-   0        0        0     9228 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/substrate/substrate_path.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.004954 bip_utils-2.9.2/bip_utils/utils/
--rw-rw-rw-   0        0        0        0 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.011861 bip_utils-2.9.2/bip_utils/utils/conf/
--rw-rw-rw-   0        0        0       55 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/conf/__init__.py
--rw-rw-rw-   0        0        0     1881 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/conf/coin_names.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.123740 bip_utils-2.9.2/bip_utils/utils/crypto/
--rw-rw-rw-   0        0        0      748 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/__init__.py
--rw-rw-rw-   0        0        0     4043 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/aes_ecb.py
--rw-rw-rw-   0        0        0     5189 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/blake2.py
--rw-rw-rw-   0        0        0     3566 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     3048 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/crc.py
--rw-rw-rw-   0        0        0     1944 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/hash160.py
--rw-rw-rw-   0        0        0     3822 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/hmac.py
--rw-rw-rw-   0        0        0     2613 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/pbkdf2.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/ripemd.py
--rw-rw-rw-   0        0        0     2561 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/scrypt.py
--rw-rw-rw-   0        0        0     4836 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/sha2.py
--rw-rw-rw-   0        0        0     3097 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/crypto/sha3.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.200636 bip_utils-2.9.2/bip_utils/utils/misc/
--rw-rw-rw-   0        0        0      501 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/__init__.py
--rw-rw-rw-   0        0        0     3458 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/algo.py
--rw-rw-rw-   0        0        0     4870 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/base32.py
--rw-rw-rw-   0        0        0     3429 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/bit.py
--rw-rw-rw-   0        0        0     6326 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/bytes.py
--rw-rw-rw-   0        0        0     4377 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/cbor_indefinite_len_array.py
--rw-rw-rw-   0        0        0     4924 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/data_bytes.py
--rw-rw-rw-   0        0        0     3512 2024-02-13 10:43:28.000000 bip_utils-2.9.2/bip_utils/utils/misc/integer.py
--rw-rw-rw-   0        0        0     1884 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/misc/string.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.274990 bip_utils-2.9.2/bip_utils/utils/mnemonic/
--rw-rw-rw-   0        0        0      643 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     1976 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/entropy_generator.py
--rw-rw-rw-   0        0        0     3716 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic.py
--rw-rw-rw-   0        0        0     3895 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_decoder_base.py
--rw-rw-rw-   0        0        0     2578 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_encoder_base.py
--rw-rw-rw-   0        0        0     1251 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_ex.py
--rw-rw-rw-   0        0        0    11170 2024-02-13 11:51:20.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_utils.py
--rw-rw-rw-   0        0        0     2860 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_validator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.292699 bip_utils-2.9.2/bip_utils/utils/typing/
--rw-rw-rw-   0        0        0       52 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/typing/__init__.py
--rw-rw-rw-   0        0        0     1372 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/utils/typing/literal.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.319158 bip_utils-2.9.2/bip_utils/wif/
--rw-rw-rw-   0        0        0       70 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/wif/__init__.py
--rw-rw-rw-   0        0        0     5624 2024-02-13 10:42:54.000000 bip_utils-2.9.2/bip_utils/wif/wif.py
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.575865 bip_utils-2.9.2/bip_utils.egg-info/
--rw-rw-rw-   0        0        0    14324 2024-03-06 22:41:16.000000 bip_utils-2.9.2/bip_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14647 2024-03-06 22:41:16.000000 bip_utils-2.9.2/bip_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 22:41:16.000000 bip_utils-2.9.2/bip_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      741 2024-03-06 22:41:16.000000 bip_utils-2.9.2/bip_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-06 22:41:16.000000 bip_utils-2.9.2/bip_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2024-02-13 10:42:55.000000 bip_utils-2.9.2/keywords.txt
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.493993 bip_utils-2.9.2/readme/
--rw-rw-rw-   0        0        0     5128 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/algorand_mnemonic.md
--rw-rw-rw-   0        0        0    17713 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/bip32.md
--rw-rw-rw-   0        0        0     3317 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/bip38.md
--rw-rw-rw-   0        0        0     7775 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/bip39.md
--rw-rw-rw-   0        0        0    20386 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/bip44.md
--rw-rw-rw-   0        0        0     4411 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/brainwallet.md
--rw-rw-rw-   0        0        0    17246 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/cardano.md
--rw-rw-rw-   0        0        0     4701 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/electrum.md
--rw-rw-rw-   0        0        0      767 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/electrum_mnemonic.md
--rw-rw-rw-   0        0        0     4827 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/electrum_v1_mnemonic.md
--rw-rw-rw-   0        0        0     8675 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/electrum_v2_mnemonic.md
--rw-rw-rw-   0        0        0     5035 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/monero.md
--rw-rw-rw-   0        0        0     6792 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/monero_mnemonic.md
--rw-rw-rw-   0        0        0     8496 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/substrate.md
-drwxrwxrwx   0        0        0        0 2024-03-06 22:41:20.559502 bip_utils-2.9.2/readme/utility/
--rw-rw-rw-   0        0        0    16914 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/addr.md
--rw-rw-rw-   0        0        0     1500 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/base58.md
--rw-rw-rw-   0        0        0      613 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/bch_addr_converter.md
--rw-rw-rw-   0        0        0     1242 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/bech32.md
--rw-rw-rw-   0        0        0     1433 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/slip32.md
--rw-rw-rw-   0        0        0      991 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/solana_spl.md
--rw-rw-rw-   0        0        0      441 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/ss58.md
--rw-rw-rw-   0        0        0     1940 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility/wif.md
--rw-rw-rw-   0        0        0      874 2024-02-13 10:42:55.000000 bip_utils-2.9.2/readme/utility_libs.md
--rw-rw-rw-   0        0        0      124 2024-02-13 10:42:55.000000 bip_utils-2.9.2/requirements-dev.txt
--rw-rw-rw-   0        0        0      682 2024-03-06 22:30:03.000000 bip_utils-2.9.2/requirements.txt
--rw-rw-rw-   0        0        0      111 2024-03-06 22:41:20.594919 bip_utils-2.9.2/setup.cfg
--rw-rw-rw-   0        0        0     6021 2024-02-13 10:42:55.000000 bip_utils-2.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:40.060905 bip_utils-2.9.3/
+-rw-rw-rw-   0        0        0     1085 2024-04-14 21:54:11.000000 bip_utils-2.9.3/LICENSE
+-rw-rw-rw-   0        0        0      122 2024-04-14 21:54:11.000000 bip_utils-2.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    13033 2024-04-15 19:28:40.060905 bip_utils-2.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10993 2024-04-14 21:54:11.000000 bip_utils-2.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:37.697910 bip_utils-2.9.3/bip_utils/
+-rw-rw-rw-   0        0        0     8783 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/__init__.py
+-rw-rw-rw-   0        0        0       28 2024-04-02 21:43:38.000000 bip_utils-2.9.3/bip_utils/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:37.966128 bip_utils-2.9.3/bip_utils/addr/
+-rw-rw-rw-   0        0        0     7422 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/P2PKH_addr.py
+-rw-rw-rw-   0        0        0     6130 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/P2SH_addr.py
+-rw-rw-rw-   0        0        0     7404 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/P2TR_addr.py
+-rw-rw-rw-   0        0        0     4171 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/P2WPKH_addr.py
+-rw-rw-rw-   0        0        0     3486 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/__init__.py
+-rw-rw-rw-   0        0        0    18678 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/ada_byron_addr.py
+-rw-rw-rw-   0        0        0    11188 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/ada_shelley_addr.py
+-rw-rw-rw-   0        0        0     4791 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/addr_dec_utils.py
+-rw-rw-rw-   0        0        0     6010 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/addr_key_validator.py
+-rw-rw-rw-   0        0        0     4658 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/algo_addr.py
+-rw-rw-rw-   0        0        0     4220 2024-04-02 21:23:55.000000 bip_utils-2.9.3/bip_utils/addr/aptos_addr.py
+-rw-rw-rw-   0        0        0     3546 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/atom_addr.py
+-rw-rw-rw-   0        0        0     5773 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/avax_addr.py
+-rw-rw-rw-   0        0        0     2377 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/bch_addr_converter.py
+-rw-rw-rw-   0        0        0     3666 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/egld_addr.py
+-rw-rw-rw-   0        0        0     4831 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/eos_addr.py
+-rw-rw-rw-   0        0        0     6397 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/ergo_addr.py
+-rw-rw-rw-   0        0        0     5229 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/eth_addr.py
+-rw-rw-rw-   0        0        0     6871 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/fil_addr.py
+-rw-rw-rw-   0        0        0     1881 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/iaddr_decoder.py
+-rw-rw-rw-   0        0        0     1982 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/iaddr_encoder.py
+-rw-rw-rw-   0        0        0     3824 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/icx_addr.py
+-rw-rw-rw-   0        0        0     3756 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/inj_addr.py
+-rw-rw-rw-   0        0        0     5459 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/nano_addr.py
+-rw-rw-rw-   0        0        0     3416 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/near_addr.py
+-rw-rw-rw-   0        0        0     4363 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/neo_addr.py
+-rw-rw-rw-   0        0        0     3713 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/okex_addr.py
+-rw-rw-rw-   0        0        0     3702 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/one_addr.py
+-rw-rw-rw-   0        0        0     3387 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/sol_addr.py
+-rw-rw-rw-   0        0        0     6173 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/substrate_addr.py
+-rw-rw-rw-   0        0        0     3742 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/sui_addr.py
+-rw-rw-rw-   0        0        0     4055 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/trx_addr.py
+-rw-rw-rw-   0        0        0     5891 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/xlm_addr.py
+-rw-rw-rw-   0        0        0    10588 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/xmr_addr.py
+-rw-rw-rw-   0        0        0     3454 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/xrp_addr.py
+-rw-rw-rw-   0        0        0     4592 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/xtz_addr.py
+-rw-rw-rw-   0        0        0     3807 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/addr/zil_addr.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:37.971435 bip_utils-2.9.3/bip_utils/algorand/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.024632 bip_utils-2.9.3/bip_utils/algorand/mnemonic/
+-rw-rw-rw-   0        0        0      688 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_entropy_generator.py
+-rw-rw-rw-   0        0        0     1994 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic.py
+-rw-rw-rw-   0        0        0     5234 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     3907 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     4297 2024-02-13 10:42:52.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     3852 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2144 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     2779 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.048969 bip_utils-2.9.3/bip_utils/base58/
+-rw-rw-rw-   0        0        0      219 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/base58/__init__.py
+-rw-rw-rw-   0        0        0     7113 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/base58/base58.py
+-rw-rw-rw-   0        0        0     1247 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/base58/base58_ex.py
+-rw-rw-rw-   0        0        0     5462 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/base58/base58_xmr.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.091798 bip_utils-2.9.3/bip_utils/bech32/
+-rw-rw-rw-   0        0        0      287 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bech32/__init__.py
+-rw-rw-rw-   0        0        0     6863 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bech32/bch_bech32.py
+-rw-rw-rw-   0        0        0     7472 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bech32/bech32.py
+-rw-rw-rw-   0        0        0     8249 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bech32/bech32_base.py
+-rw-rw-rw-   0        0        0     1247 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bech32/bech32_ex.py
+-rw-rw-rw-   0        0        0     6264 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bech32/segwit_bech32.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.099615 bip_utils-2.9.3/bip_utils/bip/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.151185 bip_utils-2.9.3/bip_utils/bip/bip32/
+-rw-rw-rw-   0        0        0     1354 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.178872 bip_utils-2.9.3/bip_utils/bip/bip32/base/
+-rw-rw-rw-   0        0        0      222 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/base/__init__.py
+-rw-rw-rw-   0        0        0    20926 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/base/bip32_base.py
+-rw-rw-rw-   0        0        0     3130 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/base/ibip32_key_derivator.py
+-rw-rw-rw-   0        0        0     1897 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py
+-rw-rw-rw-   0        0        0     1835 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_const.py
+-rw-rw-rw-   0        0        0     1318 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_ex.py
+-rw-rw-rw-   0        0        0    14058 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_key_data.py
+-rw-rw-rw-   0        0        0     2694 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_key_net_ver.py
+-rw-rw-rw-   0        0        0    10535 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_key_ser.py
+-rw-rw-rw-   0        0        0    15183 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_keys.py
+-rw-rw-rw-   0        0        0     7428 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_path.py
+-rw-rw-rw-   0        0        0     2346 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/bip32_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.214448 bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/
+-rw-rw-rw-   0        0        0      418 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py
+-rw-rw-rw-   0        0        0     4850 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py
+-rw-rw-rw-   0        0        0     8071 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py
+-rw-rw-rw-   0        0        0     4899 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.260195 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/
+-rw-rw-rw-   0        0        0      728 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/__init__.py
+-rw-rw-rw-   0        0        0     3058 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py
+-rw-rw-rw-   0        0        0     1905 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py
+-rw-rw-rw-   0        0        0     7631 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py
+-rw-rw-rw-   0        0        0     6708 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py
+-rw-rw-rw-   0        0        0     3070 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py
+-rw-rw-rw-   0        0        0     3066 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.285504 bip_utils-2.9.3/bip_utils/bip/bip38/
+-rw-rw-rw-   0        0        0      194 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip38/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip38/bip38.py
+-rw-rw-rw-   0        0        0     2665 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip38/bip38_addr.py
+-rw-rw-rw-   0        0        0    21343 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip38/bip38_ec.py
+-rw-rw-rw-   0        0        0    11382 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip38/bip38_no_ec.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.339071 bip_utils-2.9.3/bip_utils/bip/bip39/
+-rw-rw-rw-   0        0        0      656 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/__init__.py
+-rw-rw-rw-   0        0        0     3376 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_entropy_generator.py
+-rw-rw-rw-   0        0        0     3559 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic.py
+-rw-rw-rw-   0        0        0     7931 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     3997 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     4021 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     3809 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     1850 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     3486 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/bip39_seed_generator.py
+-rw-rw-rw-   0        0        0     2228 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/ibip39_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.441144 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/
+-rw-rw-rw-   0        0        0    10240 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/chinese_simplified.txt
+-rw-rw-rw-   0        0        0    10240 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/chinese_traditional.txt
+-rw-rw-rw-   0        0        0    16993 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/czech.txt
+-rw-rw-rw-   0        0        0    15164 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/english.txt
+-rw-rw-rw-   0        0        0    18825 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/french.txt
+-rw-rw-rw-   0        0        0    18081 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/italian.txt
+-rw-rw-rw-   0        0        0    39880 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/korean.txt
+-rw-rw-rw-   0        0        0    17719 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/portuguese.txt
+-rw-rw-rw-   0        0        0    16044 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/spanish.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.458664 bip_utils-2.9.3/bip_utils/bip/bip44/
+-rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip44/__init__.py
+-rw-rw-rw-   0        0        0     8919 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip44/bip44.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.483007 bip_utils-2.9.3/bip_utils/bip/bip44_base/
+-rw-rw-rw-   0        0        0      235 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip44_base/__init__.py
+-rw-rw-rw-   0        0        0    21706 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip44_base/bip44_base.py
+-rw-rw-rw-   0        0        0     1255 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip44_base/bip44_base_ex.py
+-rw-rw-rw-   0        0        0     7297 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip44_base/bip44_keys.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.490794 bip_utils-2.9.3/bip_utils/bip/bip49/
+-rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip49/__init__.py
+-rw-rw-rw-   0        0        0     8919 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip49/bip49.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.501534 bip_utils-2.9.3/bip_utils/bip/bip84/
+-rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip84/__init__.py
+-rw-rw-rw-   0        0        0     8919 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip84/bip84.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.512241 bip_utils-2.9.3/bip_utils/bip/bip86/
+-rw-rw-rw-   0        0        0       45 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip86/__init__.py
+-rw-rw-rw-   0        0        0     8917 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/bip86/bip86.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.518081 bip_utils-2.9.3/bip_utils/bip/conf/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.532810 bip_utils-2.9.3/bip_utils/bip/conf/bip44/
+-rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip44/__init__.py
+-rw-rw-rw-   0        0        0     3595 2024-04-14 21:40:32.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip44/bip44_coins.py
+-rw-rw-rw-   0        0        0    46654 2024-04-14 21:51:17.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip44/bip44_conf.py
+-rw-rw-rw-   0        0        0     7059 2024-04-14 21:51:34.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip44/bip44_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.554223 bip_utils-2.9.3/bip_utils/bip/conf/bip49/
+-rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip49/__init__.py
+-rw-rw-rw-   0        0        0     1909 2024-04-14 21:39:40.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip49/bip49_coins.py
+-rw-rw-rw-   0        0        0    15787 2024-04-14 21:52:01.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip49/bip49_conf.py
+-rw-rw-rw-   0        0        0     3467 2024-04-14 21:52:09.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip49/bip49_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.577583 bip_utils-2.9.3/bip_utils/bip/conf/bip84/
+-rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip84/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-04-14 21:33:25.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip84/bip84_coins.py
+-rw-rw-rw-   0        0        0     4972 2024-04-14 21:34:14.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip84/bip84_conf.py
+-rw-rw-rw-   0        0        0     2605 2024-04-14 21:34:29.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip84/bip84_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.599618 bip_utils-2.9.3/bip_utils/bip/conf/bip86/
+-rw-rw-rw-   0        0        0      192 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip86/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-04-14 21:27:43.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip86/bip86_coins.py
+-rw-rw-rw-   0        0        0     3538 2024-04-14 21:35:32.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip86/bip86_conf.py
+-rw-rw-rw-   0        0        0     2483 2024-04-14 21:35:16.000000 bip_utils-2.9.3/bip_utils/bip/conf/bip86/bip86_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.640095 bip_utils-2.9.3/bip_utils/bip/conf/common/
+-rw-rw-rw-   0        0        0      437 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/common/__init__.py
+-rw-rw-rw-   0        0        0     4411 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py
+-rw-rw-rw-   0        0        0     7042 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/common/bip_coin_conf.py
+-rw-rw-rw-   0        0        0     1260 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/common/bip_coins.py
+-rw-rw-rw-   0        0        0     1400 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/common/bip_conf_const.py
+-rw-rw-rw-   0        0        0     5101 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/bip/conf/common/bip_litecoin_conf.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.667883 bip_utils-2.9.3/bip_utils/brainwallet/
+-rw-rw-rw-   0        0        0      216 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/brainwallet/__init__.py
+-rw-rw-rw-   0        0        0     4829 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/brainwallet/brainwallet.py
+-rw-rw-rw-   0        0        0     5254 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/brainwallet/brainwallet_algo.py
+-rw-rw-rw-   0        0        0     2749 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/brainwallet/brainwallet_algo_getter.py
+-rw-rw-rw-   0        0        0     1874 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/brainwallet/ibrainwallet_algo.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.673724 bip_utils-2.9.3/bip_utils/cardano/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.703459 bip_utils-2.9.3/bip_utils/cardano/bip32/
+-rw-rw-rw-   0        0        0      165 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/bip32/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py
+-rw-rw-rw-   0        0        0     4290 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py
+-rw-rw-rw-   0        0        0     4426 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py
+-rw-rw-rw-   0        0        0     1975 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_icarus_bip32.py
+-rw-rw-rw-   0        0        0     4150 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.712219 bip_utils-2.9.3/bip_utils/cardano/byron/
+-rw-rw-rw-   0        0        0       77 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/byron/__init__.py
+-rw-rw-rw-   0        0        0     9560 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/byron/cardano_byron_legacy.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.722926 bip_utils-2.9.3/bip_utils/cardano/cip1852/
+-rw-rw-rw-   0        0        0       55 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/cip1852/__init__.py
+-rw-rw-rw-   0        0        0     8713 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/cip1852/cip1852.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.743365 bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/
+-rw-rw-rw-   0        0        0      222 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/__init__.py
+-rw-rw-rw-   0        0        0     1495 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/cip1852_coins.py
+-rw-rw-rw-   0        0        0     3791 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/cip1852_conf.py
+-rw-rw-rw-   0        0        0     2652 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.757965 bip_utils-2.9.3/bip_utils/cardano/mnemonic/
+-rw-rw-rw-   0        0        0      205 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     2656 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py
+-rw-rw-rw-   0        0        0     2513 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.773541 bip_utils-2.9.3/bip_utils/cardano/shelley/
+-rw-rw-rw-   0        0        0      182 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/shelley/__init__.py
+-rw-rw-rw-   0        0        0     7138 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/shelley/cardano_shelley.py
+-rw-rw-rw-   0        0        0     6383 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/cardano/shelley/cardano_shelley_keys.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.791134 bip_utils-2.9.3/bip_utils/coin_conf/
+-rw-rw-rw-   0        0        0      106 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/coin_conf/__init__.py
+-rw-rw-rw-   0        0        0     2258 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/coin_conf/coin_conf.py
+-rw-rw-rw-   0        0        0    24455 2024-04-15 19:18:02.000000 bip_utils-2.9.3/bip_utils/coin_conf/coins_conf.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.798493 bip_utils-2.9.3/bip_utils/ecc/
+-rw-rw-rw-   0        0        0     2046 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.816986 bip_utils-2.9.3/bip_utils/ecc/common/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/common/__init__.py
+-rw-rw-rw-   0        0        0     5993 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/common/dummy_point.py
+-rw-rw-rw-   0        0        0     6654 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/common/ikeys.py
+-rw-rw-rw-   0        0        0     4819 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/common/ipoint.py
+-rw-rw-rw-   0        0        0     1315 2024-04-14 21:43:39.000000 bip_utils-2.9.3/bip_utils/ecc/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.835481 bip_utils-2.9.3/bip_utils/ecc/curve/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/curve/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/curve/elliptic_curve.py
+-rw-rw-rw-   0        0        0     3135 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/curve/elliptic_curve_getter.py
+-rw-rw-rw-   0        0        0     1486 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/curve/elliptic_curve_types.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.841320 bip_utils-2.9.3/bip_utils/ecc/ecdsa/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ecdsa/__init__.py
+-rw-rw-rw-   0        0        0     1659 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ecdsa/ecdsa_keys.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.874414 bip_utils-2.9.3/bip_utils/ecc/ed25519/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/__init__.py
+-rw-rw-rw-   0        0        0     1828 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519.py
+-rw-rw-rw-   0        0        0     1761 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_const.py
+-rw-rw-rw-   0        0        0     7409 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_keys.py
+-rw-rw-rw-   0        0        0     6701 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_point.py
+-rw-rw-rw-   0        0        0     2307 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.880262 bip_utils-2.9.3/bip_utils/ecc/ed25519/lib/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/lib/__init__.py
+-rw-rw-rw-   0        0        0    10382 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519/lib/ed25519_lib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.904630 bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py
+-rw-rw-rw-   0        0        0     1571 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py
+-rw-rw-rw-   0        0        0     7358 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py
+-rw-rw-rw-   0        0        0     1646 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.925070 bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/__init__.py
+-rw-rw-rw-   0        0        0     1980 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py
+-rw-rw-rw-   0        0        0     1576 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py
+-rw-rw-rw-   0        0        0     5303 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py
+-rw-rw-rw-   0        0        0     1642 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.949402 bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/__init__.py
+-rw-rw-rw-   0        0        0     1980 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero.py
+-rw-rw-rw-   0        0        0     1780 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py
+-rw-rw-rw-   0        0        0     4174 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py
+-rw-rw-rw-   0        0        0     1642 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:38.972763 bip_utils-2.9.3/bip_utils/ecc/nist256p1/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/nist256p1/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1.py
+-rw-rw-rw-   0        0        0     1606 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1_const.py
+-rw-rw-rw-   0        0        0     7231 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1_keys.py
+-rw-rw-rw-   0        0        0     6984 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1_point.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.009787 bip_utils-2.9.3/bip_utils/ecc/secp256k1/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/__init__.py
+-rw-rw-rw-   0        0        0     1783 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1.py
+-rw-rw-rw-   0        0        0     2974 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_const.py
+-rw-rw-rw-   0        0        0     7065 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py
+-rw-rw-rw-   0        0        0     7301 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py
+-rw-rw-rw-   0        0        0     6190 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py
+-rw-rw-rw-   0        0        0     7030 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.033147 bip_utils-2.9.3/bip_utils/ecc/sr25519/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/sr25519/__init__.py
+-rw-rw-rw-   0        0        0     1828 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519.py
+-rw-rw-rw-   0        0        0     1562 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519_const.py
+-rw-rw-rw-   0        0        0     6641 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519_keys.py
+-rw-rw-rw-   0        0        0     1638 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519_point.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.052614 bip_utils-2.9.3/bip_utils/electrum/
+-rw-rw-rw-   0        0        0      136 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/__init__.py
+-rw-rw-rw-   0        0        0    10454 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/electrum_v1.py
+-rw-rw-rw-   0        0        0    12764 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/electrum_v2.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.112112 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/
+-rw-rw-rw-   0        0        0      770 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py
+-rw-rw-rw-   0        0        0     2149 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py
+-rw-rw-rw-   0        0        0     3685 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     3162 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     4396 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     3890 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2181 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     3621 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.117951 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/wordlist/
+-rw-rw-rw-   0        0        0    12120 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/wordlist/english.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.177324 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/
+-rw-rw-rw-   0        0        0      795 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/__init__.py
+-rw-rw-rw-   0        0        0     4300 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py
+-rw-rw-rw-   0        0        0     2937 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py
+-rw-rw-rw-   0        0        0     4499 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     4249 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     5966 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     4266 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2205 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     3308 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.206087 bip_utils-2.9.3/bip_utils/monero/
+-rw-rw-rw-   0        0        0      237 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.234313 bip_utils-2.9.3/bip_utils/monero/conf/
+-rw-rw-rw-   0        0        0      256 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/conf/__init__.py
+-rw-rw-rw-   0        0        0     3770 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/conf/monero_coin_conf.py
+-rw-rw-rw-   0        0        0     1386 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/conf/monero_coins.py
+-rw-rw-rw-   0        0        0     1748 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/conf/monero_conf.py
+-rw-rw-rw-   0        0        0     2508 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/conf/monero_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.294666 bip_utils-2.9.3/bip_utils/monero/mnemonic/
+-rw-rw-rw-   0        0        0      718 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     3191 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_entropy_generator.py
+-rw-rw-rw-   0        0        0     3753 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic.py
+-rw-rw-rw-   0        0        0     4355 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     6520 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     5109 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     4600 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     1872 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     2545 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.470346 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/
+-rw-rw-rw-   0        0        0     8130 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt
+-rw-rw-rw-   0        0        0    14346 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/dutch.txt
+-rw-rw-rw-   0        0        0    13093 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/english.txt
+-rw-rw-rw-   0        0        0    12524 2024-02-13 10:42:53.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/french.txt
+-rw-rw-rw-   0        0        0    13960 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/german.txt
+-rw-rw-rw-   0        0        0    14400 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/italian.txt
+-rw-rw-rw-   0        0        0    21054 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/japanese.txt
+-rw-rw-rw-   0        0        0    14765 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/portuguese.txt
+-rw-rw-rw-   0        0        0    22376 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/russian.txt
+-rw-rw-rw-   0        0        0    12524 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/spanish.txt
+-rw-rw-rw-   0        0        0    10682 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/monero.py
+-rw-rw-rw-   0        0        0     1244 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/monero_ex.py
+-rw-rw-rw-   0        0        0     8202 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/monero_keys.py
+-rw-rw-rw-   0        0        0     6050 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/monero/monero_subaddr.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.490789 bip_utils-2.9.3/bip_utils/slip/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.498137 bip_utils-2.9.3/bip_utils/slip/slip173/
+-rw-rw-rw-   0        0        0       52 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/slip173/__init__.py
+-rw-rw-rw-   0        0        0     2173 2024-04-14 21:57:30.000000 bip_utils-2.9.3/bip_utils/slip/slip173/slip173.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.517627 bip_utils-2.9.3/bip_utils/slip/slip32/
+-rw-rw-rw-   0        0        0      227 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/slip32/__init__.py
+-rw-rw-rw-   0        0        0    11214 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/slip32/slip32.py
+-rw-rw-rw-   0        0        0     2085 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/slip32/slip32_key_net_ver.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.528334 bip_utils-2.9.3/bip_utils/slip/slip44/
+-rw-rw-rw-   0        0        0       49 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/slip44/__init__.py
+-rw-rw-rw-   0        0        0     2557 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/slip/slip44/slip44.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.539045 bip_utils-2.9.3/bip_utils/solana/
+-rw-rw-rw-   0        0        0       49 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/solana/__init__.py
+-rw-rw-rw-   0        0        0     6588 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/solana/spl_token.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.555587 bip_utils-2.9.3/bip_utils/ss58/
+-rw-rw-rw-   0        0        0      112 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/ss58/__init__.py
+-rw-rw-rw-   0        0        0     5967 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/ss58/ss58.py
+-rw-rw-rw-   0        0        0     1243 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/ss58/ss58_ex.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.584789 bip_utils-2.9.3/bip_utils/substrate/
+-rw-rw-rw-   0        0        0      343 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.610713 bip_utils-2.9.3/bip_utils/substrate/conf/
+-rw-rw-rw-   0        0        0      292 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/conf/__init__.py
+-rw-rw-rw-   0        0        0     3031 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/conf/substrate_coin_conf.py
+-rw-rw-rw-   0        0        0     1606 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/conf/substrate_coins.py
+-rw-rw-rw-   0        0        0     3116 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/conf/substrate_conf.py
+-rw-rw-rw-   0        0        0     3179 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/conf/substrate_conf_getter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.619477 bip_utils-2.9.3/bip_utils/substrate/mnemonic/
+-rw-rw-rw-   0        0        0      101 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     2973 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.646328 bip_utils-2.9.3/bip_utils/substrate/scale/
+-rw-rw-rw-   0        0        0      509 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/scale/__init__.py
+-rw-rw-rw-   0        0        0     1628 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_base.py
+-rw-rw-rw-   0        0        0     1948 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_bytes.py
+-rw-rw-rw-   0        0        0     3082 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_cuint.py
+-rw-rw-rw-   0        0        0     4954 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_uint.py
+-rw-rw-rw-   0        0        0    12628 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/substrate.py
+-rw-rw-rw-   0        0        0     1349 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/substrate_ex.py
+-rw-rw-rw-   0        0        0     8752 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/substrate_keys.py
+-rw-rw-rw-   0        0        0     9228 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/substrate/substrate_path.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.652167 bip_utils-2.9.3/bip_utils/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.657034 bip_utils-2.9.3/bip_utils/utils/conf/
+-rw-rw-rw-   0        0        0       55 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/conf/__init__.py
+-rw-rw-rw-   0        0        0     1881 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/conf/coin_names.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.727156 bip_utils-2.9.3/bip_utils/utils/crypto/
+-rw-rw-rw-   0        0        0      748 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/__init__.py
+-rw-rw-rw-   0        0        0     4043 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/aes_ecb.py
+-rw-rw-rw-   0        0        0     5189 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/blake2.py
+-rw-rw-rw-   0        0        0     3566 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     3048 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/crc.py
+-rw-rw-rw-   0        0        0     1944 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/hash160.py
+-rw-rw-rw-   0        0        0     3822 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/hmac.py
+-rw-rw-rw-   0        0        0     2613 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/pbkdf2.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/ripemd.py
+-rw-rw-rw-   0        0        0     2561 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/scrypt.py
+-rw-rw-rw-   0        0        0     4836 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/sha2.py
+-rw-rw-rw-   0        0        0     3097 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/crypto/sha3.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.785716 bip_utils-2.9.3/bip_utils/utils/misc/
+-rw-rw-rw-   0        0        0      501 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/__init__.py
+-rw-rw-rw-   0        0        0     3458 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/algo.py
+-rw-rw-rw-   0        0        0     4870 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/base32.py
+-rw-rw-rw-   0        0        0     3429 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/bit.py
+-rw-rw-rw-   0        0        0     6326 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/bytes.py
+-rw-rw-rw-   0        0        0     4377 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/cbor_indefinite_len_array.py
+-rw-rw-rw-   0        0        0     4924 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/data_bytes.py
+-rw-rw-rw-   0        0        0     3512 2024-02-13 10:43:28.000000 bip_utils-2.9.3/bip_utils/utils/misc/integer.py
+-rw-rw-rw-   0        0        0     1884 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/misc/string.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.834021 bip_utils-2.9.3/bip_utils/utils/mnemonic/
+-rw-rw-rw-   0        0        0      643 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     1976 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/entropy_generator.py
+-rw-rw-rw-   0        0        0     3716 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic.py
+-rw-rw-rw-   0        0        0     3895 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_decoder_base.py
+-rw-rw-rw-   0        0        0     2578 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_encoder_base.py
+-rw-rw-rw-   0        0        0     1251 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_ex.py
+-rw-rw-rw-   0        0        0    11170 2024-02-13 11:51:20.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2860 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.844728 bip_utils-2.9.3/bip_utils/utils/typing/
+-rw-rw-rw-   0        0        0       52 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/typing/__init__.py
+-rw-rw-rw-   0        0        0     1372 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/utils/typing/literal.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:39.866140 bip_utils-2.9.3/bip_utils/wif/
+-rw-rw-rw-   0        0        0       70 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/wif/__init__.py
+-rw-rw-rw-   0        0        0     5624 2024-02-13 10:42:54.000000 bip_utils-2.9.3/bip_utils/wif/wif.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:37.721450 bip_utils-2.9.3/bip_utils.egg-info/
+-rw-rw-rw-   0        0        0    13033 2024-04-15 19:28:37.000000 bip_utils-2.9.3/bip_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14647 2024-04-15 19:28:37.000000 bip_utils-2.9.3/bip_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 19:28:37.000000 bip_utils-2.9.3/bip_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      741 2024-04-15 19:28:37.000000 bip_utils-2.9.3/bip_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-15 19:28:37.000000 bip_utils-2.9.3/bip_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2024-04-14 21:54:11.000000 bip_utils-2.9.3/keywords.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:40.001541 bip_utils-2.9.3/readme/
+-rw-rw-rw-   0        0        0     5128 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/algorand_mnemonic.md
+-rw-rw-rw-   0        0        0    17713 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/bip32.md
+-rw-rw-rw-   0        0        0     3317 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/bip38.md
+-rw-rw-rw-   0        0        0     7775 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/bip39.md
+-rw-rw-rw-   0        0        0    20386 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/bip44.md
+-rw-rw-rw-   0        0        0     4411 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/brainwallet.md
+-rw-rw-rw-   0        0        0    17246 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/cardano.md
+-rw-rw-rw-   0        0        0     4701 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/electrum.md
+-rw-rw-rw-   0        0        0      767 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/electrum_mnemonic.md
+-rw-rw-rw-   0        0        0     4827 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/electrum_v1_mnemonic.md
+-rw-rw-rw-   0        0        0     8675 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/electrum_v2_mnemonic.md
+-rw-rw-rw-   0        0        0     5035 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/monero.md
+-rw-rw-rw-   0        0        0     6792 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/monero_mnemonic.md
+-rw-rw-rw-   0        0        0     8496 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/substrate.md
+drwxrwxrwx   0        0        0        0 2024-04-15 19:28:40.045332 bip_utils-2.9.3/readme/utility/
+-rw-rw-rw-   0        0        0    16875 2024-04-09 17:37:37.000000 bip_utils-2.9.3/readme/utility/addr.md
+-rw-rw-rw-   0        0        0     1500 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/base58.md
+-rw-rw-rw-   0        0        0      613 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/bch_addr_converter.md
+-rw-rw-rw-   0        0        0     1242 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/bech32.md
+-rw-rw-rw-   0        0        0     1433 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/slip32.md
+-rw-rw-rw-   0        0        0      991 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/solana_spl.md
+-rw-rw-rw-   0        0        0      441 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/ss58.md
+-rw-rw-rw-   0        0        0     1940 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility/wif.md
+-rw-rw-rw-   0        0        0      874 2024-02-13 10:42:55.000000 bip_utils-2.9.3/readme/utility_libs.md
+-rw-rw-rw-   0        0        0      124 2024-04-14 21:54:11.000000 bip_utils-2.9.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0      682 2024-04-14 21:54:11.000000 bip_utils-2.9.3/requirements.txt
+-rw-rw-rw-   0        0        0      111 2024-04-15 19:28:40.067718 bip_utils-2.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     6021 2024-04-14 21:54:11.000000 bip_utils-2.9.3/setup.py
```

### Comparing `bip_utils-2.9.2/LICENSE` & `bip_utils-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/PKG-INFO` & `bip_utils-2.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bip_utils
-Version: 2.9.2
+Version: 2.9.3
 Summary: Generation of mnemonics, seeds, private/public keys and addresses for different types of cryptocurrencies
 Home-page: https://github.com/ebellocchia/bip_utils
-Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.9.2.tar.gz
+Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.9.3.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
 Keywords: python,cryptography,ecdsa,ed25519,ed25519-blake2b,nist256p1,secp256k1,sr25519,wallet,hd-wallet,slip10,slip32,bip38,bip39,bip39-substrate,bip32,bip44,bip49,bip84,bip86,bip173,bip350,brainwallet,base58,ss58,bech32,bech32m,segwit,electrum,substrate,taproot,daedalus,byron,shelley,akash,algorand,aptos,arbitrum,atom,avalanche,avax,axelar,band protocol,binance chain,binance smart chain,bitcoin,bitcoin cash,bitcoinsv,bnb,cardano,cardano-byron,cardano-shelley,celo,certik,cosmos,dash,dogecoin,ecash,elrond,eos,ethereum,ethereum classic,fantom opera,fetch.ai,filecoin,harmony one,huobi chain,icon,injective,iris,irisnet,kava,litecoin,matic,metis,monero,multiversx,okex chain,ontology,optimism,osmosis,nano,near,near protocol,neo,pi network,polygon,ripple,secret,solana,stellar,substrate,sui,terra,tezos,theta,tron,vechain,verge,zcash,zilliqa,acala,bifrost,chainx,edgeware,karura,kusama,moonbeam,moonriver,phala,plasm,sora,stafi,polkadot
 Platform: any
@@ -19,39 +19,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cbor2<6.0.0,>=5.1.2
-Requires-Dist: coincurve<19.0.0,>=15.0.1; python_version == "3.7"
-Requires-Dist: coincurve>=15.0.1; python_version > "3.7" and python_version < "3.10"
-Requires-Dist: coincurve>=16.0.0; python_version == "3.10"
-Requires-Dist: coincurve>=18.0.0; python_version == "3.11"
-Requires-Dist: coincurve>=19.0.1; python_version >= "3.12"
-Requires-Dist: crcmod~=1.7
-Requires-Dist: ecdsa~=0.17
-Requires-Dist: ed25519-blake2b<2.0.0,>=1.4; python_version < "3.12"
-Requires-Dist: ed25519-blake2b<2.0.0,>=1.4.1; python_version >= "3.12"
-Requires-Dist: pycryptodome~=3.15
-Requires-Dist: pynacl~=1.5
-Requires-Dist: py-sr25519-bindings<2.0.0,>=0.1.3; python_version < "3.10"
-Requires-Dist: py-sr25519-bindings<2.0.0,>=0.1.4; python_version == "3.10"
-Requires-Dist: py-sr25519-bindings<2.0.0,>=0.2.0; python_version >= "3.11"
-Requires-Dist: typing_extensions>=3.7.2; python_version == "3.7"
 Provides-Extra: develop
-Requires-Dist: coverage>=5.3; extra == "develop"
-Requires-Dist: flake8>=3.8; extra == "develop"
-Requires-Dist: isort>=5.8; extra == "develop"
-Requires-Dist: mypy>=0.900; extra == "develop"
-Requires-Dist: prospector[with_mypy,with_pyroma]>=1.7; extra == "develop"
-Requires-Dist: pytest>=7.0; extra == "develop"
-Requires-Dist: pytest-cov>=2.10; extra == "develop"
+License-File: LICENSE
 
 # BIP Utility Library
 
 | |
 |---|
 | [![PyPI - Version](https://img.shields.io/pypi/v/bip_utils.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/bip_utils/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bip_utils.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/bip_utils/) [![GitHub License](https://img.shields.io/github/license/ebellocchia/bip_utils?label=License)](https://github.com/ebellocchia/bip_utils?tab=MIT-1-ov-file) |
 | [![Code Coverage](https://github.com/ebellocchia/bip_utils/actions/workflows/code-coverage.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/code-coverage.yml) [![Code Analysis](https://github.com/ebellocchia/bip_utils/actions/workflows/code-analysis.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/code-analysis.yml) [![Build & Test](https://github.com/ebellocchia/bip_utils/actions/workflows/test.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/test.yml) [![Test Requirements](https://github.com/ebellocchia/bip_utils/actions/workflows/test_min_reqs.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/test_min_reqs.yml) |
```

### Comparing `bip_utils-2.9.2/README.md` & `bip_utils-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/__init__.py` & `bip_utils-2.9.3/bip_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/P2PKH_addr.py` & `bip_utils-2.9.3/bip_utils/addr/P2PKH_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/P2SH_addr.py` & `bip_utils-2.9.3/bip_utils/addr/P2SH_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/P2TR_addr.py` & `bip_utils-2.9.3/bip_utils/addr/P2TR_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/P2WPKH_addr.py` & `bip_utils-2.9.3/bip_utils/addr/P2WPKH_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/__init__.py` & `bip_utils-2.9.3/bip_utils/addr/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/ada_byron_addr.py` & `bip_utils-2.9.3/bip_utils/addr/ada_byron_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/ada_shelley_addr.py` & `bip_utils-2.9.3/bip_utils/addr/ada_shelley_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/addr_dec_utils.py` & `bip_utils-2.9.3/bip_utils/addr/addr_dec_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/addr_key_validator.py` & `bip_utils-2.9.3/bip_utils/addr/addr_key_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/algo_addr.py` & `bip_utils-2.9.3/bip_utils/addr/algo_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/aptos_addr.py` & `bip_utils-2.9.3/bip_utils/addr/aptos_addr.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,26 +87,30 @@
     def EncodeKey(pub_key: Union[bytes, IPublicKey],
                   **kwargs: Any) -> str:
         """
         Encode a public key to Aptos address.
 
         Args:
             pub_key (bytes or IPublicKey): Public key bytes or object
-            **kwargs                     : Not used
+
+        Other Parameters:
+            trim_zeroes (bool, optional): True to trim left zeroes from the address string, false otherwise (default)
 
         Returns:
             str: Address string
 
         Raises:
             ValueError: If the public key is not valid
             TypeError: If the public key is not ed25519
         """
+        trim_zeroes = kwargs.get("trim_zeroes", False)
+
         pub_key_obj = AddrKeyValidator.ValidateAndGetEd25519Key(pub_key)
 
         payload_bytes = pub_key_obj.RawCompressed().ToBytes()[1:] + AptosAddrConst.SINGLE_SIG_SUFFIX_BYTE
-        key_hash_bytes = Sha3_256.QuickDigest(payload_bytes)
+        key_hash_str = BytesUtils.ToHexString(Sha3_256.QuickDigest(payload_bytes))
 
-        return CoinsConf.Aptos.ParamByKey("addr_prefix") + BytesUtils.ToHexString(key_hash_bytes).lstrip("0")
+        return CoinsConf.Aptos.ParamByKey("addr_prefix") + (key_hash_str.lstrip("0") if trim_zeroes else key_hash_str)
 
 
 # Deprecated: only for compatibility, Encoder class shall be used instead
 AptosAddr = AptosAddrEncoder
```

### Comparing `bip_utils-2.9.2/bip_utils/addr/atom_addr.py` & `bip_utils-2.9.3/bip_utils/addr/atom_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/avax_addr.py` & `bip_utils-2.9.3/bip_utils/addr/avax_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/bch_addr_converter.py` & `bip_utils-2.9.3/bip_utils/addr/bch_addr_converter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/egld_addr.py` & `bip_utils-2.9.3/bip_utils/addr/egld_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/eos_addr.py` & `bip_utils-2.9.3/bip_utils/addr/eos_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/ergo_addr.py` & `bip_utils-2.9.3/bip_utils/addr/ergo_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/eth_addr.py` & `bip_utils-2.9.3/bip_utils/addr/eth_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/fil_addr.py` & `bip_utils-2.9.3/bip_utils/addr/fil_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/iaddr_decoder.py` & `bip_utils-2.9.3/bip_utils/addr/iaddr_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/iaddr_encoder.py` & `bip_utils-2.9.3/bip_utils/addr/iaddr_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/icx_addr.py` & `bip_utils-2.9.3/bip_utils/addr/icx_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/inj_addr.py` & `bip_utils-2.9.3/bip_utils/addr/inj_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/nano_addr.py` & `bip_utils-2.9.3/bip_utils/addr/nano_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/near_addr.py` & `bip_utils-2.9.3/bip_utils/addr/near_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/neo_addr.py` & `bip_utils-2.9.3/bip_utils/addr/neo_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/okex_addr.py` & `bip_utils-2.9.3/bip_utils/addr/okex_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/one_addr.py` & `bip_utils-2.9.3/bip_utils/addr/one_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/sol_addr.py` & `bip_utils-2.9.3/bip_utils/addr/sol_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/substrate_addr.py` & `bip_utils-2.9.3/bip_utils/addr/substrate_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/sui_addr.py` & `bip_utils-2.9.3/bip_utils/addr/sui_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/trx_addr.py` & `bip_utils-2.9.3/bip_utils/addr/trx_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/xlm_addr.py` & `bip_utils-2.9.3/bip_utils/addr/xlm_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/xmr_addr.py` & `bip_utils-2.9.3/bip_utils/addr/xmr_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/xrp_addr.py` & `bip_utils-2.9.3/bip_utils/addr/xrp_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/xtz_addr.py` & `bip_utils-2.9.3/bip_utils/addr/xtz_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/addr/zil_addr.py` & `bip_utils-2.9.3/bip_utils/addr/zil_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/__init__.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_entropy_generator.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/algorand/mnemonic/algorand_seed_generator.py` & `bip_utils-2.9.3/bip_utils/algorand/mnemonic/algorand_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/base58/base58.py` & `bip_utils-2.9.3/bip_utils/base58/base58.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/base58/base58_ex.py` & `bip_utils-2.9.3/bip_utils/base58/base58_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/base58/base58_xmr.py` & `bip_utils-2.9.3/bip_utils/base58/base58_xmr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bech32/bch_bech32.py` & `bip_utils-2.9.3/bip_utils/bech32/bch_bech32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bech32/bech32.py` & `bip_utils-2.9.3/bip_utils/bech32/bech32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bech32/bech32_base.py` & `bip_utils-2.9.3/bip_utils/bech32/bech32_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bech32/bech32_ex.py` & `bip_utils-2.9.3/bip_utils/bech32/bech32_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bech32/segwit_bech32.py` & `bip_utils-2.9.3/bip_utils/bech32/segwit_bech32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/__init__.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/base/bip32_base.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/base/bip32_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/base/ibip32_key_derivator.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/base/ibip32_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_const.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_ex.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_key_data.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_key_data.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_key_net_ver.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_key_net_ver.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_key_ser.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_key_ser.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_keys.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_path.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_path.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/bip32_utils.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/bip32_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/__init__.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py` & `bip_utils-2.9.3/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip38/bip38.py` & `bip_utils-2.9.3/bip_utils/bip/bip38/bip38.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip38/bip38_addr.py` & `bip_utils-2.9.3/bip_utils/bip/bip38/bip38_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip38/bip38_ec.py` & `bip_utils-2.9.3/bip_utils/bip/bip38/bip38_ec.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip38/bip38_no_ec.py` & `bip_utils-2.9.3/bip_utils/bip/bip38/bip38_no_ec.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/__init__.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_entropy_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_decoder.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_encoder.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_utils.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_mnemonic_validator.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/bip39_seed_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/bip39_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/ibip39_seed_generator.py` & `bip_utils-2.9.3/bip_utils/bip/bip39/ibip39_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/chinese_simplified.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/chinese_traditional.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/czech.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/czech.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/english.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/french.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/italian.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/korean.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/korean.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/portuguese.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/portuguese.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip39/wordlist/spanish.txt` & `bip_utils-2.9.3/bip_utils/bip/bip39/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip44/bip44.py` & `bip_utils-2.9.3/bip_utils/bip/bip44/bip44.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip44_base/bip44_base.py` & `bip_utils-2.9.3/bip_utils/bip/bip44_base/bip44_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip44_base/bip44_base_ex.py` & `bip_utils-2.9.3/bip_utils/bip/bip44_base/bip44_base_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip44_base/bip44_keys.py` & `bip_utils-2.9.3/bip_utils/bip/bip44_base/bip44_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip49/bip49.py` & `bip_utils-2.9.3/bip_utils/bip/bip49/bip49.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip84/bip84.py` & `bip_utils-2.9.3/bip_utils/bip/bip84/bip84.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/bip86/bip86.py` & `bip_utils-2.9.3/bip_utils/bip/bip86/bip86.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip44/bip44_coins.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip44/bip44_coins.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     VERGE = auto()
     ZCASH = auto()
     ZILLIQA = auto()
     # Test nets
     BITCOIN_CASH_TESTNET = auto()
     BITCOIN_CASH_SLP_TESTNET = auto()
     BITCOIN_SV_TESTNET = auto()
+    BITCOIN_REGTEST = auto()
     BITCOIN_TESTNET = auto()
     DASH_TESTNET = auto()
     DOGECOIN_TESTNET = auto()
     ECASH_TESTNET = auto()
     ERGO_TESTNET = auto()
     LITECOIN_TESTNET = auto()
     ZCASH_TESTNET = auto()
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip44/bip44_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip44/bip44_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,29 @@
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinMainNet.ParamByKey("p2pkh_net_ver"),
         },
     )
+    # Configuration for Bitcoin regtest
+    BitcoinRegTest: BipCoinConf = BipCoinConf(
+        coin_names=CoinsConf.BitcoinRegTest.CoinNames(),
+        coin_idx=Slip44.TESTNET,
+        is_testnet=True,
+        def_path=DER_PATH_NON_HARDENED_FULL,
+        key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
+        wif_net_ver=CoinsConf.BitcoinRegTest.ParamByKey("wif_net_ver"),
+        bip32_cls=Bip32Slip10Secp256k1,
+        addr_cls=P2PKHAddrEncoder,
+        addr_params={
+            "net_ver": CoinsConf.BitcoinRegTest.ParamByKey("p2pkh_net_ver"),
+        },
+    )
+
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
         def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip44/bip44_conf_getter.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip44/bip44_conf_getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         Bip44Coins.AVAX_P_CHAIN: Bip44Conf.AvaxPChain,
         Bip44Coins.AVAX_X_CHAIN: Bip44Conf.AvaxXChain,
         Bip44Coins.AXELAR: Bip44Conf.Axelar,
         Bip44Coins.BAND_PROTOCOL: Bip44Conf.BandProtocol,
         Bip44Coins.BINANCE_CHAIN: Bip44Conf.BinanceChain,
         Bip44Coins.BINANCE_SMART_CHAIN: Bip44Conf.BinanceSmartChain,
         Bip44Coins.BITCOIN: Bip44Conf.BitcoinMainNet,
+        Bip44Coins.BITCOIN_REGTEST: Bip44Conf.BitcoinRegTest,
         Bip44Coins.BITCOIN_TESTNET: Bip44Conf.BitcoinTestNet,
         Bip44Coins.BITCOIN_CASH: Bip44Conf.BitcoinCashMainNet,
         Bip44Coins.BITCOIN_CASH_TESTNET: Bip44Conf.BitcoinCashTestNet,
         Bip44Coins.BITCOIN_CASH_SLP: Bip44Conf.BitcoinCashSlpMainNet,
         Bip44Coins.BITCOIN_CASH_SLP_TESTNET: Bip44Conf.BitcoinCashSlpTestNet,
         Bip44Coins.BITCOIN_SV: Bip44Conf.BitcoinSvMainNet,
         Bip44Coins.BITCOIN_SV_TESTNET: Bip44Conf.BitcoinSvTestNet,
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip49/bip49_coins.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip49/bip49_coins.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,13 +40,14 @@
     ECASH = auto()
     LITECOIN = auto()
     ZCASH = auto()
     # Test nets
     BITCOIN_CASH_TESTNET = auto()
     BITCOIN_CASH_SLP_TESTNET = auto()
     BITCOIN_SV_TESTNET = auto()
+    BITCOIN_REGTEST = auto()
     BITCOIN_TESTNET = auto()
     DASH_TESTNET = auto()
     DOGECOIN_TESTNET = auto()
     ECASH_TESTNET = auto()
     LITECOIN_TESTNET = auto()
     ZCASH_TESTNET = auto()
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip49/bip49_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip49/bip49_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,28 @@
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinMainNet.ParamByKey("p2sh_net_ver"),
         },
     )
+    # Configuration for Bitcoin regtest
+    BitcoinRegTest: BipCoinConf = BipCoinConf(
+        coin_names=CoinsConf.BitcoinRegTest.CoinNames(),
+        coin_idx=Slip44.TESTNET,
+        is_testnet=True,
+        def_path=DER_PATH_NON_HARDENED_FULL,
+        key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
+        wif_net_ver=CoinsConf.BitcoinRegTest.ParamByKey("wif_net_ver"),
+        bip32_cls=Bip32Slip10Secp256k1,
+        addr_cls=P2SHAddrEncoder,
+        addr_params={
+            "net_ver": CoinsConf.BitcoinRegTest.ParamByKey("p2sh_net_ver"),
+        },
+    )
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
         def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip49/bip49_conf_getter.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip49/bip49_conf_getter.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 class Bip49ConfGetterConst:
     """Class container for BIP49 configuration getter constants."""
 
     # Map from Bip49Coins to configuration classes
     COIN_TO_CONF: Dict[BipCoins, BipCoinConf] = {
         Bip49Coins.BITCOIN: Bip49Conf.BitcoinMainNet,
+        Bip49Coins.BITCOIN_REGTEST: Bip49Conf.BitcoinRegTest,
         Bip49Coins.BITCOIN_TESTNET: Bip49Conf.BitcoinTestNet,
         Bip49Coins.BITCOIN_CASH: Bip49Conf.BitcoinCashMainNet,
         Bip49Coins.BITCOIN_CASH_TESTNET: Bip49Conf.BitcoinCashTestNet,
         Bip49Coins.BITCOIN_CASH_SLP: Bip49Conf.BitcoinCashSlpMainNet,
         Bip49Coins.BITCOIN_CASH_SLP_TESTNET: Bip49Conf.BitcoinCashSlpTestNet,
         Bip49Coins.BITCOIN_SV: Bip49Conf.BitcoinSvMainNet,
         Bip49Coins.BITCOIN_SV_TESTNET: Bip49Conf.BitcoinSvTestNet,
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip84/bip84_coins.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip84/bip84_coins.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 class Bip84Coins(BipCoins):
     """Enumerative for supported BIP84 coins."""
 
     # Main nets
     BITCOIN = auto()
     LITECOIN = auto()
     # Test nets
+    BITCOIN_REGTEST = auto()
     BITCOIN_TESTNET = auto()
     LITECOIN_TESTNET = auto()
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip84/bip84_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip84/bip84_conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,59 +24,75 @@
 from bip_utils.addr import P2WPKHAddrEncoder
 from bip_utils.bip.bip32 import Bip32KeyNetVersions, Bip32Slip10Secp256k1
 from bip_utils.bip.conf.common import DER_PATH_NON_HARDENED_FULL, BipCoinConf
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
-# Bitcoin key net version (zpub / zprv)
-_BIP84_BTC_KEY_NET_VER: Bip32KeyNetVersions = Bip32KeyNetVersions(b"\x04\xb2\x47\x46",
-                                                                  b"\x04\xb2\x43\x0c")
+# Bitcoin key net version for main net (zpub / zprv)
+_BIP84_BTC_KEY_NET_VER_MAIN: Bip32KeyNetVersions = Bip32KeyNetVersions(b"\x04\xb2\x47\x46",
+                                                                       b"\x04\xb2\x43\x0c")
+# Bitcoin key test net version for test net (vpub / vprv)
+_BIP84_BTC_KEY_NET_VER_TEST: Bip32KeyNetVersions = Bip32KeyNetVersions(b"\x04\x5f\x1c\xf6",
+                                                                       b"\x04\x5f\x18\xbc")
 
 
 class Bip84Conf:
     """Class container for BIP84 configuration."""
 
     # Configuration for Bitcoin main net
     BitcoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN,
         is_testnet=False,
         def_path=DER_PATH_NON_HARDENED_FULL,
-        key_net_ver=_BIP84_BTC_KEY_NET_VER,
+        key_net_ver=_BIP84_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinMainNet.ParamByKey("p2wpkh_hrp"),
         },
     )
+    # Configuration for Bitcoin regtest
+    BitcoinRegTest: BipCoinConf = BipCoinConf(
+        coin_names=CoinsConf.BitcoinRegTest.CoinNames(),
+        coin_idx=Slip44.TESTNET,
+        is_testnet=True,
+        def_path=DER_PATH_NON_HARDENED_FULL,
+        key_net_ver=_BIP84_BTC_KEY_NET_VER_TEST,
+        wif_net_ver=CoinsConf.BitcoinRegTest.ParamByKey("wif_net_ver"),
+        bip32_cls=Bip32Slip10Secp256k1,
+        addr_cls=P2WPKHAddrEncoder,
+        addr_params={
+            "hrp": CoinsConf.BitcoinRegTest.ParamByKey("p2wpkh_hrp"),
+        },
+    )
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
         def_path=DER_PATH_NON_HARDENED_FULL,
-        key_net_ver=Bip32KeyNetVersions(b"\x04\x5f\x1c\xf6",
-                                        b"\x04\x5f\x18\xbc"),   # vpub / vprv
+        key_net_ver=_BIP84_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinTestNet.ParamByKey("p2wpkh_hrp"),
         },
     )
 
     # Configuration for Litecoin main net
     LitecoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.LitecoinMainNet.CoinNames(),
         coin_idx=Slip44.LITECOIN,
         is_testnet=False,
         def_path=DER_PATH_NON_HARDENED_FULL,
-        key_net_ver=_BIP84_BTC_KEY_NET_VER,
+        key_net_ver=_BIP84_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.LitecoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.LitecoinMainNet.ParamByKey("p2wpkh_hrp"),
         },
     )
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip84/bip84_conf_getter.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip84/bip84_conf_getter.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 class Bip84ConfGetterConst:
     """Class container for BIP84 configuration getter constants."""
 
     # Map from Bip84Coins to configuration classes
     COIN_TO_CONF: Dict[BipCoins, BipCoinConf] = {
         Bip84Coins.BITCOIN: Bip84Conf.BitcoinMainNet,
+        Bip84Coins.BITCOIN_REGTEST: Bip84Conf.BitcoinRegTest,
         Bip84Coins.BITCOIN_TESTNET: Bip84Conf.BitcoinTestNet,
         Bip84Coins.LITECOIN: Bip84Conf.LitecoinMainNet,
         Bip84Coins.LITECOIN_TESTNET: Bip84Conf.LitecoinTestNet,
     }
 
 
 class Bip84ConfGetter:
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip86/bip86_coins.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip86/bip86_coins.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 @unique
 class Bip86Coins(BipCoins):
     """Enumerative for supported BIP86 coins."""
 
     # Main nets
     BITCOIN = auto()
     # Test nets
+    BITCOIN_REGTEST = auto()
     BITCOIN_TESTNET = auto()
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip86/bip86_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip86/bip86_conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,37 +25,52 @@
 from bip_utils.bip.bip32 import Bip32Const, Bip32KeyNetVersions, Bip32Slip10Secp256k1
 from bip_utils.bip.conf.common import DER_PATH_NON_HARDENED_FULL, BipCoinConf
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
 # Bitcoin key net version for main net (same as BIP32)
-_BIP86_BTC_KEY_NET_VER: Bip32KeyNetVersions = Bip32Const.MAIN_NET_KEY_NET_VERSIONS
+_BIP86_BTC_KEY_NET_VER_MAIN: Bip32KeyNetVersions = Bip32Const.MAIN_NET_KEY_NET_VERSIONS
 # Bitcoin key net version for test net (same as BIP32)
 _BIP86_BTC_KEY_NET_VER_TEST: Bip32KeyNetVersions = Bip32Const.TEST_NET_KEY_NET_VERSIONS
 
 
 class Bip86Conf:
     """Class container for BIP86 configuration."""
 
     # Configuration for Bitcoin main net
     BitcoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN,
         is_testnet=False,
         def_path=DER_PATH_NON_HARDENED_FULL,
-        key_net_ver=_BIP86_BTC_KEY_NET_VER,
+        key_net_ver=_BIP86_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2TRAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinMainNet.ParamByKey("p2tr_hrp"),
         },
     )
 
+    # Configuration for Bitcoin regtest
+    BitcoinRegTest: BipCoinConf = BipCoinConf(
+        coin_names=CoinsConf.BitcoinRegTest.CoinNames(),
+        coin_idx=Slip44.TESTNET,
+        is_testnet=True,
+        def_path=DER_PATH_NON_HARDENED_FULL,
+        key_net_ver=_BIP86_BTC_KEY_NET_VER_TEST,
+        wif_net_ver=CoinsConf.BitcoinRegTest.ParamByKey("wif_net_ver"),
+        bip32_cls=Bip32Slip10Secp256k1,
+        addr_cls=P2TRAddrEncoder,
+        addr_params={
+            "hrp": CoinsConf.BitcoinRegTest.ParamByKey("p2tr_hrp"),
+        },
+    )
+
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
         def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP86_BTC_KEY_NET_VER_TEST,
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/bip86/bip86_conf_getter.py` & `bip_utils-2.9.3/bip_utils/bip/conf/bip86/bip86_conf_getter.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 class Bip86ConfGetterConst:
     """Class container for BIP86 configuration getter constants."""
 
     # Map from Bip86Coins to configuration classes
     COIN_TO_CONF: Dict[BipCoins, BipCoinConf] = {
         Bip86Coins.BITCOIN: Bip86Conf.BitcoinMainNet,
+        Bip86Coins.BITCOIN_REGTEST: Bip86Conf.BitcoinRegTest,
         Bip86Coins.BITCOIN_TESTNET: Bip86Conf.BitcoinTestNet,
     }
 
 
 class Bip86ConfGetter:
     """
     BIP86 configuration getter class.
```

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/common/bip_coin_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/common/bip_coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/common/bip_coins.py` & `bip_utils-2.9.3/bip_utils/bip/conf/common/bip_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/common/bip_conf_const.py` & `bip_utils-2.9.3/bip_utils/bip/conf/common/bip_conf_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/bip/conf/common/bip_litecoin_conf.py` & `bip_utils-2.9.3/bip_utils/bip/conf/common/bip_litecoin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/brainwallet/brainwallet.py` & `bip_utils-2.9.3/bip_utils/brainwallet/brainwallet.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/brainwallet/brainwallet_algo.py` & `bip_utils-2.9.3/bip_utils/brainwallet/brainwallet_algo.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/brainwallet/brainwallet_algo_getter.py` & `bip_utils-2.9.3/bip_utils/brainwallet/brainwallet_algo_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/brainwallet/ibrainwallet_algo.py` & `bip_utils-2.9.3/bip_utils/brainwallet/ibrainwallet_algo.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py` & `bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py` & `bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py` & `bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_icarus_bip32.py` & `bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_icarus_bip32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py` & `bip_utils-2.9.3/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/byron/cardano_byron_legacy.py` & `bip_utils-2.9.3/bip_utils/cardano/byron/cardano_byron_legacy.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/cip1852/cip1852.py` & `bip_utils-2.9.3/bip_utils/cardano/cip1852/cip1852.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/cip1852_coins.py` & `bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/cip1852_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/cip1852_conf.py` & `bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/cip1852_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py` & `bip_utils-2.9.3/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py` & `bip_utils-2.9.3/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py` & `bip_utils-2.9.3/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/shelley/cardano_shelley.py` & `bip_utils-2.9.3/bip_utils/cardano/shelley/cardano_shelley.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/cardano/shelley/cardano_shelley_keys.py` & `bip_utils-2.9.3/bip_utils/cardano/shelley/cardano_shelley_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/coin_conf/coin_conf.py` & `bip_utils-2.9.3/bip_utils/coin_conf/coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/coin_conf/coins_conf.py` & `bip_utils-2.9.3/bip_utils/coin_conf/coins_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,22 @@
 _BTC_P2PKH_NET_VER_TN: bytes = b"\x6f"
 _BTC_P2SH_NET_VER_TN: bytes = b"\xc4"
 _BTC_P2WPKH_HRP_TN: str = Slip173.BITCOIN_TESTNET
 _BTC_P2WPKH_WIT_VER_TN: int = 0
 _BTC_P2TR_HRP_TN: str = Slip173.BITCOIN_TESTNET
 _BTC_P2TR_WIT_VER_TN: int = 1
 _BTC_WIF_NET_VER_TN: bytes = b"\xef"
+# Regtest
+_BTC_P2PKH_NET_VER_RT: bytes = _BTC_P2PKH_NET_VER_TN
+_BTC_P2SH_NET_VER_RT: bytes = _BTC_P2SH_NET_VER_TN
+_BTC_P2WPKH_HRP_RT: str = Slip173.BITCOIN_REGTEST
+_BTC_P2WPKH_WIT_VER_RT: int = _BTC_P2TR_WIT_VER_TN
+_BTC_P2TR_HRP_RT: str = Slip173.BITCOIN_REGTEST
+_BTC_P2TR_WIT_VER_RT: int = _BTC_P2TR_WIT_VER_TN
+_BTC_WIF_NET_VER_RT: bytes = _BTC_WIF_NET_VER_TN
 
 
 class CoinsConf:
     """Class container for coins configuration."""
 
     # Configuration for Acala
     Acala: CoinConf = CoinConf(
@@ -165,19 +173,33 @@
         coin_name=CoinNames("Bitcoin TestNet", "BTC"),
         params={
             "p2pkh_net_ver": _BTC_P2PKH_NET_VER_TN,
             "p2sh_net_ver": _BTC_P2SH_NET_VER_TN,
             "p2wpkh_hrp": _BTC_P2WPKH_HRP_TN,
             "p2wpkh_wit_ver": _BTC_P2WPKH_WIT_VER_TN,
             "p2tr_hrp": _BTC_P2TR_HRP_TN,
-            "p2tr_wit_ver": _BTC_P2TR_WIT_VER_MN,
+            "p2tr_wit_ver": _BTC_P2TR_WIT_VER_TN,
             "wif_net_ver": _BTC_WIF_NET_VER_TN,
         },
     )
 
+    # Configuration for Bitcoin regtest
+    BitcoinRegTest: CoinConf = CoinConf(
+        coin_name=CoinNames("Bitcoin RegTest", "BTC"),
+        params={
+            "p2pkh_net_ver": _BTC_P2PKH_NET_VER_RT,
+            "p2sh_net_ver": _BTC_P2SH_NET_VER_RT,
+            "p2wpkh_hrp": _BTC_P2WPKH_HRP_RT,
+            "p2wpkh_wit_ver": _BTC_P2WPKH_WIT_VER_RT,
+            "p2tr_hrp": _BTC_P2TR_HRP_RT,
+            "p2tr_wit_ver": _BTC_P2TR_WIT_VER_RT,
+            "wif_net_ver": _BTC_WIF_NET_VER_RT,
+        },
+    )
+
     # Configuration for Bitcoin Cash main net
     BitcoinCashMainNet: CoinConf = CoinConf(
         coin_name=CoinNames("Bitcoin Cash", "BCH"),
         params={
             "p2pkh_std_hrp": "bitcoincash",
             "p2pkh_std_net_ver": _BTC_P2PKH_NET_VER_MN,
             "p2pkh_legacy_net_ver": _BTC_P2PKH_NET_VER_MN,
```

### Comparing `bip_utils-2.9.2/bip_utils/ecc/__init__.py` & `bip_utils-2.9.3/bip_utils/ecc/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/common/dummy_point.py` & `bip_utils-2.9.3/bip_utils/ecc/common/dummy_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/common/ikeys.py` & `bip_utils-2.9.3/bip_utils/ecc/common/ikeys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/common/ipoint.py` & `bip_utils-2.9.3/bip_utils/ecc/common/ipoint.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/conf.py` & `bip_utils-2.9.3/bip_utils/ecc/conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/curve/elliptic_curve.py` & `bip_utils-2.9.3/bip_utils/ecc/curve/elliptic_curve.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/curve/elliptic_curve_getter.py` & `bip_utils-2.9.3/bip_utils/ecc/curve/elliptic_curve_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/curve/elliptic_curve_types.py` & `bip_utils-2.9.3/bip_utils/ecc/curve/elliptic_curve_types.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ecdsa/ecdsa_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/ecdsa/ecdsa_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_const.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_point.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519/ed25519_utils.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519/ed25519_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519/lib/ed25519_lib.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519/lib/ed25519_lib.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py` & `bip_utils-2.9.3/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1.py` & `bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1_const.py` & `bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/nist256p1/nist256p1_point.py` & `bip_utils-2.9.3/bip_utils/ecc/nist256p1/nist256p1_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1.py` & `bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_const.py` & `bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py` & `bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py` & `bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py` & `bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py` & `bip_utils-2.9.3/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519.py` & `bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519_const.py` & `bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519_keys.py` & `bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ecc/sr25519/sr25519_point.py` & `bip_utils-2.9.3/bip_utils/ecc/sr25519/sr25519_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/electrum_v1.py` & `bip_utils-2.9.3/bip_utils/electrum/electrum_v1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/electrum_v2.py` & `bip_utils-2.9.3/bip_utils/electrum/electrum_v2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/__init__.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v1/wordlist/english.txt` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v1/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/__init__.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py` & `bip_utils-2.9.3/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/conf/monero_coin_conf.py` & `bip_utils-2.9.3/bip_utils/monero/conf/monero_coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/conf/monero_coins.py` & `bip_utils-2.9.3/bip_utils/monero/conf/monero_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/conf/monero_conf.py` & `bip_utils-2.9.3/bip_utils/monero/conf/monero_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/conf/monero_conf_getter.py` & `bip_utils-2.9.3/bip_utils/monero/conf/monero_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/__init__.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_entropy_generator.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_generator.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_utils.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_mnemonic_validator.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/monero_seed_generator.py` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/monero_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/dutch.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/dutch.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/english.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/french.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/german.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/german.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/italian.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/japanese.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/portuguese.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/portuguese.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/russian.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/russian.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/mnemonic/wordlist/spanish.txt` & `bip_utils-2.9.3/bip_utils/monero/mnemonic/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/monero.py` & `bip_utils-2.9.3/bip_utils/monero/monero.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/monero_ex.py` & `bip_utils-2.9.3/bip_utils/monero/monero_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/monero_keys.py` & `bip_utils-2.9.3/bip_utils/monero/monero_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/monero/monero_subaddr.py` & `bip_utils-2.9.3/bip_utils/monero/monero_subaddr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/slip/slip173/slip173.py` & `bip_utils-2.9.3/bip_utils/slip/slip173/slip173.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     """
 
     AKASH_NETWORK: str = "akash"
     AXELAR: str = "axelar"
     BAND_PROTOCOL: str = "band"
     BINANCE_CHAIN: str = "bnb"
     BITCOIN_MAINNET: str = "bc"
+    BITCOIN_REGTEST: str = "bcrt"
     BITCOIN_TESTNET: str = "tb"
     CERTIK: str = "certik"
     CHIHUAHUA: str = "chihuahua"
     COSMOS: str = "cosmos"
     ELROND: str = "erd"
     FETCH_AI: str = "fetch"
     HARMONY_ONE: str = "one"
```

### Comparing `bip_utils-2.9.2/bip_utils/slip/slip32/slip32.py` & `bip_utils-2.9.3/bip_utils/slip/slip32/slip32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/slip/slip32/slip32_key_net_ver.py` & `bip_utils-2.9.3/bip_utils/slip/slip32/slip32_key_net_ver.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/slip/slip44/slip44.py` & `bip_utils-2.9.3/bip_utils/slip/slip44/slip44.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/solana/spl_token.py` & `bip_utils-2.9.3/bip_utils/solana/spl_token.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ss58/ss58.py` & `bip_utils-2.9.3/bip_utils/ss58/ss58.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/ss58/ss58_ex.py` & `bip_utils-2.9.3/bip_utils/ss58/ss58_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/conf/substrate_coin_conf.py` & `bip_utils-2.9.3/bip_utils/substrate/conf/substrate_coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/conf/substrate_coins.py` & `bip_utils-2.9.3/bip_utils/substrate/conf/substrate_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/conf/substrate_conf.py` & `bip_utils-2.9.3/bip_utils/substrate/conf/substrate_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/conf/substrate_conf_getter.py` & `bip_utils-2.9.3/bip_utils/substrate/conf/substrate_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py` & `bip_utils-2.9.3/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_base.py` & `bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_bytes.py` & `bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_bytes.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_cuint.py` & `bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_cuint.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/scale/substrate_scale_enc_uint.py` & `bip_utils-2.9.3/bip_utils/substrate/scale/substrate_scale_enc_uint.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/substrate.py` & `bip_utils-2.9.3/bip_utils/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/substrate_ex.py` & `bip_utils-2.9.3/bip_utils/substrate/substrate_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/substrate_keys.py` & `bip_utils-2.9.3/bip_utils/substrate/substrate_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/substrate/substrate_path.py` & `bip_utils-2.9.3/bip_utils/substrate/substrate_path.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/conf/coin_names.py` & `bip_utils-2.9.3/bip_utils/utils/conf/coin_names.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/__init__.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/aes_ecb.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/aes_ecb.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/blake2.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/blake2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/chacha20_poly1305.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/crc.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/crc.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/hash160.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/hash160.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/hmac.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/hmac.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/pbkdf2.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/ripemd.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/ripemd.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/scrypt.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/scrypt.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/sha2.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/sha2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/crypto/sha3.py` & `bip_utils-2.9.3/bip_utils/utils/crypto/sha3.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/algo.py` & `bip_utils-2.9.3/bip_utils/utils/misc/algo.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/base32.py` & `bip_utils-2.9.3/bip_utils/utils/misc/base32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/bit.py` & `bip_utils-2.9.3/bip_utils/utils/misc/bit.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/bytes.py` & `bip_utils-2.9.3/bip_utils/utils/misc/bytes.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/cbor_indefinite_len_array.py` & `bip_utils-2.9.3/bip_utils/utils/misc/cbor_indefinite_len_array.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/data_bytes.py` & `bip_utils-2.9.3/bip_utils/utils/misc/data_bytes.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/integer.py` & `bip_utils-2.9.3/bip_utils/utils/misc/integer.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/misc/string.py` & `bip_utils-2.9.3/bip_utils/utils/misc/string.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/__init__.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/entropy_generator.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_decoder_base.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_decoder_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_encoder_base.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_encoder_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_ex.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_utils.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/mnemonic/mnemonic_validator.py` & `bip_utils-2.9.3/bip_utils/utils/mnemonic/mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/utils/typing/literal.py` & `bip_utils-2.9.3/bip_utils/utils/typing/literal.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils/wif/wif.py` & `bip_utils-2.9.3/bip_utils/wif/wif.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils.egg-info/PKG-INFO` & `bip_utils-2.9.3/bip_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: bip_utils
-Version: 2.9.2
+Name: bip-utils
+Version: 2.9.3
 Summary: Generation of mnemonics, seeds, private/public keys and addresses for different types of cryptocurrencies
 Home-page: https://github.com/ebellocchia/bip_utils
-Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.9.2.tar.gz
+Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.9.3.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
 Keywords: python,cryptography,ecdsa,ed25519,ed25519-blake2b,nist256p1,secp256k1,sr25519,wallet,hd-wallet,slip10,slip32,bip38,bip39,bip39-substrate,bip32,bip44,bip49,bip84,bip86,bip173,bip350,brainwallet,base58,ss58,bech32,bech32m,segwit,electrum,substrate,taproot,daedalus,byron,shelley,akash,algorand,aptos,arbitrum,atom,avalanche,avax,axelar,band protocol,binance chain,binance smart chain,bitcoin,bitcoin cash,bitcoinsv,bnb,cardano,cardano-byron,cardano-shelley,celo,certik,cosmos,dash,dogecoin,ecash,elrond,eos,ethereum,ethereum classic,fantom opera,fetch.ai,filecoin,harmony one,huobi chain,icon,injective,iris,irisnet,kava,litecoin,matic,metis,monero,multiversx,okex chain,ontology,optimism,osmosis,nano,near,near protocol,neo,pi network,polygon,ripple,secret,solana,stellar,substrate,sui,terra,tezos,theta,tron,vechain,verge,zcash,zilliqa,acala,bifrost,chainx,edgeware,karura,kusama,moonbeam,moonriver,phala,plasm,sora,stafi,polkadot
 Platform: any
@@ -19,39 +19,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cbor2<6.0.0,>=5.1.2
-Requires-Dist: coincurve<19.0.0,>=15.0.1; python_version == "3.7"
-Requires-Dist: coincurve>=15.0.1; python_version > "3.7" and python_version < "3.10"
-Requires-Dist: coincurve>=16.0.0; python_version == "3.10"
-Requires-Dist: coincurve>=18.0.0; python_version == "3.11"
-Requires-Dist: coincurve>=19.0.1; python_version >= "3.12"
-Requires-Dist: crcmod~=1.7
-Requires-Dist: ecdsa~=0.17
-Requires-Dist: ed25519-blake2b<2.0.0,>=1.4; python_version < "3.12"
-Requires-Dist: ed25519-blake2b<2.0.0,>=1.4.1; python_version >= "3.12"
-Requires-Dist: pycryptodome~=3.15
-Requires-Dist: pynacl~=1.5
-Requires-Dist: py-sr25519-bindings<2.0.0,>=0.1.3; python_version < "3.10"
-Requires-Dist: py-sr25519-bindings<2.0.0,>=0.1.4; python_version == "3.10"
-Requires-Dist: py-sr25519-bindings<2.0.0,>=0.2.0; python_version >= "3.11"
-Requires-Dist: typing_extensions>=3.7.2; python_version == "3.7"
 Provides-Extra: develop
-Requires-Dist: coverage>=5.3; extra == "develop"
-Requires-Dist: flake8>=3.8; extra == "develop"
-Requires-Dist: isort>=5.8; extra == "develop"
-Requires-Dist: mypy>=0.900; extra == "develop"
-Requires-Dist: prospector[with_mypy,with_pyroma]>=1.7; extra == "develop"
-Requires-Dist: pytest>=7.0; extra == "develop"
-Requires-Dist: pytest-cov>=2.10; extra == "develop"
+License-File: LICENSE
 
 # BIP Utility Library
 
 | |
 |---|
 | [![PyPI - Version](https://img.shields.io/pypi/v/bip_utils.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/bip_utils/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bip_utils.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/bip_utils/) [![GitHub License](https://img.shields.io/github/license/ebellocchia/bip_utils?label=License)](https://github.com/ebellocchia/bip_utils?tab=MIT-1-ov-file) |
 | [![Code Coverage](https://github.com/ebellocchia/bip_utils/actions/workflows/code-coverage.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/code-coverage.yml) [![Code Analysis](https://github.com/ebellocchia/bip_utils/actions/workflows/code-analysis.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/code-analysis.yml) [![Build & Test](https://github.com/ebellocchia/bip_utils/actions/workflows/test.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/test.yml) [![Test Requirements](https://github.com/ebellocchia/bip_utils/actions/workflows/test_min_reqs.yml/badge.svg)](https://github.com/ebellocchia/bip_utils/actions/workflows/test_min_reqs.yml) |
```

### Comparing `bip_utils-2.9.2/bip_utils.egg-info/SOURCES.txt` & `bip_utils-2.9.3/bip_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/bip_utils.egg-info/requires.txt` & `bip_utils-2.9.3/bip_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/keywords.txt` & `bip_utils-2.9.3/keywords.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/algorand_mnemonic.md` & `bip_utils-2.9.3/readme/algorand_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/bip32.md` & `bip_utils-2.9.3/readme/bip32.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/bip38.md` & `bip_utils-2.9.3/readme/bip38.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/bip39.md` & `bip_utils-2.9.3/readme/bip39.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/bip44.md` & `bip_utils-2.9.3/readme/bip44.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/brainwallet.md` & `bip_utils-2.9.3/readme/brainwallet.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/cardano.md` & `bip_utils-2.9.3/readme/cardano.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/electrum.md` & `bip_utils-2.9.3/readme/electrum.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/electrum_mnemonic.md` & `bip_utils-2.9.3/readme/electrum_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/electrum_v1_mnemonic.md` & `bip_utils-2.9.3/readme/electrum_v1_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/electrum_v2_mnemonic.md` & `bip_utils-2.9.3/readme/electrum_v2_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/monero.md` & `bip_utils-2.9.3/readme/monero.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/monero_mnemonic.md` & `bip_utils-2.9.3/readme/monero_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/substrate.md` & `bip_utils-2.9.3/readme/substrate.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility/addr.md` & `bip_utils-2.9.3/readme/utility/addr.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 The address library allows encoding/decoding addresses for all the supported coins.\
 `ValueError` is raised in case of errors.
 
 **Code example (coins based on the secp256k1 curve)**
 
     import binascii
     from bip_utils import *
-    
+
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"022f469a1b5498da2bc2f1e978d1e4af2ce21dd10ae5de64e4081e062f6fc6dca2")
     pub_key = Secp256k1PublicKey.FromBytes(
         binascii.unhexlify(b"022f469a1b5498da2bc2f1e978d1e4af2ce21dd10ae5de64e4081e062f6fc6dca2")
     )
-    
+
     # P2PKH address with parameters from generic configuration
     addr = P2PKHAddrEncoder.EncodeKey(pub_key,
                                       net_ver=CoinsConf.BitcoinMainNet.ParamByKey("p2pkh_net_ver"))
     # Or with custom parameters
     addr = P2PKHAddrEncoder.EncodeKey(pub_key,
                                       net_ver=b"\x01")
     # Or simply with the default parameters from BIP:
     addr = P2PKHAddrEncoder.EncodeKey(pub_key,
                                       **Bip44Conf.BitcoinMainNet.AddrParams())
     # Same as before for decoding
     pub_key_hash = P2PKHAddrDecoder.DecodeAddr(addr,
                                                net_ver=CoinsConf.BitcoinMainNet.ParamByKey("p2pkh_net_ver"))
-    
-    # Same for P2SH 
+
+    # Same for P2SH
     addr = P2SHAddrEncoder.EncodeKey(pub_key,
                                      net_ver=CoinsConf.BitcoinMainNet.ParamByKey("p2sh_net_ver"))
     addr = P2SHAddrEncoder.EncodeKey(pub_key,
                                      net_ver=b"\x01")
     addr = P2SHAddrEncoder.EncodeKey(pub_key,
                                      **Bip49Conf.BitcoinMainNet.AddrParams())
     pub_key_hash = P2SHAddrDecoder.DecodeAddr(addr,
@@ -50,15 +50,15 @@
                                      hrp=CoinsConf.BitcoinMainNet.ParamByKey("p2tr_hrp"))
     addr = P2TRAddrEncoder.EncodeKey(pub_key,
                                      hrp="hrp")
     addr = P2TRAddrEncoder.EncodeKey(pub_key,
                                      **Bip86Conf.BitcoinMainNet.AddrParams())
     pub_key_hash = P2TRAddrDecoder.DecodeAddr(addr,
                                               hrp=CoinsConf.BitcoinMainNet.ParamByKey("p2tr_hrp"))
-    
+
     # P2PKH address in Bitcoin Cash format with parameters from generic configuration
     addr = BchP2PKHAddrEncoder.EncodeKey(pub_key,
                                          hrp=CoinsConf.BitcoinCashMainNet.ParamByKey("p2pkh_std_hrp"),
                                          net_ver=CoinsConf.BitcoinCashMainNet.ParamByKey("p2pkh_std_net_ver"))
     # Or with custom parameters
     addr = BchP2PKHAddrEncoder.EncodeKey(pub_key,
                                          hrp="hrp",
@@ -78,15 +78,15 @@
                                         hrp="hrp",
                                         net_ver=b"\x01")
     addr = BchP2SHAddrEncoder.EncodeKey(pub_key,
                                         **Bip49Conf.BitcoinCashMainNet.AddrParams())
     pub_key_hash = BchP2SHAddrDecoder.DecodeAddr(addr,
                                                  hrp=CoinsConf.BitcoinCashMainNet.ParamByKey("p2sh_std_hrp"),
                                                  net_ver=CoinsConf.BitcoinCashMainNet.ParamByKey("p2sh_std_net_ver"))
-    
+
     # Ethereum address
     # Checksum encoding can be skipped to get a lower case address
     addr = EthAddrEncoder.EncodeKey(pub_key)
     pub_key_hash = EthAddrDecoder.DecodeAddr(addr)
     addr = EthAddrEncoder.EncodeKey(pub_key, skip_chksum_enc=True)
     pub_key_hash = EthAddrDecoder.DecodeAddr(addr, skip_chksum_enc=True)
     # Tron address
@@ -109,15 +109,15 @@
     addr = AtomAddrEncoder.EncodeKey(pub_key,
                                      **Bip44Conf.Cosmos.AddrParams())
     addr = AtomAddrEncoder.EncodeKey(pub_key,
                                      **Bip44Conf.Kava.AddrParams())
     # Same as before for decoding
     pub_key_hash = AtomAddrDecoder.DecodeAddr(addr,
                                               hrp=CoinsConf.Kava.ParamByKey("addr_hrp"))
-    
+
     # Filecoin address
     addr = FilSecp256k1AddrEncoder.EncodeKey(pub_key)
     pub_key_hash = FilSecp256k1AddrDecoder.DecodeAddr(addr)
     # OKEx Chain address
     addr = OkexAddrEncoder.EncodeKey(pub_key)
     pub_key_hash = OkexAddrDecoder.DecodeAddr(addr)
     # Harmony One address
@@ -130,81 +130,82 @@
     addr = ZilAddrEncoder.EncodeKey(pub_key)
     pub_key_hash = ZilAddrDecoder.DecodeAddr(addr)
 
 **Code example (coins based on the ed25519 curve)**
 
     import binascii
     from bip_utils import *
-    
+
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"00dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832")
     pub_key = Ed25519PublicKey.FromBytes(
         binascii.unhexlify(b"00dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832"))
-    
+
     # Algorand address
     addr = AlgoAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = AlgoAddrDecoder.DecodeAddr(addr)
     # Aptos address
     addr = AptosAddrEncoder.EncodeKey(pub_key)
+    addr = AptosAddrEncoder.EncodeKey(pub_key, trim_zeroes=True)
     pub_key_hash = AptosAddrDecoder.DecodeAddr(addr)
     # Elrond address
     addr = EgldAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = EgldAddrDecoder.DecodeAddr(addr)
-    
+
     # Solana address
     addr = SolAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = SolAddrDecoder.DecodeAddr(addr)
-    
+
     # Stellar address with custom parameters
     addr = XlmAddrEncoder.EncodeKey(pub_key,
                                     addr_type=XlmAddrTypes.PUB_KEY)
     # Or with the default parameters from BIP configuration:
     addr = XlmAddrEncoder.EncodeKey(pub_key,
                                     **Bip44Conf.Stellar.AddrParams())
     # Same as before for decoding
     pub_key_bytes = XlmAddrDecoder.DecodeAddr(addr,
                                               addr_type=XlmAddrTypes.PUB_KEY)
-    
+
     # Substrate address with parameters from generic configuration
     addr = SubstrateEd25519AddrEncoder.EncodeKey(pub_key,
                                                  ss58_format=CoinsConf.Polkadot.ParamByKey("addr_ss58_format"))
     # Or with custom parameters
     addr = SubstrateEd25519AddrEncoder.EncodeKey(pub_key,
                                                  ss58_format=5)
-    
+
     # Or with the default parameters from BIP/Substrate:
     addr = SubstrateEd25519AddrEncoder.EncodeKey(pub_key,
                                                  **Bip44Conf.PolkadotEd25519Slip.AddrParams())
     addr = SubstrateEd25519AddrEncoder.EncodeKey(pub_key,
                                                  **SubstrateConf.Polkadot.AddrParams())
     # Same as before for decoding
     pub_key_bytes = SubstrateEd25519AddrDecoder.DecodeAddr(addr,
                                                            ss58_format=CoinsConf.Polkadot.ParamByKey("addr_ss58_format"))
-    
+
     # Tezos address with custom parameters
     addr = XtzAddrEncoder.EncodeKey(pub_key,
                                     prefix=XtzAddrPrefixes.TZ1)
     # Or with the default parameters from BIP configuration:
     addr = XtzAddrEncoder.EncodeKey(pub_key,
                                     **Bip44Conf.Tezos.AddrParams())
     # Same as before for decoding
     pub_key_hash = XtzAddrDecoder.DecodeAddr(addr,
                                              prefix=XtzAddrPrefixes.TZ1)
 
 **Code example (coins based on the ed25519-blake2b curve)**
-    
+
     import binascii
     from bip_utils import *
 
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"00dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832")
     pub_key = Ed25519Blake2bPublicKey.FromBytes(
         binascii.unhexlify(b"00dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832")
     )
-    
+
     # Nano address
     addr = NanoAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = NanoAddrDecoder.DecodeAddr(addr)
 
 **Code example (coins based on the ed25519-monero curve)**
 
     import binascii
@@ -215,27 +216,27 @@
     pub_skey = Ed25519MoneroPublicKey.FromBytes(
         binascii.unhexlify(b"a95d2eb7e157f0a169df0a9c490dcd8e0feefb31bbf1328ca4938592a9d02422")
     )
     pub_vkey = binascii.unhexlify(b"dc2a1b478b8cc0ee655324fb8299c8904f121ab113e4216fbad6fe6d000758f5")
     pub_vkey = Ed25519MoneroPublicKey.FromBytes(
         binascii.unhexlify(b"dc2a1b478b8cc0ee655324fb8299c8904f121ab113e4216fbad6fe6d000758f5")
     )
-    
+
     # Monero address
     addr = XmrAddrEncoder.EncodeKey(pub_skey,
                                     pub_vkey=pub_vkey,
                                     net_ver=CoinsConf.MoneroMainNet.ParamByKey("addr_net_ver"))
     # Equivalent
     addr = XmrAddrEncoder.EncodeKey(pub_skey,
                                     pub_vkey=pub_vkey,
                                     net_ver=MoneroConf.MainNet.AddrNetVersion())
     # Decoding
     pub_key_bytes = XmrAddrDecoder.DecodeAddr(addr,
                                               net_ver=CoinsConf.MoneroMainNet.ParamByKey("addr_net_ver"))
-    
+
     # Monero integrated address
     addr = XmrIntegratedAddrEncoder.EncodeKey(pub_skey,
                                               pub_vkey=pub_vkey,
                                               net_ver=CoinsConf.MoneroMainNet.ParamByKey("addr_int_net_ver"),
                                               payment_id=binascii.unhexlify(b"d7af025ab223b74e"))
     # Equivalent
     addr = XmrIntegratedAddrEncoder.EncodeKey(pub_skey,
@@ -247,54 +248,54 @@
                                                         net_ver=CoinsConf.MoneroMainNet.ParamByKey("addr_int_net_ver"),
                                                         payment_id=binascii.unhexlify(b"d7af025ab223b74e"))
 
 **Code example (coins based on the ed25519-kholaw curve)**
 
     import binascii
     from bip_utils import *
-    
+
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"01f9256746c79ad5ba163ae677e3e3477471f0c3f8e1b5012c7a09f862e3972d")
     pub_key = Ed25519KholawPublicKey.FromBytes(
         binascii.unhexlify(b"0072629d389eabb6a4a6e35c9b0cab50b546b4a49a20d1d831956bd06098ba3370")
     )
-    
+
     # ADA Byron Icarus address (a chain code is also required)
     chain_code = binascii.unhexlify(b"fa8397359cea983fe2195214e96b4d9f9bc31941d973a77d2d98ac77ea186db8")
-    
+
     addr = AdaByronIcarusAddrEncoder.EncodeKey(pub_key, chain_code=chain_code)
     pub_key_hash = AdaByronAddrDecoder.DecodeAddr(addr)
-    
+
     # ADA Byron legacy address (chain code and HD data are also required)
     hd_path_key = binascii.unhexlify(b"c582f8e7cf7aeb6e5f3e96e939a92ae1642360a51d45150f34e70132a152203f")
-    
+
     addr = AdaByronLegacyAddrEncoder.EncodeKey(pub_key,
                                                chain_code=chain_code,
                                                hd_path="m/0'/0'",
                                                hd_path_key=hd_path_key)
     pub_key_hash = AdaByronAddrDecoder.DecodeAddr(addr)
-    
+
     # ADA Shelley address (a staking key is also required)
     pub_skey = binascii.unhexlify(b"7680c767b8096daa3299dc282068327c79976f346e55b72d0ffd751295a45913")
-    
+
     addr = AdaShelleyAddrEncoder.EncodeKey(pub_key,
                                            pub_skey=pub_skey,
                                            net_tag=AdaShelleyAddrNetworkTags.MAINNET)
     pub_key_hash = AdaShelleyAddrDecoder.DecodeAddr(addr)
 
 **Code example (coins based on the nist256p1 curve)**
 
     import binascii
     from bip_utils import *
 
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"038ea003d38b3f2043e681f06f56b3864d28d73b4f243aee90ed04a28dbc058c5b")
     pub_key = Nist256p1PublicKey.FromBytes(
         binascii.unhexlify(b"038ea003d38b3f2043e681f06f56b3864d28d73b4f243aee90ed04a28dbc058c5b"))
-    
+
     # NEO address with parameters from generic configuration
     addr = NeoAddrEncoder.EncodeKey(pub_key,
                                     ver=CoinsConf.Neo.ParamByKey("addr_ver"))
     # Or with custom parameters
     addr = NeoAddrEncoder.EncodeKey(pub_key,
                                     ver=b"\x10")
     # Or with the default parameters from BIP configuration:
@@ -309,15 +310,15 @@
     import binascii
     from bip_utils import *
 
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832")
     pub_key = Sr25519PublicKey.FromBytes(
         binascii.unhexlify(b"dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832"))
-    
+
     # Substrate address (like before)
     addr = SubstrateSr25519AddrEncoder.EncodeKey(pub_key,
                                                  ss58_format=CoinsConf.Kusama.ParamByKey("addr_ss58_format"))
     addr = SubstrateSr25519AddrEncoder.EncodeKey(pub_key,
                                                  ss58_format=3)
     addr = SubstrateSr25519AddrEncoder.EncodeKey(pub_key,
                                                  **SubstrateConf.Kusama.AddrParams())
```

### Comparing `bip_utils-2.9.2/readme/utility/base58.md` & `bip_utils-2.9.3/readme/utility/base58.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility/bch_addr_converter.md` & `bip_utils-2.9.3/readme/utility/bch_addr_converter.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility/bech32.md` & `bip_utils-2.9.3/readme/utility/bech32.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility/slip32.md` & `bip_utils-2.9.3/readme/utility/slip32.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility/solana_spl.md` & `bip_utils-2.9.3/readme/utility/solana_spl.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility/wif.md` & `bip_utils-2.9.3/readme/utility/wif.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/readme/utility_libs.md` & `bip_utils-2.9.3/readme/utility_libs.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/requirements.txt` & `bip_utils-2.9.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.9.2/setup.py` & `bip_utils-2.9.3/setup.py`

 * *Files identical despite different names*

