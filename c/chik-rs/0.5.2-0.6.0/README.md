# Comparing `tmp/chik_rs-0.5.2.tar.gz` & `tmp/chik_rs-0.6.0.tar.gz`

## Comparing `chik_rs-0.5.2.tar` & `chik_rs-0.6.0.tar`

### file list

```diff
@@ -1,211 +1,126 @@
--rw-r--r--   0     1001      127     1157 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/Cargo.toml
--rw-r--r--   0     1001      127     7051 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/block_record.rs
--rw-r--r--   0     1001      127    17089 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/bytes.rs
--rw-r--r--   0     1001      127     5022 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/chik_protocol.rs
--rw-r--r--   0     1001      127     1229 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/classgroup.rs
--rw-r--r--   0     1001      127     4441 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/coin.rs
--rw-r--r--   0     1001      127      225 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      127      209 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/coin_state.rs
--rw-r--r--   0     1001      127      424 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      127      552 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      127     2000 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/foliage.rs
--rw-r--r--   0     1001      127     2870 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/full_node_protocol.rs
--rw-r--r--   0     1001      127     4369 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/fullblock.rs
--rw-r--r--   0     1001      127     3532 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/header_block.rs
--rw-r--r--   0     1001      127     1397 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/lazy_node.rs
--rw-r--r--   0     1001      127     1479 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/lib.rs
--rw-r--r--   0     1001      127     1687 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/message_struct.rs
--rw-r--r--   0     1001      127      169 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/peer_info.rs
--rw-r--r--   0     1001      127      221 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/pool_target.rs
--rw-r--r--   0     1001      127    17547 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/program.rs
--rw-r--r--   0     1001      127      346 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      127     1991 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      127     1472 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/slots.rs
--rw-r--r--   0     1001      127     8271 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      127      471 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/sub_epoch_summary.rs
--rw-r--r--   0     1001      127     2343 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/unfinished_block.rs
--rw-r--r--   0     1001      127      360 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/vdf.rs
--rw-r--r--   0     1001      127     3644 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      127     2371 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-protocol/src/weight_proof.rs
--rw-r--r--   0     1001      127     2028 2024-02-21 13:21:40.000000 chik_rs-0.5.2/Cargo.toml
--rw-r--r--   0     1001      127      625 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/Cargo.toml
--rw-r--r--   0     1001      127      839 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/src/chik_error.rs
--rw-r--r--   0     1001      127     2346 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/src/from_json_dict.rs
--rw-r--r--   0     1001      127     2474 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/src/int.rs
--rw-r--r--   0     1001      127      457 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/src/lib.rs
--rw-r--r--   0     1001      127    20446 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/src/streamable.rs
--rw-r--r--   0     1001      127     1892 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-traits/src/to_json_dict.rs
--rw-r--r--   0     1001      127      785 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/Cargo.toml
--rw-r--r--   0     1001      127     6089 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/derive_synthetic.rs
--rw-r--r--   0     1001      127      114 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/lib.rs
--rw-r--r--   0     1001      127      710 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/proof.rs
--rw-r--r--   0     1001      127    11368 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles/cat.rs
--rw-r--r--   0     1001      127     4509 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles/did.rs
--rw-r--r--   0     1001      127    13636 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles/nft.rs
--rw-r--r--   0     1001      127     2711 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles/offer.rs
--rw-r--r--   0     1001      127     4721 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles/singleton.rs
--rw-r--r--   0     1001      127     3086 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles/standard.rs
--rw-r--r--   0     1001      127      427 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-wallet/src/puzzles.rs
--rw-r--r--   0     1001      127      518 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127     5782 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127      441 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-derive/Cargo.toml
--rw-r--r--   0     1001      127    10152 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-derive/src/from_klvm.rs
--rw-r--r--   0     1001      127     2602 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-derive/src/helpers.rs
--rw-r--r--   0     1001      127      603 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-derive/src/lib.rs
--rw-r--r--   0     1001      127     1217 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-derive/src/macros.rs
--rw-r--r--   0     1001      127     7548 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-derive/src/to_klvm.rs
--rw-r--r--   0     1001      127      465 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-utils/Cargo.toml
--rw-r--r--   0     1001      127     2069 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-utils/src/curried_program.rs
--rw-r--r--   0     1001      127     1899 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-utils/src/curry_tree_hash.rs
--rw-r--r--   0     1001      127      806 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-utils/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-utils/src/tree_hash.rs
--rw-r--r--   0     1001      127      224 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.cargo/config
--rw-r--r--   0     1001      127      290 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.github/workflows/audit-check.yml.bak
--rw-r--r--   0     1001      127     3029 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.github/workflows/benchmark.yml.bak
--rw-r--r--   0     1001      127     5031 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.github/workflows/build-crate-and-npm.yml
--rw-r--r--   0     1001      127     4212 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.github/workflows/build-riscv64.yml
--rw-r--r--   0     1001      127    15324 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.github/workflows/build-test.yml
--rw-r--r--   0     1001      127       15 2024-02-21 13:21:40.000000 chik_rs-0.5.2/.gitignore
--rw-r--r--   0     1001      127    11357 2024-02-21 13:21:40.000000 chik_rs-0.5.2/LICENSE
--rw-r--r--   0     1001      127      192 2024-02-21 13:21:40.000000 chik_rs-0.5.2/README.md
--rw-r--r--   0     1001      127     3146 2024-02-21 13:21:40.000000 chik_rs-0.5.2/benches/run-generator.rs
--rw-r--r--   0     1001      127     1671 2024-02-21 13:21:40.000000 chik_rs-0.5.2/benches/tree-hash.rs
--rw-r--r--   0     1001      127     1713 2024-02-21 13:21:40.000000 chik_rs-0.5.2/bump-version.py
--rw-r--r--   0     1001      127      142 2024-02-21 13:21:40.000000 chik_rs-0.5.2/cl/README.md
--rw-r--r--   0     1001      127     4603 2024-02-21 13:21:40.000000 chik_rs-0.5.2/cl/deserialize_w_backrefs.cl
--rw-r--r--   0     1001      127     4474 2024-02-21 13:21:40.000000 chik_rs-0.5.2/docs/implementation-notes.md
--rw-r--r--   0     1001      127     6297 2024-02-21 13:21:40.000000 chik_rs-0.5.2/ff-tests/bb13.spend
--rw-r--r--   0     1001      127     6297 2024-02-21 13:21:40.000000 chik_rs-0.5.2/ff-tests/e3c0.spend
--rw-r--r--   0     1001      127     2184 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/assert-puzzle-announce-fail.txt
--rw-r--r--   0     1001      127   777146 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-1ee588dc.txt
--rw-r--r--   0     1001      127   468780 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-225758.env
--rw-r--r--   0     1001      127     8068 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-225758.txt
--rw-r--r--   0     1001      127    80742 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-4671894.env
--rw-r--r--   0     1001      127   531620 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-4671894.txt
--rw-r--r--   0     1001      127   776352 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-6fe59b24.txt
--rw-r--r--   0     1001      127    12107 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834752-compressed.txt
--rw-r--r--   0     1001      127    28444 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834752.txt
--rw-r--r--   0     1001      127   132615 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834760.txt
--rw-r--r--   0     1001      127    26930 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834761.txt
--rw-r--r--   0     1001      127    74748 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834765.txt
--rw-r--r--   0     1001      127   124696 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834766.txt
--rw-r--r--   0     1001      127   104382 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-834768.txt
--rw-r--r--   0     1001      127   764957 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-b45268ac.txt
--rw-r--r--   0     1001      127   824220 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-c2a8df0d.txt
--rw-r--r--   0     1001      127   772549 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/block-e5002df2.txt
--rw-r--r--   0     1001      127      665 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/create-coin-different-amounts.txt
--rw-r--r--   0     1001      127      425 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/create-coin-hint-duplicate-outputs.txt
--rw-r--r--   0     1001      127      808 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/create-coin-hint.txt
--rw-r--r--   0     1001      127      832 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/create-coin-hint2.txt
--rw-r--r--   0     1001      127      321 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/deep-recursion-plus.txt
--rw-r--r--   0     1001      127      413 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/double-spend.txt
--rw-r--r--   0     1001      127      413 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-coin-announce.txt
--rw-r--r--   0     1001      127      405 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-create-coin.txt
--rw-r--r--   0     1001      127      556 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-height-absolute-div.txt
--rw-r--r--   0     1001      127      601 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-height-absolute-substr-tail.txt
--rw-r--r--   0     1001      127      589 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-height-absolute-substr.txt
--rw-r--r--   0     1001      127      556 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-height-absolute.txt
--rw-r--r--   0     1001      127      556 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-height-relative.txt
--rw-r--r--   0     1001      127      281 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-outputs.txt
--rw-r--r--   0     1001      127      556 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-reserve-fee.txt
--rw-r--r--   0     1001      127      556 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-seconds-absolute.txt
--rw-r--r--   0     1001      127      557 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/duplicate-seconds-relative.txt
--rw-r--r--   0     1001      127      546 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/height-absolute-ladder.txt
--rw-r--r--   0     1001      127      171 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/infinite-recursion1.txt
--rw-r--r--   0     1001      127      155 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/infinite-recursion2.txt
--rw-r--r--   0     1001      127     1431 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/infinite-recursion3.txt
--rw-r--r--   0     1001      127      219 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/infinite-recursion4.txt
--rw-r--r--   0     1001      127      110 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/invalid-conditions.txt
--rw-r--r--   0     1001      127     2380 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/just-puzzle-announce.txt
--rw-r--r--   0     1001      127   590784 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/many-create-coin.txt
--rw-r--r--   0     1001      127      796 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/many-large-ints-negative.txt
--rw-r--r--   0     1001      127      612 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/many-large-ints.txt
--rw-r--r--   0     1001      127      559 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/max-height.txt
--rw-r--r--   0     1001      127      373 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/multiple-reserve-fee.txt
--rw-r--r--   0     1001      127      598 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/negative-reserve-fee.txt
--rw-r--r--   0     1001      127      273 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/recursion-pairs.txt
--rw-r--r--   0     1001      127      367 2024-02-21 13:21:40.000000 chik_rs-0.5.2/generator-tests/unknown-condition.txt
--rw-r--r--   0     1001      127       93 2024-02-21 13:21:40.000000 chik_rs-0.5.2/mypy.ini
--rw-r--r--   0     1001      127      266 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/allocator.rs
--rw-r--r--   0     1001      127     1712 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/compression/compressor.rs
--rw-r--r--   0     1001      127      858 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/compression/deserialize_w_backrefs.bin
--rw-r--r--   0     1001      127       20 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/compression/mod.rs
--rw-r--r--   0     1001      127     1228 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/error.rs
--rw-r--r--   0     1001      127    17249 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/fast_forward.rs
--rw-r--r--   0     1001      127     3075 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/coin_id.rs
--rw-r--r--   0     1001      127     4489 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      127   154041 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/conditions.rs
--rw-r--r--   0     1001      127     1584 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/flags.rs
--rw-r--r--   0     1001      127     6454 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      127      462 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/mod.rs
--rw-r--r--   0     1001      127    10104 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/opcodes.rs
--rw-r--r--   0     1001      127     6578 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      127     2033 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      127     2916 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      127    10937 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/solution_generator.rs
--rw-r--r--   0     1001      127      471 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/spend_visitor.rs
--rw-r--r--   0     1001      127     9135 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/test_generators.rs
--rw-r--r--   0     1001      127     6133 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/gen/validation_error.rs
--rw-r--r--   0     1001      127     3133 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/generator_rom.rs
--rw-r--r--   0     1001      127      133 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/lib.rs
--rw-r--r--   0     1001      127    22644 2024-02-21 13:21:40.000000 chik_rs-0.5.2/src/merkle_set.rs
--rw-r--r--   0     1001      127    16295 2024-02-21 13:21:40.000000 chik_rs-0.5.2/test-bundles/1000101.bundle
--rw-r--r--   0     1001      127     3469 2024-02-21 13:21:40.000000 chik_rs-0.5.2/test-bundles/3000253.bundle
--rwxr-xr-x   0     1001      127     8264 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/generate-programs.py
--rwxr-xr-x   0     1001      127     3079 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/run-programs.py
--rwxr-xr-x   0     1001      127     1569 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/run.py
--rwxr-xr-x   0     1001      127     4015 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/run_gen.py
--rwxr-xr-x   0     1001      127     4076 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test-generators.py
--rw-r--r--   0     1001      127     3801 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_block_record_fidelity.py
--rw-r--r--   0     1001      127    23047 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_blspy_fidelity.py
--rw-r--r--   0     1001      127    11414 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_coin.py
--rw-r--r--   0     1001      127     1012 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_fast_forward.py
--rw-r--r--   0     1001      127     3499 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_program_fidelity.py
--rw-r--r--   0     1001      127     1217 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_replace.py
--rw-r--r--   0     1001      127     1947 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_run_block_generator.py
--rw-r--r--   0     1001      127     5657 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_run_puzzle.py
--rw-r--r--   0     1001      127    12592 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_spend_bundle.py
--rw-r--r--   0     1001      127    15889 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_streamable.py
--rw-r--r--   0     1001      127     1050 2024-02-21 13:21:40.000000 chik_rs-0.5.2/tests/test_tree_hash.py
--rw-r--r--   0     1001      127     1287 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/Cargo.toml
--rw-r--r--   0     1001      127     2115 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/README.md
--rw-r--r--   0     1001      127     1389 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/benches/derive_key.rs
--rw-r--r--   0     1001      127     1356 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/benches/parse.rs
--rw-r--r--   0     1001      127      828 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/benches/sign.rs
--rw-r--r--   0     1001      127     1023 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/benches/verify.rs
--rw-r--r--   0     1001      127       78 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/derivable_key.rs
--rw-r--r--   0     1001      127     1500 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/derive_keys.rs
--rw-r--r--   0     1001      127     1114 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/error.rs
--rw-r--r--   0     1001      127     4267 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/gtelement.rs
--rw-r--r--   0     1001      127      565 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/lib.rs
--rw-r--r--   0     1001      127     4509 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/mnemonic.rs
--rw-r--r--   0     1001      127    26579 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/public_key.rs
--rw-r--r--   0     1001      127    19133 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/secret_key.rs
--rw-r--r--   0     1001      127    41483 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik-bls/src/signature.rs
--rw-r--r--   0     1001      127      835 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/Cargo.toml
--rw-r--r--   0     1001      127     6975 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/docs/derive_macros.md
--rw-r--r--   0     1001      127     1067 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/error.rs
--rw-r--r--   0     1001      127     9955 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/from_klvm.rs
--rw-r--r--   0     1001      127     1738 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/klvm_decoder.rs
--rw-r--r--   0     1001      127     1518 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/klvm_encoder.rs
--rw-r--r--   0     1001      127     5612 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/lib.rs
--rw-r--r--   0     1001      127     3246 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/macros.rs
--rw-r--r--   0     1001      127     1017 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/match_byte.rs
--rw-r--r--   0     1001      127     8530 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/to_klvm.rs
--rw-r--r--   0     1001      127      670 2024-02-21 13:21:40.000000 chik_rs-0.5.2/klvm-traits/src/wrappers.rs
--rw-r--r--   0     1001      127      506 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127    13873 2024-02-21 13:21:40.000000 chik_rs-0.5.2/chik_py_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 chik_rs-0.5.2/wheel/Cargo.toml
--rw-r--r--   0     1001      127       77 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/README.md
--rw-r--r--   0     1001      127   147700 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/chik_rs.pyi
--rw-r--r--   0     1001      127    15122 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/generate_type_stubs.py
--rw-r--r--   0     1001      127        0 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/py.typed
--rw-r--r--   0     1001      127      559 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/src/adapt_response.rs
--rw-r--r--   0     1001      127    17723 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/src/api.rs
--rw-r--r--   0     1001      127      641 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/src/compression.rs
--rw-r--r--   0     1001      127      175 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/src/lib.rs
--rw-r--r--   0     1001      127     8386 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/src/run_generator.rs
--rw-r--r--   0     1001      127     1772 2024-02-21 13:21:40.000000 chik_rs-0.5.2/wheel/src/run_program.rs
--rw-r--r--   0     1001      127    28496 2024-02-21 13:21:49.000000 chik_rs-0.5.2/wheel/Cargo.lock
--rw-r--r--   0        0        0      147 1970-01-01 00:00:00.000000 chik_rs-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chik_rs-0.5.2/PKG-INFO
+-rw-r--r--   0     1001      127      516 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127     9355 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127     1267 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/Cargo.toml
+-rw-r--r--   0     1001      127     2115 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/README.md
+-rw-r--r--   0     1001      127     1389 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/benches/derive_key.rs
+-rw-r--r--   0     1001      127     1356 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/benches/parse.rs
+-rw-r--r--   0     1001      127      828 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/benches/sign.rs
+-rw-r--r--   0     1001      127     1023 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/benches/verify.rs
+-rw-r--r--   0     1001      127       78 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/derivable_key.rs
+-rw-r--r--   0     1001      127     1500 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/derive_keys.rs
+-rw-r--r--   0     1001      127     1114 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/error.rs
+-rw-r--r--   0     1001      127     4267 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/gtelement.rs
+-rw-r--r--   0     1001      127      565 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/lib.rs
+-rw-r--r--   0     1001      127     4484 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/mnemonic.rs
+-rw-r--r--   0     1001      127    26579 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/public_key.rs
+-rw-r--r--   0     1001      127    19133 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/secret_key.rs
+-rw-r--r--   0     1001      127    41458 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-bls/src/signature.rs
+-rw-r--r--   0     1001      127      759 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/Cargo.toml
+-rw-r--r--   0     1001      127     6089 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/derive_synthetic.rs
+-rw-r--r--   0     1001      127      114 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/lib.rs
+-rw-r--r--   0     1001      127      710 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/proof.rs
+-rw-r--r--   0     1001      127    11363 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles/cat.rs
+-rw-r--r--   0     1001      127     4507 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles/did.rs
+-rw-r--r--   0     1001      127    13636 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles/nft.rs
+-rw-r--r--   0     1001      127     2711 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles/offer.rs
+-rw-r--r--   0     1001      127     4717 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles/singleton.rs
+-rw-r--r--   0     1001      127     3082 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles/standard.rs
+-rw-r--r--   0     1001      127      427 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-wallet/src/puzzles.rs
+-rw-r--r--   0     1001      127      809 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/Cargo.toml
+-rw-r--r--   0     1001      127     6975 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/docs/derive_macros.md
+-rw-r--r--   0     1001      127     1067 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/error.rs
+-rw-r--r--   0     1001      127    10142 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/from_klvm.rs
+-rw-r--r--   0     1001      127     1742 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/klvm_decoder.rs
+-rw-r--r--   0     1001      127     1518 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/klvm_encoder.rs
+-rw-r--r--   0     1001      127     5612 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/lib.rs
+-rw-r--r--   0     1001      127     3246 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/macros.rs
+-rw-r--r--   0     1001      127     1026 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/match_byte.rs
+-rw-r--r--   0     1001      127     8530 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/to_klvm.rs
+-rw-r--r--   0     1001      127      670 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-traits/src/wrappers.rs
+-rw-r--r--   0     1001      127      415 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-derive/Cargo.toml
+-rw-r--r--   0     1001      127    10152 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-derive/src/from_klvm.rs
+-rw-r--r--   0     1001      127     2602 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-derive/src/helpers.rs
+-rw-r--r--   0     1001      127      603 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-derive/src/lib.rs
+-rw-r--r--   0     1001      127     1217 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-derive/src/macros.rs
+-rw-r--r--   0     1001      127     7548 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-derive/src/to_klvm.rs
+-rw-r--r--   0     1001      127     1134 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/Cargo.toml
+-rw-r--r--   0     1001      127     4313 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/README.md
+-rw-r--r--   0     1001      127     3186 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/benches/run-generator.rs
+-rw-r--r--   0     1001      127     2182 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/benches/tree-hash.rs
+-rw-r--r--   0     1001      127      266 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/allocator.rs
+-rw-r--r--   0     1001      127     1228 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/error.rs
+-rw-r--r--   0     1001      127    17250 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/fast_forward.rs
+-rw-r--r--   0     1001      127     3075 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/coin_id.rs
+-rw-r--r--   0     1001      127     6868 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      127   192415 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/conditions.rs
+-rw-r--r--   0     1001      127     1719 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/flags.rs
+-rw-r--r--   0     1001      127     6437 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      127     9639 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/messages.rs
+-rw-r--r--   0     1001      127      480 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/mod.rs
+-rw-r--r--   0     1001      127    11894 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/opcodes.rs
+-rw-r--r--   0     1001      127     6795 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      127     2017 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      127     2944 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      127    10908 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/solution_generator.rs
+-rw-r--r--   0     1001      127      471 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/spend_visitor.rs
+-rw-r--r--   0     1001      127     9411 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/test_generators.rs
+-rw-r--r--   0     1001      127     6371 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/gen/validation_error.rs
+-rw-r--r--   0     1001      127     3133 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/generator_rom.rs
+-rw-r--r--   0     1001      127      152 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/lib.rs
+-rw-r--r--   0     1001      127    22644 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-consensus/src/merkle_set.rs
+-rw-r--r--   0     1001      127     1151 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/Cargo.toml
+-rw-r--r--   0     1001      127     7024 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/block_record.rs
+-rw-r--r--   0     1001      127    17338 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/bytes.rs
+-rw-r--r--   0     1001      127     4997 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/chik_protocol.rs
+-rw-r--r--   0     1001      127     1208 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      127     4453 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/coin.rs
+-rw-r--r--   0     1001      127      199 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      127      182 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      127      397 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      127      531 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      127     1983 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/foliage.rs
+-rw-r--r--   0     1001      127     3226 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/full_node_protocol.rs
+-rw-r--r--   0     1001      127     4342 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      127     3505 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/header_block.rs
+-rw-r--r--   0     1001      127     1406 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/lazy_node.rs
+-rw-r--r--   0     1001      127     1455 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/lib.rs
+-rw-r--r--   0     1001      127      142 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/peer_info.rs
+-rw-r--r--   0     1001      127      195 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      127    17472 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/program.rs
+-rw-r--r--   0     1001      127      319 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      127     1967 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      127     1458 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/slots.rs
+-rw-r--r--   0     1001      127     8260 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      127      449 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/sub_epoch_summary.rs
+-rw-r--r--   0     1001      127     2343 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/unfinished_block.rs
+-rw-r--r--   0     1001      127      338 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/vdf.rs
+-rw-r--r--   0     1001      127     4071 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      127     2361 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-protocol/src/weight_proof.rs
+-rw-r--r--   0     1001      127      625 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/Cargo.toml
+-rw-r--r--   0     1001      127      839 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/src/chik_error.rs
+-rw-r--r--   0     1001      127     2346 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/src/from_json_dict.rs
+-rw-r--r--   0     1001      127     2480 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/src/int.rs
+-rw-r--r--   0     1001      127      457 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/src/lib.rs
+-rw-r--r--   0     1001      127    20419 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/src/streamable.rs
+-rw-r--r--   0     1001      127     1892 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik-traits/src/to_json_dict.rs
+-rw-r--r--   0     1001      127      454 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127    13876 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/chik_py_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127      471 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-utils/Cargo.toml
+-rw-r--r--   0     1001      127     2069 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-utils/src/curried_program.rs
+-rw-r--r--   0     1001      127     1899 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-utils/src/curry_tree_hash.rs
+-rw-r--r--   0     1001      127      806 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-utils/src/lib.rs
+-rw-r--r--   0     1001      127     9843 2024-04-15 01:57:53.000000 chik_rs-0.6.0/crates/klvm-utils/src/tree_hash.rs
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 chik_rs-0.6.0/wheel/Cargo.toml
+-rw-r--r--   0     1001      127       77 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/README.md
+-rw-r--r--   0     1001      127   147712 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/chik_rs.pyi
+-rw-r--r--   0     1001      127    15138 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/generate_type_stubs.py
+-rw-r--r--   0     1001      127        0 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/py.typed
+-rw-r--r--   0     1001      127      364 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/src/adapt_response.rs
+-rw-r--r--   0     1001      127    17725 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/src/api.rs
+-rw-r--r--   0     1001      127      158 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/src/lib.rs
+-rw-r--r--   0     1001      127     8579 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/src/run_generator.rs
+-rw-r--r--   0     1001      127     1788 2024-04-15 01:57:53.000000 chik_rs-0.6.0/wheel/src/run_program.rs
+-rw-r--r--   0     1001      127    72089 2024-04-15 01:57:53.000000 chik_rs-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 chik_rs-0.6.0/Cargo.toml
+-rw-r--r--   0        0        0      184 1970-01-01 00:00:00.000000 chik_rs-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 chik_rs-0.6.0/PKG-INFO
```

### Comparing `chik_rs-0.5.2/chik-protocol/Cargo.toml` & `chik_rs-0.6.0/crates/chik-protocol/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [package]
 name = "chik-protocol"
-version = "0.5.1"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik network protocol message types"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
-homepage = "https://github.com/Chik-Network/chik_rs/chik-protocol/"
-repository = "https://github.com/Chik-Network/chik_rs/chik-protocol/"
+homepage = "https://github.com/Chik-Network/chik_rs"
+repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
-py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro", "chik-traits/py-bindings"]
+py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro", "chik-traits/py-bindings", "chik-bls/py-bindings"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["multiple-pymethods", "num-bigint"], optional = true }
 sha2 = "0.10.8"
 hex = "0.4.3"
-chik_streamable_macro = { version = "0.3.0", path = "../chik_streamable_macro" }
-chik_py_streamable_macro = { version = "0.5.1", path = "../chik_py_streamable_macro", optional = true }
-klvmr = "0.5.0"
-chik-traits = { version = "0.5.1", path = "../chik-traits" }
-klvm-traits = { version = "0.5.1", path = "../klvm-traits", features = ["derive"] }
-klvm-utils = { version = "0.5.1", path = "../klvm-utils" }
-chik-bls = { version = "0.5.1", path = "../chik-bls" }
+chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
+chik_py_streamable_macro = { version = "0.6.0", path = "../chik_py_streamable_macro", optional = true }
+klvmr = "0.6.1"
+chik-traits = { version = "0.6.0", path = "../chik-traits" }
+klvm-traits = { version = "0.6.0", path = "../klvm-traits", features = ["derive"] }
+klvm-utils = { version = "0.6.0", path = "../klvm-utils" }
+chik-bls = { version = "0.6.0", path = "../chik-bls" }
 arbitrary = { version = "1.3.0", features = ["derive"] }
 
 [dev-dependencies]
 rstest = "0.17.0"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/block_record.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/block_record.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
-use crate::streamable_struct;
 use crate::{Bytes32, ClassgroupElement, Coin, SubEpochSummary};
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
 // This class is not included or hashed into the blockchain, but it is kept in memory as a more
 // efficient way to maintain data about the blockchain. This allows us to validate future blocks,
 // difficulty adjustments, etc, without saving the whole header block in memory.
-streamable_struct! (BlockRecord {
+#[streamable]
+pub struct BlockRecord {
     header_hash: Bytes32,
     // Header hash of the previous block
     prev_hash: Bytes32,
     height: u32,
     // Total cumulative difficulty of all ancestor blocks since genesis
     weight: u128,
     // Total number of VDF iterations since genesis, including this block
@@ -49,15 +49,15 @@
     // Slot (present iff this is the first SB in sub slot)
     finished_challenge_slot_hashes: Option<Vec<Bytes32>>,
     finished_infused_challenge_slot_hashes: Option<Vec<Bytes32>>,
     finished_reward_slot_hashes: Option<Vec<Bytes32>>,
 
     // Sub-epoch (present iff this is the first SB after sub-epoch)
     sub_epoch_summary_included: Option<SubEpochSummary>,
-});
+}
 
 impl BlockRecord {
     pub fn is_transaction_block(&self) -> bool {
         self.timestamp.is_some()
     }
 
     pub fn first_in_sub_slot(&self) -> bool {
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/bytes.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/bytes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 use chik_traits::{chik_error, read_bytes, Streamable};
 use klvm_traits::{FromKlvm, FromKlvmError, KlvmDecoder, KlvmEncoder, ToKlvm, ToKlvmError};
 use sha2::{Digest, Sha256};
 use std::array::TryFromSliceError;
-use std::convert::{AsRef, TryInto};
 use std::fmt;
 use std::io::Cursor;
 use std::ops::Deref;
 
 #[cfg(feature = "py-bindings")]
 use chik_traits::{ChikToPython, FromJsonDict, ToJsonDict};
 #[cfg(feature = "py-bindings")]
@@ -110,15 +109,15 @@
         encoder.encode_atom(self.0.as_slice())
     }
 }
 
 impl<N> FromKlvm<N> for Bytes {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let bytes = decoder.decode_atom(&node)?;
-        Ok(Self(bytes.to_vec()))
+        Ok(Self(bytes.as_ref().to_vec()))
     }
 }
 
 impl From<&[u8]> for Bytes {
     fn from(value: &[u8]) -> Self {
         Self(value.to_vec())
     }
@@ -243,21 +242,21 @@
         encoder.encode_atom(self.0.as_slice())
     }
 }
 
 impl<N, const LEN: usize> FromKlvm<N> for BytesImpl<LEN> {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let bytes = decoder.decode_atom(&node)?;
-        if bytes.len() != LEN {
+        if bytes.as_ref().len() != LEN {
             return Err(FromKlvmError::WrongAtomLength {
                 expected: LEN,
-                found: bytes.len(),
+                found: bytes.as_ref().len(),
             });
         }
-        Ok(Self::try_from(bytes).unwrap())
+        Ok(Self::try_from(bytes.as_ref()).unwrap())
     }
 }
 
 impl<const N: usize> TryFrom<&[u8]> for BytesImpl<N> {
     type Error = TryFromSliceError;
 
     fn try_from(value: &[u8]) -> Result<Self, TryFromSliceError> {
@@ -355,15 +354,21 @@
         PyBytes::new(py, &self.0).into()
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> ChikToPython for BytesImpl<N> {
     fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        Ok(PyBytes::new(py, &self.0).into())
+        if N == 32 {
+            let bytes_module = PyModule::import(py, "chik.types.blockchain_format.sized_bytes")?;
+            let ty = bytes_module.getattr("bytes32")?;
+            ty.call1((self.0.into_py(py),))
+        } else {
+            Ok(PyBytes::new(py, &self.0).into())
+        }
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<'py, const N: usize> FromPyObject<'py> for BytesImpl<N> {
     fn extract(obj: &'py PyAny) -> PyResult<Self> {
         let b = <PyBytes as PyTryFrom>::try_from(obj)?;
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/chik_protocol.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/chik_protocol.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::{streamable, Streamable};
 
-use crate::message_struct;
-use crate::streamable_struct;
 use crate::Bytes;
 
 #[cfg(feature = "py-bindings")]
 use chik_py_streamable_macro::{PyJsonDict, PyStreamable};
 
 #[repr(u8)]
 #[cfg_attr(feature = "py-bindings", derive(PyJsonDict, PyStreamable))]
@@ -151,27 +149,29 @@
 #[cfg(feature = "py-bindings")]
 impl chik_traits::ChikToPython for NodeType {
     fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
         Ok(pyo3::IntoPy::into_py(*self, py).into_ref(py))
     }
 }
 
-streamable_struct! (Message {
+#[streamable]
+pub struct Message {
     msg_type: ProtocolMessageTypes,
     id: Option<u16>,
     data: Bytes,
-});
+}
 
-message_struct! (Handshake {
+#[streamable(message)]
+pub struct Handshake {
     // Network id, usually the genesis challenge of the blockchain
     network_id: String,
     // Protocol version to determine which messages the peer supports
     protocol_version: String,
     // Version of the software, to debug and determine feature support
     software_version: String,
     // Which port the server is listening on
     server_port: u16,
     // NodeType (full node, wallet, farmer, etc.)
     node_type: NodeType,
     // Key value dict to signal support for additional capabilities/features
     capabilities: Vec<(u16, String)>,
-});
+}
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/classgroup.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/classgroup.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-use crate::streamable_struct;
 use crate::Bytes100;
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
-streamable_struct!(ClassgroupElement { data: Bytes100 });
+#[streamable]
+pub struct ClassgroupElement {
+    data: Bytes100,
+}
 
 impl ClassgroupElement {
     pub fn get_default_element() -> ClassgroupElement {
         let mut data = [0_u8; 100];
         data[0] = 0x08;
         ClassgroupElement { data: data.into() }
     }
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/coin.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/coin.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-use crate::streamable_struct;
 use crate::{bytes::Bytes32, BytesImpl};
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 use klvm_traits::{
     destructure_list, klvm_list, match_list, FromKlvm, FromKlvmError, KlvmDecoder, KlvmEncoder,
     ToKlvm, ToKlvmError,
 };
 use sha2::{Digest, Sha256};
-use std::convert::TryInto;
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
-streamable_struct!(Coin {
+#[streamable]
+pub struct Coin {
     parent_coin_info: Bytes32,
     puzzle_hash: Bytes32,
     amount: u64,
-});
+}
 
 impl Coin {
-    pub fn coin_id(&self) -> [u8; 32] {
+    pub fn coin_id(&self) -> Bytes32 {
         let mut hasher = Sha256::new();
         hasher.update(self.parent_coin_info);
         hasher.update(self.puzzle_hash);
 
         let amount_bytes = self.amount.to_be_bytes();
         if self.amount >= 0x8000000000000000_u64 {
             hasher.update([0_u8]);
@@ -38,15 +37,16 @@
                 n if n >= 0x80_u64 => 6,
                 n if n > 0 => 7,
                 _ => 8,
             };
             hasher.update(&amount_bytes[start..]);
         }
 
-        hasher.finalize().as_slice().try_into().unwrap()
+        let coin_id: [u8; 32] = hasher.finalize().as_slice().try_into().unwrap();
+        Bytes32::new(coin_id)
     }
 }
 
 #[cfg(feature = "py-bindings")]
 #[pymethods]
 impl Coin {
     fn name<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
@@ -107,15 +107,15 @@
         let puzzle_hash = b"---bar---                       ";
 
         let c = Coin::new(parent_coin.into(), puzzle_hash.into(), amount);
         let mut sha256 = Sha256::new();
         sha256.update(parent_coin);
         sha256.update(puzzle_hash);
         sha256.update(bytes);
-        assert_eq!(c.coin_id(), &sha256.finalize() as &[u8]);
+        assert_eq!(c.coin_id().to_bytes(), &sha256.finalize() as &[u8]);
     }
 
     #[test]
     fn coin_roundtrip() {
         let a = &mut Allocator::new();
         let expected = "ffa09e144397decd2b831551f9710c17ae776d9c5a3ae5283c5f9747263fd1255381ffa0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ff0180";
         let expected_bytes = hex::decode(expected).unwrap();
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/foliage.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/foliage.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
-use crate::streamable_struct;
 use crate::Bytes32;
 use crate::Coin;
 use crate::PoolTarget;
 use chik_bls::G2Element;
 
-streamable_struct! (TransactionsInfo {
+#[streamable]
+pub struct TransactionsInfo {
     // Information that goes along with each transaction block
     generator_root: Bytes32, // sha256 of the block generator in this block
     generator_refs_root: Bytes32, // sha256 of the concatenation of the generator ref list entries
     aggregated_signature: G2Element,
     fees: u64, // This only includes user fees, not block rewards
     cost: u64, // This is the total cost of this block, including KLVM cost, cost of program size and conditions
     reward_claims_incorporated: Vec<Coin>, // These can be in any order
-});
+}
 
-streamable_struct!(FoliageTransactionBlock {
+#[streamable]
+pub struct FoliageTransactionBlock {
     // Information that goes along with each transaction block that is relevant for light clients
     prev_transaction_block_hash: Bytes32,
     timestamp: u64,
     filter_hash: Bytes32,
     additions_root: Bytes32,
     removals_root: Bytes32,
     transactions_info_hash: Bytes32,
-});
+}
 
-streamable_struct! (FoliageBlockData {
+#[streamable]
+pub struct FoliageBlockData {
     // Part of the block that is signed by the plot key
     unfinished_reward_block_hash: Bytes32,
     pool_target: PoolTarget,
     pool_signature: Option<G2Element>, // Iff ProofOfSpace has a pool pk
     farmer_reward_puzzle_hash: Bytes32,
     extension_data: Bytes32, // Used for future updates. Can be any 32 byte value initially
-});
+}
 
-streamable_struct! (Foliage {
+#[streamable]
+pub struct Foliage {
     // The entire foliage block, containing signature and the unsigned back pointer
     // The hash of this is the "header hash". Note that for unfinished blocks, the prev_block_hash
     // Is the prev from the signage point, and can be replaced with a more recent block
     prev_block_hash: Bytes32,
     reward_block_hash: Bytes32,
     foliage_block_data: FoliageBlockData,
     foliage_block_data_signature: G2Element,
     foliage_transaction_block_hash: Option<Bytes32>,
     foliage_transaction_block_signature: Option<G2Element>,
-});
+}
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/fullblock.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/fullblock.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
-use crate::streamable_struct;
 use crate::Bytes32;
 use crate::Coin;
 use crate::EndOfSubSlotBundle;
 use crate::Program;
 use crate::RewardChainBlock;
 use crate::VDFProof;
 use crate::{Foliage, FoliageTransactionBlock, TransactionsInfo};
 use chik_traits::Streamable;
 
-streamable_struct! (FullBlock {
+#[streamable]
+pub struct FullBlock {
     finished_sub_slots: Vec<EndOfSubSlotBundle>,
     reward_chain_block: RewardChainBlock,
     challenge_chain_sp_proof: Option<VDFProof>, // # If not first sp in sub-slot
     challenge_chain_ip_proof: VDFProof,
     reward_chain_sp_proof: Option<VDFProof>, // # If not first sp in sub-slot
     reward_chain_ip_proof: VDFProof,
     infused_challenge_chain_ip_proof: Option<VDFProof>, // # Iff deficit < 4
     foliage: Foliage,                                   // # Reward chain foliage data
     foliage_transaction_block: Option<FoliageTransactionBlock>, // # Reward chain foliage data (tx block)
     transactions_info: Option<TransactionsInfo>, // Reward chain foliage data (tx block additional)
     transactions_generator: Option<Program>,     // Program that generates transactions
     transactions_generator_ref_list: Vec<u32>, // List of block heights of previous generators referenced in this block
-});
+}
 
 impl FullBlock {
     pub fn prev_header_hash(&self) -> Bytes32 {
         self.foliage.prev_block_hash
     }
 
     pub fn header_hash(&self) -> Bytes32 {
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/header_block.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/header_block.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
-use crate::streamable_struct;
 use crate::Bytes;
 use crate::Bytes32;
 use crate::EndOfSubSlotBundle;
 use crate::RewardChainBlock;
 use crate::VDFProof;
 use crate::{Foliage, FoliageTransactionBlock, TransactionsInfo};
 use chik_traits::Streamable;
 
-streamable_struct! (HeaderBlock {
+#[streamable]
+pub struct HeaderBlock {
     // If first sb
     finished_sub_slots: Vec<EndOfSubSlotBundle>,
     // Reward chain trunk data
     reward_chain_block: RewardChainBlock,
     // If not first sp in sub-slot
     challenge_chain_sp_proof: Option<VDFProof>,
     challenge_chain_ip_proof: VDFProof,
@@ -26,15 +26,15 @@
     foliage: Foliage,
     // Reward chain foliage data (tx block)
     foliage_transaction_block: Option<FoliageTransactionBlock>,
     // Filter for block transactions
     transactions_filter: Bytes,
     // Reward chain foliage data (tx block additional)
     transactions_info: Option<TransactionsInfo>,
-});
+}
 
 impl HeaderBlock {
     pub fn prev_header_hash(&self) -> Bytes32 {
         self.foliage.prev_block_hash
     }
 
     pub fn prev_hash(&self) -> Bytes32 {
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/lazy_node.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/lazy_node.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             _ => Ok(None),
         }
     }
 
     #[getter(atom)]
     pub fn atom(&self, py: Python) -> Option<PyObject> {
         match &self.allocator.sexp(self.node) {
-            SExp::Atom => Some(PyBytes::new(py, self.allocator.atom(self.node)).into()),
+            SExp::Atom => Some(PyBytes::new(py, self.allocator.atom(self.node).as_ref()).into()),
             _ => None,
         }
     }
 }
 
 impl LazyNode {
     pub const fn new(a: Rc<Allocator>, n: NodePtr) -> Self {
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/lib.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 pub mod coin_state;
 pub mod end_of_sub_slot_bundle;
 pub mod fee_estimate;
 pub mod foliage;
 pub mod full_node_protocol;
 pub mod fullblock;
 pub mod header_block;
-pub mod message_struct;
 pub mod peer_info;
 pub mod pool_target;
 pub mod program;
 pub mod proof_of_space;
 pub mod reward_chain_block;
 pub mod slots;
 pub mod spend_bundle;
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/program.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/program.rs`

 * *Files 2% similar despite different names*

```diff
@@ -292,24 +292,17 @@
     } else {
         klvm_convert(a, o)
     }
 }
 
 #[cfg(feature = "py-bindings")]
 fn to_program(py: Python<'_>, node: LazyNode) -> PyResult<&PyAny> {
-    use pyo3::types::PyDict;
-    let ctx: &PyDict = PyDict::new(py);
-    ctx.set_item("node", node)?;
-    py.run(
-        "from chik.types.blockchain_format.program import Program\n\
-        ret = Program(node)\n",
-        None,
-        Some(ctx),
-    )?;
-    Ok(ctx.get_item("ret").unwrap())
+    let int_module = PyModule::import(py, "chik.types.blockchain_format.program")?;
+    let ty = int_module.getattr("Program")?;
+    ty.call1((node.into_py(py),))
 }
 
 #[cfg(feature = "py-bindings")]
 #[pymethods]
 impl Program {
     #[pyo3(name = "default")]
     #[staticmethod]
@@ -323,16 +316,15 @@
         let mut a = Allocator::new_limited(500000000);
         let klvm = klvm_convert(&mut a, args)?;
         Program::from_node_ptr(&a, klvm)
             .map_err(|error| PyErr::new::<PyTypeError, _>(error.to_string()))
     }
 
     fn get_tree_hash(&self) -> crate::Bytes32 {
-        let mut cursor = Cursor::new(self.0.as_ref());
-        klvmr::serde::tree_hash_from_stream(&mut cursor)
+        klvm_utils::tree_hash_from_bytes(self.0.as_ref())
             .unwrap()
             .into()
     }
 
     #[staticmethod]
     fn from_program(py: Python<'_>, p: PyObject) -> PyResult<Self> {
         let buf = p.getattr(py, "__bytes__")?.call0(py)?;
@@ -398,15 +390,18 @@
             Ok(py.allow_threads(|| run_program(&mut a, &dialect, program, klvm_args, max_cost)))
         })()?;
         match r {
             Ok(reduction) => {
                 let val = LazyNode::new(Rc::new(a), reduction.1);
                 Ok((reduction.0, to_program(py, val)?))
             }
-            Err(eval_err) => Err(PyValueError::new_err(eval_err.to_string())),
+            Err(eval_err) => {
+                let blob = node_to_bytes(&a, eval_err.0).ok().map(hex::encode);
+                Err(PyValueError::new_err((eval_err.1, blob)))
+            }
         }
     }
 
     fn to_program<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
         use std::rc::Rc;
         let mut a = Allocator::new_limited(500000000);
         let prg = node_from_bytes_backrefs(&mut a, self.0.as_ref())?;
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/reward_chain_block.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/reward_chain_block.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-use crate::streamable_struct;
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
 use crate::Bytes32;
 use crate::ProofOfSpace;
 use crate::VDFInfo;
 use chik_bls::G2Element;
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
-streamable_struct! (RewardChainBlockUnfinished {
+#[streamable]
+pub struct RewardChainBlockUnfinished {
     total_iters: u128,
     signage_point_index: u8,
     pos_ss_cc_challenge_hash: Bytes32,
     proof_of_space: ProofOfSpace,
     challenge_chain_sp_vdf: Option<VDFInfo>, // Not present for first sp in slot
     challenge_chain_sp_signature: G2Element,
     reward_chain_sp_vdf: Option<VDFInfo>, // Not present for first sp in slot
     reward_chain_sp_signature: G2Element,
-});
+}
 
-streamable_struct! (RewardChainBlock {
+#[streamable]
+pub struct RewardChainBlock {
     weight: u128,
     height: u32,
     total_iters: u128,
     signage_point_index: u8,
     pos_ss_cc_challenge_hash: Bytes32,
     proof_of_space: ProofOfSpace,
     challenge_chain_sp_vdf: Option<VDFInfo>, // Not present for first sp in slot
     challenge_chain_sp_signature: G2Element,
     challenge_chain_ip_vdf: VDFInfo,
     reward_chain_sp_vdf: Option<VDFInfo>, // Not present for first sp in slot
     reward_chain_sp_signature: G2Element,
     reward_chain_ip_vdf: VDFInfo,
     infused_challenge_chain_ip_vdf: Option<VDFInfo>, // Iff deficit < 16
     is_transaction_block: bool,
-});
+}
 
 #[cfg_attr(feature = "py-bindings", pymethods)]
 impl RewardChainBlock {
     pub fn get_unfinished(&self) -> RewardChainBlockUnfinished {
         RewardChainBlockUnfinished {
             total_iters: self.total_iters,
             signage_point_index: self.signage_point_index,
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/slots.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/slots.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-use crate::streamable_struct;
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
 use crate::Bytes32;
 use crate::ProofOfSpace;
 use crate::VDFInfo;
 use crate::VDFProof;
 use chik_bls::G2Element;
 
 // The hash of this is used as the challenge_hash for the ICC VDF
-streamable_struct! (ChallengeBlockInfo {
+#[streamable]
+pub struct ChallengeBlockInfo {
     proof_of_space: ProofOfSpace,
     challenge_chain_sp_vdf: Option<VDFInfo>, // Only present if not the first sp
     challenge_chain_sp_signature: G2Element,
     challenge_chain_ip_vdf: VDFInfo,
-});
+}
 
-streamable_struct! (ChallengeChainSubSlot {
+#[streamable]
+pub struct ChallengeChainSubSlot {
     challenge_chain_end_of_slot_vdf: VDFInfo,
     infused_challenge_chain_sub_slot_hash: Option<Bytes32>, // Only at the end of a slot
     subepoch_summary_hash: Option<Bytes32>, // Only once per sub-epoch, and one sub-epoch delayed
     new_sub_slot_iters: Option<u64>,        // Only at the end of epoch, sub-epoch, and slot
     new_difficulty: Option<u64>,            // Only at the end of epoch, sub-epoch, and slot
-});
+}
 
-streamable_struct!(InfusedChallengeChainSubSlot {
+#[streamable]
+pub struct InfusedChallengeChainSubSlot {
     infused_challenge_chain_end_of_slot_vdf: VDFInfo,
-});
+}
 
-streamable_struct! (RewardChainSubSlot {
+#[streamable]
+pub struct RewardChainSubSlot {
     end_of_slot_vdf: VDFInfo,
     challenge_chain_sub_slot_hash: Bytes32,
     infused_challenge_chain_sub_slot_hash: Option<Bytes32>,
     deficit: u8, // 16 or less. usually zero
-});
+}
 
-streamable_struct! (SubSlotProofs {
+#[streamable]
+pub struct SubSlotProofs {
     challenge_chain_slot_proof: VDFProof,
     infused_challenge_chain_slot_proof: Option<VDFProof>,
     reward_chain_slot_proof: VDFProof,
-});
+}
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/spend_bundle.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/spend_bundle.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 use crate::coin_spend::CoinSpend;
-use crate::streamable_struct;
 use crate::Bytes32;
 use crate::Coin;
 use chik_bls::G2Element;
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 use chik_traits::Streamable;
 use klvm_traits::FromKlvm;
 use klvmr::allocator::{NodePtr, SExp};
 use klvmr::cost::Cost;
 use klvmr::op_utils::{first, rest};
 use klvmr::reduction::EvalErr;
 use klvmr::Allocator;
-use std::result::Result;
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
-streamable_struct! (SpendBundle {
+#[streamable]
+pub struct SpendBundle {
     coin_spends: Vec<CoinSpend>,
     aggregated_signature: G2Element,
-});
+}
 
 impl SpendBundle {
     pub fn aggregate(spend_bundles: &[SpendBundle]) -> SpendBundle {
         let mut coin_spends = Vec::<CoinSpend>::new();
         let mut aggregated_signature = G2Element::default();
         for sb in spend_bundles {
             coin_spends.extend_from_slice(&sb.coin_spends[..]);
@@ -54,26 +53,27 @@
             let (cost, mut conds) =
                 cs.puzzle_reveal
                     .run(&mut a, ENABLE_FIXED_DIV, cost_left, &cs.solution)?;
             if cost > cost_left {
                 return Err(EvalErr(a.nil(), "cost exceeded".to_string()));
             }
             cost_left -= cost;
-            let parent_coin_info: Bytes32 = cs.coin.coin_id().into();
+            let parent_coin_info: Bytes32 = cs.coin.coin_id();
 
             while let Some((c, tail)) = a.next(conds) {
                 conds = tail;
                 let op = first(&a, c)?;
                 let c = rest(&a, c)?;
                 let buf = match a.sexp(op) {
                     SExp::Atom => a.atom(op),
                     _ => {
                         return Err(EvalErr(op, "invalid condition".to_string()));
                     }
                 };
+                let buf = buf.as_ref();
                 if buf.len() != 1 {
                     continue;
                 }
                 if buf[0] == CREATE_COIN {
                     let (puzzle_hash, (amount, _)) = <(Bytes32, (u64, NodePtr))>::from_klvm(&a, c)
                         .map_err(|_| EvalErr(c, "failed to parse spend".to_string()))?;
                     ret.push(Coin {
@@ -152,15 +152,16 @@
         "bb13d1e13438736c7ba0217c7b82ee4db56a7f4fb9d22c703c2152362b2314ee"
     )]
     fn test_additions_ff(
         #[case] spend_file: &str,
         #[case] expect_parent: &str,
         #[case] expect_ph: &str,
     ) {
-        let spend_bytes = fs::read(format!("../ff-tests/{spend_file}.spend")).expect("read file");
+        let spend_bytes =
+            fs::read(format!("../../ff-tests/{spend_file}.spend")).expect("read file");
         let spend = CoinSpend::from_bytes(&spend_bytes).expect("parse CoinSpend");
         let bundle = SpendBundle::new(vec![spend], G2Element::default());
 
         let additions = bundle.additions().expect("additions");
 
         assert_eq!(additions.len(), 1);
         assert_eq!(
@@ -210,15 +211,15 @@
 ff01\
 80\
 80";
         test_impl(solution, |test_coin: Coin, bundle: SpendBundle| {
             let additions = bundle.additions().expect("additions");
 
             let new_coin = Coin::new(
-                test_coin.coin_id().into(),
+                test_coin.coin_id(),
                 hex::decode("2222222222222222222222222222222222222222222222222222222222222222")
                     .unwrap()
                     .try_into()
                     .unwrap(),
                 1,
             );
             assert_eq!(additions, [new_coin]);
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/unfinished_block.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/unfinished_block.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
-use crate::streamable_struct;
 use crate::Bytes32;
 use crate::EndOfSubSlotBundle;
 use crate::Program;
 use crate::RewardChainBlockUnfinished;
 use crate::VDFProof;
 use crate::{Foliage, FoliageTransactionBlock, TransactionsInfo};
 use chik_traits::Streamable;
 
-streamable_struct! (UnfinishedBlock {
+#[streamable]
+pub struct UnfinishedBlock {
     // Full block, without the final VDFs
-    finished_sub_slots: Vec<EndOfSubSlotBundle>,  // If first sb
-    reward_chain_block: RewardChainBlockUnfinished,  // Reward chain trunk data
+    finished_sub_slots: Vec<EndOfSubSlotBundle>, // If first sb
+    reward_chain_block: RewardChainBlockUnfinished, // Reward chain trunk data
     challenge_chain_sp_proof: Option<VDFProof>,  // If not first sp in sub-slot
-    reward_chain_sp_proof: Option<VDFProof>,  // If not first sp in sub-slot
-    foliage: Foliage,  // Reward chain foliage data
-    foliage_transaction_block: Option<FoliageTransactionBlock>,  // Reward chain foliage data (tx block)
-    transactions_info: Option<TransactionsInfo>,  // Reward chain foliage data (tx block additional)
-    transactions_generator: Option<Program>,  // Program that generates transactions
-    transactions_generator_ref_list: Vec<u32>,  // List of block heights of previous generators referenced in this block
-});
+    reward_chain_sp_proof: Option<VDFProof>,     // If not first sp in sub-slot
+    foliage: Foliage,                            // Reward chain foliage data
+    foliage_transaction_block: Option<FoliageTransactionBlock>, // Reward chain foliage data (tx block)
+    transactions_info: Option<TransactionsInfo>, // Reward chain foliage data (tx block additional)
+    transactions_generator: Option<Program>,     // Program that generates transactions
+    transactions_generator_ref_list: Vec<u32>, // List of block heights of previous generators referenced in this block
+}
 
 impl UnfinishedBlock {
     pub fn prev_header_hash(&self) -> Bytes32 {
         self.foliage.prev_block_hash
     }
 
     pub fn partial_hash(&self) -> Bytes32 {
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/wallet_protocol.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/wallet_protocol.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,180 +1,216 @@
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
-use crate::message_struct;
-use crate::streamable_struct;
-use crate::ChikProtocolMessage;
 use crate::Coin;
 use crate::CoinState;
 use crate::FeeEstimateGroup;
 use crate::HeaderBlock;
 use crate::Program;
 use crate::SpendBundle;
 use crate::{Bytes, Bytes32};
 
-message_struct!(RequestPuzzleSolution {
+#[streamable(message)]
+pub struct RequestPuzzleSolution {
     coin_name: Bytes32,
     height: u32,
-});
+}
 
-streamable_struct!(PuzzleSolutionResponse {
+#[streamable]
+pub struct PuzzleSolutionResponse {
     coin_name: Bytes32,
     height: u32,
     puzzle: Program,
     solution: Program,
-});
+}
 
-message_struct!(RespondPuzzleSolution {
+#[streamable(message)]
+pub struct RespondPuzzleSolution {
     response: PuzzleSolutionResponse,
-});
+}
 
-message_struct!(RejectPuzzleSolution {
+#[streamable(message)]
+pub struct RejectPuzzleSolution {
     coin_name: Bytes32,
     height: u32,
-});
+}
 
-message_struct!(SendTransaction {
+#[streamable(message)]
+pub struct SendTransaction {
     transaction: SpendBundle,
-});
+}
 
-message_struct! (TransactionAck {
+#[streamable(message)]
+pub struct TransactionAck {
     txid: Bytes32,
     status: u8, // MempoolInclusionStatus
     error: Option<String>,
-});
+}
 
-message_struct!(NewPeakWallet {
+#[streamable(message)]
+pub struct NewPeakWallet {
     header_hash: Bytes32,
     height: u32,
     weight: u128,
     fork_point_with_previous_peak: u32,
-});
+}
 
-message_struct!(RequestBlockHeader { height: u32 });
+#[streamable(message)]
+pub struct RequestBlockHeader {
+    height: u32,
+}
 
-message_struct!(RespondBlockHeader {
+#[streamable(message)]
+pub struct RespondBlockHeader {
     header_block: HeaderBlock,
-});
+}
 
-message_struct!(RejectHeaderRequest { height: u32 });
+#[streamable(message)]
+pub struct RejectHeaderRequest {
+    height: u32,
+}
 
-message_struct! (RequestRemovals {
+#[streamable(message)]
+pub struct RequestRemovals {
     height: u32,
     header_hash: Bytes32,
     coin_names: Option<Vec<Bytes32>>,
-});
+}
 
-message_struct! (RespondRemovals {
+#[streamable(message)]
+pub struct RespondRemovals {
     height: u32,
     header_hash: Bytes32,
     coins: Vec<(Bytes32, Option<Coin>)>,
     proofs: Option<Vec<(Bytes32, Bytes)>>,
-});
+}
 
-message_struct!(RejectRemovalsRequest {
+#[streamable(message)]
+pub struct RejectRemovalsRequest {
     height: u32,
     header_hash: Bytes32,
-});
+}
 
-message_struct! (RequestAdditions {
+#[streamable(message)]
+pub struct RequestAdditions {
     height: u32,
     header_hash: Option<Bytes32>,
     puzzle_hashes: Option<Vec<Bytes32>>,
-});
+}
 
-message_struct! (RespondAdditions {
+#[streamable(message)]
+pub struct RespondAdditions {
     height: u32,
     header_hash: Bytes32,
     coins: Vec<(Bytes32, Vec<Coin>)>,
     proofs: Option<Vec<(Bytes32, Bytes, Option<Bytes>)>>,
-});
+}
 
-message_struct!(RejectAdditionsRequest {
+#[streamable(message)]
+pub struct RejectAdditionsRequest {
     height: u32,
     header_hash: Bytes32,
-});
+}
 
-message_struct! (RespondBlockHeaders {
+#[streamable(message)]
+pub struct RespondBlockHeaders {
     start_height: u32,
     end_height: u32,
     header_blocks: Vec<HeaderBlock>,
-});
+}
 
-message_struct!(RejectBlockHeaders {
+#[streamable(message)]
+pub struct RejectBlockHeaders {
     start_height: u32,
     end_height: u32,
-});
+}
 
-message_struct!(RequestBlockHeaders {
+#[streamable(message)]
+pub struct RequestBlockHeaders {
     start_height: u32,
     end_height: u32,
     return_filter: bool,
-});
+}
 
-message_struct!(RequestHeaderBlocks {
+#[streamable(message)]
+pub struct RequestHeaderBlocks {
     start_height: u32,
     end_height: u32,
-});
+}
 
-message_struct!(RejectHeaderBlocks {
+#[streamable(message)]
+pub struct RejectHeaderBlocks {
     start_height: u32,
     end_height: u32,
-});
+}
 
-message_struct! (RespondHeaderBlocks {
+#[streamable(message)]
+pub struct RespondHeaderBlocks {
     start_height: u32,
     end_height: u32,
     header_blocks: Vec<HeaderBlock>,
-});
+}
 
-message_struct! (RegisterForPhUpdates {
+#[streamable(message)]
+pub struct RegisterForPhUpdates {
     puzzle_hashes: Vec<Bytes32>,
     min_height: u32,
-});
+}
 
-message_struct! (RespondToPhUpdates {
+#[streamable(message)]
+pub struct RespondToPhUpdates {
     puzzle_hashes: Vec<Bytes32>,
     min_height: u32,
     coin_states: Vec<CoinState>,
-});
+}
 
-message_struct! (RegisterForCoinUpdates {
+#[streamable(message)]
+pub struct RegisterForCoinUpdates {
     coin_ids: Vec<Bytes32>,
     min_height: u32,
-});
+}
 
-message_struct! (RespondToCoinUpdates {
+#[streamable(message)]
+pub struct RespondToCoinUpdates {
     coin_ids: Vec<Bytes32>,
     min_height: u32,
     coin_states: Vec<CoinState>,
-});
+}
 
-message_struct! (CoinStateUpdate {
+#[streamable(message)]
+pub struct CoinStateUpdate {
     height: u32,
     fork_height: u32,
     peak_hash: Bytes32,
     items: Vec<CoinState>,
-});
+}
 
-message_struct!(RequestChildren { coin_name: Bytes32 });
+#[streamable(message)]
+pub struct RequestChildren {
+    coin_name: Bytes32,
+}
 
-message_struct! (RespondChildren {
+#[streamable(message)]
+pub struct RespondChildren {
     coin_states: Vec<CoinState>,
-});
+}
 
-message_struct!(RequestSesInfo {
+#[streamable(message)]
+pub struct RequestSesInfo {
     start_height: u32,
     end_height: u32,
-});
+}
 
-message_struct! (RespondSesInfo {
+#[streamable(message)]
+pub struct RespondSesInfo {
     reward_chain_hash: Vec<Bytes32>,
     heights: Vec<Vec<u32>>,
-});
+}
 
-message_struct! (RequestFeeEstimates {
+#[streamable(message)]
+pub struct RequestFeeEstimates {
     time_targets: Vec<u64>,
-});
+}
 
-message_struct!(RespondFeeEstimates {
+#[streamable(message)]
+pub struct RespondFeeEstimates {
     estimates: FeeEstimateGroup,
-});
+}
```

### Comparing `chik_rs-0.5.2/chik-protocol/src/weight_proof.rs` & `chik_rs-0.6.0/crates/chik-protocol/src/weight_proof.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-use crate::streamable_struct;
-use chik_streamable_macro::Streamable;
+use chik_streamable_macro::streamable;
 
 use crate::Bytes32;
 use crate::EndOfSubSlotBundle;
 use crate::HeaderBlock;
 use crate::ProofOfSpace;
 use crate::RewardChainBlock;
 use crate::{VDFInfo, VDFProof};
 
-streamable_struct! (SubEpochData {
+#[streamable]
+pub struct SubEpochData {
     reward_chain_hash: Bytes32,
     num_blocks_overflow: u8,
     new_sub_slot_iters: Option<u64>,
     new_difficulty: Option<u64>,
-});
+}
 
 // number of challenge blocks
 // Average iters for challenge blocks
 // |--A-R----R-------R--------R------R----R----------R-----R--R---|       Honest difficulty 1000
 //           0.16
 
 //  compute total reward chain blocks
 // |----------------------------A---------------------------------|       Attackers chain 1000
 //                            0.48
 // total number of challenge blocks == total number of reward chain blocks
 
-streamable_struct! (SubSlotData {
+#[streamable]
+pub struct SubSlotData {
     proof_of_space: Option<ProofOfSpace>,
     cc_signage_point: Option<VDFProof>,
     cc_infusion_point: Option<VDFProof>,
     icc_infusion_point: Option<VDFProof>,
     cc_sp_vdf_info: Option<VDFInfo>,
     signage_point_index: Option<u8>,
     cc_slot_end: Option<VDFProof>,
     icc_slot_end: Option<VDFProof>,
     cc_slot_end_info: Option<VDFInfo>,
     icc_slot_end_info: Option<VDFInfo>,
     cc_ip_vdf_info: Option<VDFInfo>,
     icc_ip_vdf_info: Option<VDFInfo>,
     total_iters: Option<u128>,
-});
+}
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
 #[cfg_attr(feature = "py-bindings", pymethods)]
 impl SubSlotData {
     pub fn is_end_of_slot(&self) -> bool {
@@ -51,32 +52,37 @@
     }
 
     pub fn is_challenge(&self) -> bool {
         self.proof_of_space.is_some()
     }
 }
 
-streamable_struct! (SubEpochChallengeSegment {
+#[streamable]
+pub struct SubEpochChallengeSegment {
     sub_epoch_n: u32,
     sub_slots: Vec<SubSlotData>,
     rc_slot_end_info: Option<VDFInfo>,
-});
+}
 
-streamable_struct! (SubEpochSegments {
+#[streamable]
+pub struct SubEpochSegments {
     challenge_segments: Vec<SubEpochChallengeSegment>,
-});
+}
 
 // this is used only for serialization to database
-streamable_struct! (RecentChainData {
+#[streamable]
+pub struct RecentChainData {
     recent_chain_data: Vec<HeaderBlock>,
-});
+}
 
-streamable_struct! (ProofBlockHeader {
+#[streamable]
+pub struct ProofBlockHeader {
     finished_sub_slots: Vec<EndOfSubSlotBundle>,
     reward_chain_block: RewardChainBlock,
-});
+}
 
-streamable_struct! (WeightProof {
+#[streamable]
+pub struct WeightProof {
     sub_epochs: Vec<SubEpochData>,
-    sub_epoch_segments: Vec<SubEpochChallengeSegment>,  // sampled sub epoch
+    sub_epoch_segments: Vec<SubEpochChallengeSegment>, // sampled sub epoch
     recent_chain_data: Vec<HeaderBlock>,
-});
+}
```

### Comparing `chik_rs-0.5.2/chik-traits/Cargo.toml` & `chik_rs-0.6.0/crates/chik-traits/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "chik-traits"
-version = "0.5.2"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik traits for Streamable types (chik's serialization format)"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["multiple-pymethods"], optional = true }
-chik_py_streamable_macro = { version = "0.5.1", path = "../chik_py_streamable_macro", optional = true }
-chik_streamable_macro = { version = "0.3.0", path = "../chik_streamable_macro" }
+chik_py_streamable_macro = { version = "0.6.0", path = "../chik_py_streamable_macro", optional = true }
+chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
 sha2 = "0.10.8"
 hex = "0.4.3"
 thiserror = "1.0.44"
```

### Comparing `chik_rs-0.5.2/chik-traits/src/chik_error.rs` & `chik_rs-0.6.0/crates/chik-traits/src/chik_error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-traits/src/from_json_dict.rs` & `chik_rs-0.6.0/crates/chik-traits/src/from_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-traits/src/int.rs` & `chik_rs-0.6.0/crates/chik-traits/src/int.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-use pyo3::prelude::*;
-use pyo3::types::{PyAny, PyBool, PyList, PyString, PyTuple};
-use pyo3::PyResult;
+use pyo3::types::{PyAny, PyBool, PyList, PyModule, PyString, PyTuple};
+use pyo3::{IntoPy, PyResult, Python};
 
 /// A custom to-python conversion trait that turns primitive integer types into
 /// the chik-blockchain fixed-width integer types (uint8, int8, etc.)
 pub trait ChikToPython {
     fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::types::PyAny>;
 }
```

### Comparing `chik_rs-0.5.2/chik-traits/src/streamable.rs` & `chik_rs-0.6.0/crates/chik-traits/src/streamable.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use crate::chik_error::{Error, Result};
 use sha2::{Digest, Sha256};
-use std::convert::TryInto;
 use std::io::Cursor;
 use std::mem::size_of;
 
 pub fn read_bytes<'a>(input: &'a mut Cursor<&[u8]>, len: usize) -> Result<&'a [u8]> {
     let pos = input.position();
     let buf: &'a [u8] = &input.get_ref()[pos as usize..];
     if buf.len() < len {
```

### Comparing `chik_rs-0.5.2/chik-traits/src/to_json_dict.rs` & `chik_rs-0.6.0/crates/chik-traits/src/to_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-wallet/Cargo.toml` & `chik_rs-0.6.0/crates/chik-wallet/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [package]
 name = "chik-wallet"
-version = "0.5.1"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik primitives needed for building wallets."
 authors = ["Brandon Haggstrom <b.haggstrom@chiknetwork.com>"]
-homepage = "https://github.com/Chik-Network/chik_rs/chik-wallet/"
-repository = "https://github.com/Chik-Network/chik_rs/chik-wallet/"
+homepage = "https://github.com/Chik-Network/chik_rs"
+repository = "https://github.com/Chik-Network/chik_rs"
 
 [dependencies]
-klvmr = "0.5.0"
+klvmr = "0.6.1"
 sha2 = "0.10.8"
 num-bigint = "0.4.3"
 hex-literal = "0.4.1"
-klvm-utils = { version = "0.5.1", path = "../klvm-utils" }
-klvm-traits = { version = "0.5.1", path = "../klvm-traits", features = ["chik-bls"] }
-chik-bls = { version = "0.5.1", path = "../chik-bls" }
-chik-protocol = { version = "0.5.1", path = "../chik-protocol" }
+klvm-utils = { version = "0.6.0", path = "../klvm-utils" }
+klvm-traits = { version = "0.6.0", path = "../klvm-traits", features = ["chik-bls"] }
+chik-bls = { version = "0.6.0", path = "../chik-bls" }
+chik-protocol = { version = "0.6.0", path = "../chik-protocol" }
 arbitrary = "1.3.0"
 
 [dev-dependencies]
 hex = "0.4.3"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chik_rs-0.5.2/chik-wallet/src/derive_synthetic.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/derive_synthetic.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-wallet/src/proof.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/proof.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-wallet/src/puzzles/cat.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/puzzles/cat.rs`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     curry_tree_hash(
         CAT_PUZZLE_HASH,
         &[mod_hash, asset_id_hash, inner_puzzle_hash],
     )
 }
 
 /// This is the puzzle reveal of the [CAT2 standard](https://chiklisp.com/cats) puzzle.
-pub static CAT_PUZZLE: [u8; 1672] = hex!(
+pub const CAT_PUZZLE: [u8; 1672] = hex!(
     "
     ff02ffff01ff02ff5effff04ff02ffff04ffff04ff05ffff04ffff0bff34ff05
     80ffff04ff0bff80808080ffff04ffff02ff17ff2f80ffff04ff5fffff04ffff
     02ff2effff04ff02ffff04ff17ff80808080ffff04ffff02ff2affff04ff02ff
     ff04ff82027fffff04ff82057fffff04ff820b7fff808080808080ffff04ff81
     bfffff04ff82017fffff04ff8202ffffff04ff8205ffffff04ff820bffff8080
     8080808080808080808080ffff04ffff01ffffffff3d46ff02ff333cffff0401
@@ -105,35 +105,35 @@
     2effff04ff02ffff04ffff04ff15ffff04ffff10ff82017fffff11ff8202dfff
     2b80ff8202ff80ff808080ff8080808080ff808080ff138080ff808080808080
     80808080ff018080
     "
 );
 
 /// This is the puzzle hash of the [CAT2 standard](https://chiklisp.com/cats) puzzle.
-pub static CAT_PUZZLE_HASH: [u8; 32] = hex!(
+pub const CAT_PUZZLE_HASH: [u8; 32] = hex!(
     "
     37bef360ee858133b69d595a906dc45d01af50379dad515eb9518abb7c1d2a7a
     "
 );
 
 /// This is the puzzle reveal of the [CAT2 multi-issuance TAIL](https://chiklisp.com/cats#multi) puzzle.
-pub static EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE: [u8; 41] = hex!(
+pub const EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE: [u8; 41] = hex!(
     "
     ff02ffff01ff04ffff04ff02ffff04ff05ffff04ff5fff80808080ff8080ffff
     04ffff0132ff018080
     "
 );
 
 /// This is the puzzle reveal of the old [CAT1 standard](https://chiklisp.com/cats) puzzle.
 ///
 /// **Warning:**
 /// It is recommended not to use CAT1 for anything other than backwards compatibility (e.g. offer compression),
 /// due to security issues uncovered in an audit. You can read more about the vulnerability that prompted the creation
 /// of CAT2 in the [CATbleed Post Mortem](https://github.com/Chik-Network/post-mortem/blob/main/2022-08/2022-08-19-CATbleed.md).
-pub static CAT_PUZZLE_V1: [u8; 1420] = hex!(
+pub const CAT_PUZZLE_V1: [u8; 1420] = hex!(
     "
     ff02ffff01ff02ff5effff04ff02ffff04ffff04ff05ffff04ffff0bff2cff05
     80ffff04ff0bff80808080ffff04ffff02ff17ff2f80ffff04ff5fffff04ffff
     02ff2effff04ff02ffff04ff17ff80808080ffff04ffff0bff82027fff82057f
     ff820b7f80ffff04ff81bfffff04ff82017fffff04ff8202ffffff04ff8205ff
     ffff04ff820bffff80808080808080808080808080ffff04ffff01ffffffff81
     ca3dff46ff0233ffff3c04ff01ff0181cbffffff02ff02ffff03ff05ffff01ff
@@ -181,15 +181,15 @@
 
 /// This is the puzzle hash of the old [CAT1 standard](https://chiklisp.com/cats) puzzle.
 ///
 /// **Warning:**
 /// It is recommended not to use CAT1 for anything other than backwards compatibility (e.g. offer compression),
 /// due to security issues uncovered in an audit. You can read more about the vulnerability that prompted the creation
 /// of CAT2 in the [CATbleed Post Mortem](https://github.com/Chik-Network/post-mortem/blob/main/2022-08/2022-08-19-CATbleed.md).
-pub static CAT_PUZZLE_HASH_V1: [u8; 32] = hex!(
+pub const CAT_PUZZLE_HASH_V1: [u8; 32] = hex!(
     "
     72dec062874cd4d3aab892a0906688a1ae412b0109982e1797a170add88bdcdc
     "
 );
 
 #[cfg(test)]
 mod tests {
```

### Comparing `chik_rs-0.5.2/chik-wallet/src/puzzles/did.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/puzzles/did.rs`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         match self {
             Self::InnerSpend(solution) => klvm_list!(1, solution).to_klvm(encoder),
         }
     }
 }
 
 /// This is the puzzle reveal of the [DID1 standard](https://chiklisp.com/dids) puzzle.
-pub static DID_INNER_PUZZLE: [u8; 1012] = hex!(
+pub const DID_INNER_PUZZLE: [u8; 1012] = hex!(
     "
     ff02ffff01ff02ffff03ff81bfffff01ff02ff05ff82017f80ffff01ff02ffff
     03ffff22ffff09ffff02ff7effff04ff02ffff04ff8217ffff80808080ff0b80
     ffff15ff17ff808080ffff01ff04ffff04ff28ffff04ff82017fff808080ffff
     04ffff04ff34ffff04ff8202ffffff04ff82017fffff04ffff04ff8202ffff80
     80ff8080808080ffff04ffff04ff38ffff04ff822fffff808080ffff02ff26ff
     ff04ff02ffff04ff2fffff04ff17ffff04ff8217ffffff04ff822fffffff04ff
@@ -86,15 +86,15 @@
     808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff7effff04ff
     02ffff04ff09ff80808080ffff02ff7effff04ff02ffff04ff0dff8080808080
     ffff01ff0bffff0101ff058080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [DID1 standard](https://chiklisp.com/dids) puzzle.
-pub static DID_INNER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const DID_INNER_PUZZLE_HASH: [u8; 32] = hex!(
     "
     33143d2bef64f14036742673afd158126b94284b4530a28c354fac202b0c910e
     "
 );
 
 #[cfg(test)]
 mod tests {
```

### Comparing `chik_rs-0.5.2/chik-wallet/src/puzzles/nft.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/puzzles/nft.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-wallet/src/puzzles/offer.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/puzzles/offer.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-wallet/src/puzzles/singleton.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/puzzles/singleton.rs`

 * *Files 3% similar despite different names*

```diff
@@ -42,34 +42,34 @@
             launcher_id,
             launcher_puzzle_hash: SINGLETON_LAUNCHER_PUZZLE_HASH.into(),
         }
     }
 }
 
 /// This is the puzzle reveal of the [singleton launcher](https://chiklisp.com/singletons#launcher) puzzle.
-pub static SINGLETON_LAUNCHER_PUZZLE: [u8; 175] = hex!(
+pub const SINGLETON_LAUNCHER_PUZZLE: [u8; 175] = hex!(
     "
     ff02ffff01ff04ffff04ff04ffff04ff05ffff04ff0bff80808080ffff04ffff
     04ff0affff04ffff02ff0effff04ff02ffff04ffff04ff05ffff04ff0bffff04
     ff17ff80808080ff80808080ff808080ff808080ffff04ffff01ff33ff3cff02
     ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff0effff04ff02ffff04ff
     09ff80808080ffff02ff0effff04ff02ffff04ff0dff8080808080ffff01ff0b
     ffff0101ff058080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [singleton launcher](https://chiklisp.com/singletons#launcher) puzzle.
-pub static SINGLETON_LAUNCHER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const SINGLETON_LAUNCHER_PUZZLE_HASH: [u8; 32] = hex!(
     "
     eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9
     "
 );
 
 /// This is the puzzle reveal of the [singleton](https://chiklisp.com/singletons) puzzle.
-pub static SINGLETON_TOP_LAYER_PUZZLE: [u8; 967] = hex!(
+pub const SINGLETON_TOP_LAYER_PUZZLE: [u8; 967] = hex!(
     "
     ff02ffff01ff02ffff03ffff18ff2fff3480ffff01ff04ffff04ff20ffff04ff
     2fff808080ffff04ffff02ff3effff04ff02ffff04ff05ffff04ffff02ff2aff
     ff04ff02ffff04ff27ffff04ffff02ffff03ff77ffff01ff02ff36ffff04ff02
     ffff04ff09ffff04ff57ffff04ffff02ff2effff04ff02ffff04ff05ff808080
     80ff808080808080ffff011d80ff0180ffff04ffff02ffff03ff77ffff0181b7
     ffff015780ff0180ff808080808080ffff04ff77ff808080808080ffff02ff3a
@@ -98,15 +98,15 @@
     ff8080808080ffff01ff0bffff0101ff058080ff0180ff02ffff03ffff21ff17
     ffff09ff0bff158080ffff01ff04ff30ffff04ff0bff808080ffff01ff088080
     ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [singleton](https://chiklisp.com/singletons) puzzle.
-pub static SINGLETON_TOP_LAYER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const SINGLETON_TOP_LAYER_PUZZLE_HASH: [u8; 32] = hex!(
     "
     7faa3253bfddd1e0decb0906b2dc6247bbc4cf608f58345d173adb63e8b47c9f
     "
 );
 
 #[cfg(test)]
 mod tests {
```

### Comparing `chik_rs-0.5.2/chik-wallet/src/puzzles/standard.rs` & `chik_rs-0.6.0/crates/chik-wallet/src/puzzles/standard.rs`

 * *Files 11% similar despite different names*

```diff
@@ -19,39 +19,39 @@
 
 pub fn standard_puzzle_hash(synthetic_key: &PublicKey) -> [u8; 32] {
     let sk_tree_hash = tree_hash_atom(&synthetic_key.to_bytes());
     curry_tree_hash(STANDARD_PUZZLE_HASH, &[sk_tree_hash])
 }
 
 /// This is the puzzle reveal of the [standard transaction](https://chiklisp.com/standard-transactions) puzzle.
-pub static STANDARD_PUZZLE: [u8; 227] = hex!(
+pub const STANDARD_PUZZLE: [u8; 227] = hex!(
     "
     ff02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff1dff0bffff
     1effff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080808080ffff
     01ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff04ffff04ff
     05ffff04ffff02ff06ffff04ff02ffff04ff17ff80808080ff80808080ffff02
     ff17ff2f808080ff0180ffff04ffff01ff32ff02ffff03ffff07ff0580ffff01
     ff0bffff0102ffff02ff06ffff04ff02ffff04ff09ff80808080ffff02ff06ff
     ff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff
     018080
     "
 );
 
 /// This is the puzzle hash of the [standard transaction](https://chiklisp.com/standard-transactions) puzzle.
-pub static STANDARD_PUZZLE_HASH: [u8; 32] = hex!(
+pub const STANDARD_PUZZLE_HASH: [u8; 32] = hex!(
     "
     e9aaa49f45bad5c889b86ee3341550c155cfdd10c3a6757de618d20612fffd52
     "
 );
 
 /// This is the puzzle reveal of the [default hidden puzzle](https://chiklisp.com/standard-transactions#default-hidden-puzzle).
-pub static DEFAULT_HIDDEN_PUZZLE: [u8; 3] = hex!("ff0980");
+pub const DEFAULT_HIDDEN_PUZZLE: [u8; 3] = hex!("ff0980");
 
 /// This is the puzzle hash of the [default hidden puzzle](https://chiklisp.com/standard-transactions#default-hidden-puzzle).
-pub static DEFAULT_HIDDEN_PUZZLE_HASH: [u8; 32] = hex!(
+pub const DEFAULT_HIDDEN_PUZZLE_HASH: [u8; 32] = hex!(
     "
     711d6c4e32c92e53179b199484cf8c897542bc57f2b22582799f9d657eec4699
     "
 );
 
 #[cfg(test)]
 mod tests {
```

### Comparing `chik_rs-0.5.2/chik_streamable_macro/Cargo.toml` & `chik_rs-0.6.0/crates/chik_streamable_macro/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [package]
 name = "chik_streamable_macro"
-version = "0.3.0"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Streamable derive macro for serializing/deserializing types in Chik protocol format"
 authors = ["Arvid Norberg <arvid@libtorrent.org>"]
-homepage = "https://github.com/Chik-Network/chik_rs/"
-repository = "https://github.com/Chik-Network/chik_rs/"
+homepage = "https://github.com/Chik-Network/chik_rs"
+repository = "https://github.com/Chik-Network/chik_rs"
 
 [lib]
 proc-macro = true
 
 [dependencies]
 syn = { version = "2.0.27", features = ["full"] }
 quote = "1.0.32"
```

### Comparing `chik_rs-0.5.2/klvm-derive/src/from_klvm.rs` & `chik_rs-0.6.0/crates/klvm-derive/src/from_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-derive/src/helpers.rs` & `chik_rs-0.6.0/crates/klvm-derive/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-derive/src/lib.rs` & `chik_rs-0.6.0/crates/klvm-derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-derive/src/macros.rs` & `chik_rs-0.6.0/crates/klvm-derive/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-derive/src/to_klvm.rs` & `chik_rs-0.6.0/crates/klvm-derive/src/to_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-utils/src/curried_program.rs` & `chik_rs-0.6.0/crates/klvm-utils/src/curried_program.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-utils/src/curry_tree_hash.rs` & `chik_rs-0.6.0/crates/klvm-utils/src/curry_tree_hash.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-utils/src/lib.rs` & `chik_rs-0.6.0/crates/klvm-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/benches/run-generator.rs` & `chik_rs-0.6.0/crates/chik-consensus/benches/run-generator.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-use chik::gen::conditions::MempoolVisitor;
-use chik::gen::flags::ALLOW_BACKREFS;
-use chik::gen::run_block_generator::{run_block_generator, run_block_generator2};
+use chik_consensus::gen::conditions::MempoolVisitor;
+use chik_consensus::gen::flags::ALLOW_BACKREFS;
+use chik_consensus::gen::run_block_generator::{run_block_generator, run_block_generator2};
 use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use klvmr::serde::{node_from_bytes, node_to_bytes_backrefs};
 use klvmr::Allocator;
 use std::fs::read_to_string;
 use std::time::Instant;
 
 fn run(c: &mut Criterion) {
@@ -20,23 +20,23 @@
         "block-1ee588dc",
         "block-6fe59b24",
         "block-b45268ac",
         "block-c2a8df0d",
         "block-e5002df2",
         "recursion-pairs",
     ] {
-        let filename = format!("generator-tests/{name}.txt");
+        let filename = format!("../../generator-tests/{name}.txt");
         println!("file: {filename}");
         let test_file = read_to_string(filename).expect("test file not found");
         let generator = test_file.split_once('\n').expect("invalid test file").0;
         let generator = hex::decode(generator).expect("invalid hex encoded generator");
 
         let mut block_refs = Vec::<Vec<u8>>::new();
 
-        let filename = format!("generator-tests/{name}.env");
+        let filename = format!("../../generator-tests/{name}.env");
         if let Ok(env_hex) = std::fs::read_to_string(&filename) {
             println!("block-ref file: {filename}");
             block_refs.push(hex::decode(env_hex).expect("hex decode env-file"));
         }
 
         let compressed_generator = {
             let mut a = Allocator::new();
@@ -48,15 +48,15 @@
             group.bench_function(format!("run_block_generator {name}{name_suffix}"), |b| {
                 b.iter(|| {
                     let mut a = Allocator::new();
                     let start = Instant::now();
 
                     let conds = run_block_generator::<_, MempoolVisitor>(
                         &mut a,
-                        &gen,
+                        gen,
                         &block_refs,
                         11000000000,
                         ALLOW_BACKREFS,
                     );
                     let _ = black_box(conds);
                     start.elapsed()
                 })
@@ -65,15 +65,15 @@
             group.bench_function(format!("run_block_generator2 {name}{name_suffix}"), |b| {
                 b.iter(|| {
                     let mut a = Allocator::new();
                     let start = Instant::now();
 
                     let conds = run_block_generator2::<_, MempoolVisitor>(
                         &mut a,
-                        &gen,
+                        gen,
                         &block_refs,
                         11000000000,
                         ALLOW_BACKREFS,
                     );
                     let _ = black_box(conds);
                     start.elapsed()
                 })
```

### Comparing `chik_rs-0.5.2/docs/implementation-notes.md` & `chik_rs-0.6.0/crates/chik-consensus/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-Implementation notes
-====================
+## Implementation notes
 
 Here are some edge cases that may be easy to get wrong in other implementations.
 
-
-1. interpreting integers
-------------------------
+### Interpreting integers
 
 When interpreting atoms as integers in the conditions output from a SpendBundle,
 leading zeroes as well as sign-extending `0xff` bytes are allowed.
 
 As an optimization, all negative integers are either immediate failures (e.g. as
 a coin value) or turn the condition into a tautology (always true) (e.g. as a
 height or time condition). In the latter case, the whole condition can just be
@@ -17,48 +14,44 @@
 
 This leaves valid, positive integers with leading zeroes. The integers in
 conditions are always limited to 32 or 64 bits, but given leading zeroes, the
 atoms can potentially be a lot larger than that. This opens up a denial of
 service challenge. It's non-trivial to make an implementation scan and ignore
 leading zeroes efficient enough to be viable against such attacks. Because of
 this the mempool will reject Spend Bundles returning conditions with any
-*redundant* leading zeroes. (Note that in order to make an integer positive,
+_redundant_ leading zeroes. (Note that in order to make an integer positive,
 it's sometimes necessary to have a single leading zero. That wouldn't count as
 redundant).
 
 This implementation of condition parsing and checking is robust enough to
 withstand this attack, which currently can only be launched by a farmer (since
 the mempool rejects it for non-farmers).
 
-
-2. Relative height condition of 0
----------------------------------
+### Relative height condition of 0
 
 Similar to how some conditions with negative arguments are tautologies, so are
 some conditions with a 0 argument. E.g. `ASSERT_SECONDS_RELATIVE`
 `ASSERT_SECONDS_ABSOLUTE` `ASSERT_HEIGHT_ABSOLUTE`.
 
 Notably absent from this list is `ASSERT_HEIGHT_RELATIVE`. A relative height
 condition of 0 still prevents spending the coin in the same block (as an
 ephemeral coin). The `ASSERT_HEIGHT_RELATIVE` condition requires that the height
-difference between the creation of the coin and spending it *exceeds* the
+difference between the creation of the coin and spending it _exceeds_ the
 parameter (0 in this case).
 
-This is a bit of an inconsistency, since `ASSERT_SECONDS_RELATIVE` of 0 *does*
+This is a bit of an inconsistency, since `ASSERT_SECONDS_RELATIVE` of 0 _does_
 allow spending the coin in the same block. All spends in a block happen
-simultaneously, so the time difference between the spends doesn't *exceed* 0, it
-*is* 0.
+simultaneously, so the time difference between the spends doesn't _exceed_ 0, it
+_is_ 0.
 
-
-3. list NIL terminators
------------------------
+### List NIL terminators
 
 The output from a Spend Bundle or block generator program is expected to be:
 
-```
+```text
 (
   (
     (*parent-coin-id* *puzzle-hash* *amount*   # <- identify the coin to be spent
       (
         (
           (*condition-code* *condition-args...*)  # <- first condition
           ... # more conditions here. Must have valid terminator
@@ -68,57 +61,53 @@
     )
     ... # more spends here, must have valid terminator
   )
    *future-extensions*
 )
 ```
 
-Some of these lists *must* be terminated by a NIL atom, whereas others are
+Some of these lists _must_ be terminated by a NIL atom, whereas others are
 parsed forgivingly, just requiring the list to end with any atom on the right
 hand side.
 
 Lists requiring NIL termination:
 
 1. The list of Spends (i.e. identifying a coin to be spent along with the conditions)
 2. The list of conditions
 
 Lists not requiring NIL termination:
 
-1. The outer list of spends, that's there to allow for *future extensions*
-2. The outer list of conditions, there to allow for *future extensions*
+1. The outer list of spends, that's there to allow for _future extensions_
+2. The outer list of conditions, there to allow for _future extensions_
 3. The list of condition arguments
 
 A NIL terminator is an atom of length 0, used as the right-hand element at the end of the list.
 
-```
+```text
 (A . (B . (C . ())))
 ```
 
-A list that does not require a NIL terminator can end with *any* kind of atom. E.g.
+A list that does not require a NIL terminator can end with _any_ kind of atom. E.g.
 
-```
+```text
 (A . (B . (C . 8)))
 ```
 
-
-4. Additional arguments to conditions
--------------------------------------
+### Additional arguments to conditions
 
 Additional arguments are allowed to conditions, and ignored. This is to leave
 room for future expansion. One exception is the `AGG_SIG_UNSAFE` and
 `AGG_SIG_ME` conditions. They both require exactly 2 arguments. Anything else is
 a condition failure.
 
-5. Deduplicating identical spends
----------------------------------
+### Deduplicating identical spends
 
 The feature that deduplicates identical spends, in the mempool, can only work
 with spends that do not have any `AGG_SIG_ME` nor `AGG_SIG_UNSAFE` conditions.
 Because the signature cannot be subtracted from the aggregated siggnature in the
 general case. This feature is only active when these conditions are met:
 
-* The spend does not output an `AGG_SIG_ME` nor an `AGG_SIG_UNSAFE` condition.
-* The spend uses the exact same solution.
+- The spend does not output an `AGG_SIG_ME` nor an `AGG_SIG_UNSAFE` condition.
+- The spend uses the exact same solution.
 
 Spends that are eligible for deduplication are marked with a bool in the `Spend`
 object when running the generator.
-
```

### Comparing `chik_rs-0.5.2/generator-tests/block-834752-compressed.txt` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/solution_generator.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,302 @@
-ff01ffffffa022cf3c17be4e0e0e0b2e2a3f6dd1ee955528f737f0cb724247bc2e4a776cb989ffff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080fe81ffffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180fe7a8080ff80808080808080ffff01ff02ffff03ff17ff80fe837b7fffff018080fe3bffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53fe861db6d7ffffff808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080fe82f6ffff0180ffff04ffff09ffff18ff05fe8301d6fffe0effff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080fe861eeeb6ed77ff8080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101fe6f80ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17fe853b6da3ffff808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80fe841ecfffffff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bfe8307aeffff0180fe7b80ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa0f08eda9271f9dd1c00d9789ba0f3e4f547d66c8ad6f75edbb587b8c68d8ef5f1a0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff8202ffffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff82017fffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8202ff8080ff0bfffe2f80ff8080808080808080ffff01ff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02fe8876db6db7d77fffff80ff80808080ffff04ffff04ff1cffff04ff5fffff04ff8206bfff80808080ff80808080ff0180ffff04ffff01ffff32ff3d33ff3effff04ffff04ff1cffff04ff0bfe8503af5dffff80ffff04ffff04ff1cffff04ff05ffff04ff2fff80808080ffff04ffff04ff0afe87076db6edb7ffffffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080fe76808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1efe861dda75dfffffffff02ff1efe8677b4ebbfffff80fe8507a75dffffff0180fe7b80ffff04ffff01a02f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d57ffff04ffff01a0c4a8fb8a651c5e8636c6dd67ed8c8f7a70f516f41ab73abd14dd79c7582f079affff04ffff01b08116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6ffff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff01a022c0df3c66541eb57c226e12742a9f7182ceb0318cdaf5a84facb6c80bfaac1aff01808080808080fe81ff8080ff01ffffffa01daef44c653c413eba01d89790edfb613cb020ed0979d8447d6ed398327d0958ffa0976299e4fbb74e8732ae1ea7092ab617af435218f20912f99689d8fc69d12318fe3fff01ffffffff70c07101022f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d578116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6010000001668747470733a2f2f6575312e706f6f6c2e73706163650000004080ff80808080ffffa0e8058c610f8f50e5e603ad136f58ff3b1f0120a76bb4985553db8bda88738ca9ffff02fffe81abffff04ffff01fffe82ab5fffa0df84418c7ba1b1a847fa23bd1101fcee22b2bd81c69d10e6d4b280f09eba2c70fe8307ad7fffff04ffff01ff02fffe835adaffffff04fffe840aeb6bffffff04ffff01a09c117e3fba164415fb868361a5c6d9c8a4551c71e5a359807cb27810b80f23bdffff04ffff01b08a505367d099210c24f1be8945a83de7db6d9396a9742c8f609aebf7ba56bbaacb038819b122741211bbc9227c903573ffff04fffe86056dbadaffffffff04ffff01a0a78f9cbed5f7e1b529aa32088dcc3c53ac1df57bd0c8f4773f4c0ddae048a8edff01808080808080ff01808080ff01ffffffa0245c7e4ad426a2a6b6eb5622286d2fd8178fca04cdb9a23aeb8da08ae6d6e6c0ffa0c79f2213f98b1ac6bfa141b6724138223236e89ae456e6c6727f8709e4b28ed6fe7fff01ffffffff70c07101022f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d578a505367d099210c24f1be8945a83de7db6d9396a9742c8f609aebf7ba56bbaacb038819b122741211bbc9227c903573010000001668747470733a2f2f6e61312e706f6f6c2e73706163650000004080ff80808080ffffa0bc334d2f6b030790debd7e4a998a38d0628b2b853fa7895db16ce14da37c441dffff02fffe81abffff04ffff01fffe82ab5fffa01a3272c823c1175f83016303bfd33823687df39736e2b7eaf9057f00671d9f97fe8307ad7fffff04ffff01ff02fffe835adaffffff04ffff01a09d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ffff04ffff01a0e691c76d0108a7a7a44591b3784ecf4099bf5fb057173a0bb2f79fdfa2ed9fceffff04ffff01b0ab6824901d856c5a8c1664c990d1ef94a19ed7b4ab28a6b8e064f1a11e07f5e75bdb6ff8242f517534df36ae03c81da0ffff04fffe86056dbadaffffffff04ffff01a0ab43e98b62a2dc33caf0b16fb5a3c037e3303fc8e177ddf437eef233c87d32f2ff01808080808080ff01808080ff01ffffffa00afb9bf9c6a13d380c9645ae07e466bf71a171ae6fe35bc3a7ac5fb5df53a937ffa0cec914e2de9e524237e7a76f3d483a9cf1674be213d4c5bf51fe28b6dab92898ff0180ff01ffffffff70c07001029d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ab6824901d856c5a8c1664c990d1ef94a19ed7b4ab28a6b8e064f1a11e07f5e75bdb6ff8242f517534df36ae03c81da0010000001568747470733a2f2f636869612e64706f6f6c2e63630000002080ff80808080ffffa07016fd25c14831bfe48a08cd3cd9eeb6d416436087252e1061e62cdc95cc892affff02fffe81abffff04ffff01fffe82ab5fffa0cb75e5c90f2ab4bdf1db8a420e56e9edb261b919b73a6f8756453c07d73d430ffe8307ad7fffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff82017fffff01ff04ffff04ff1cfe8676db6edb7fffffff04ffff04ff12ffff04ff8205fffe8803b5ddb6b6bfffff80ffff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ffff04ff8205ffffff04ff8202ffff808080fe768080ff80808080ff80808080ffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff8202ffffff04ffff0bffff19ff2fffff18fffe8b15ab6db76db5b5ffffffffff8205ff8080ff0bfffe2f80ff808080808080808080ff0180ffff04ffff01ffff32ff3d52ffff333effff04ffff04ff12fe8675d76b6bffffffff04ffff04ff12fe870eb75dadafffffffff04ffff04ff1afe83edb7fffe873b6ebb5b5fffff8080fe8601f5dadafffffe7b80ffff04fffe840aeb6bffffff04ffff01a0a219765e3616e24fb86a7ddace966d0aacfcdb8d8b6823e9760e6b4a0469e07affff04ffff01b0afdbc8d2811665196a20931b06ffe981a2ec64aebd2d917478bf8441d77cb2b62f96194277d91983c5ca9edf0a17fdccffff04fffe86056dbadaffffffff04ffff0120ff01808080808080ff01808080ff01ffffffa0b3957791c7e84aa27e759b217ef97285c3c260b0410f230679a00a346ee695b4ffa03732f9605848b5ee1fe700dd36aab3aa23110d35c0e5917676d042883330c39aff0180ff01ffff01ffffff70c0570101016127e457a90eb12296658006a7928d5acffbe3c707b705177efe504d1beae0afdbc8d2811665196a20931b06ffe981a2ec64aebd2d917478bf8441d77cb2b62f96194277d91983c5ca9edf0a17fdcc000000000080ffa062e47157eea5430b839a8fcd8390ce3c162b61acd19f94eeb97db81d7622a52e808080ffffa0b63a7ce25b1050bfd97a9e4e67fcf42ca6545eaf392a13c67307ee3614e59bc2ffff02fffe81abffff04ffff01fffe82ab5fffa05a7cdf809298a6c314bfd6ec63c6761b396fca802c0067d87de23644d17a8bb5fe8307ad7fffff04ffff01ff02fffe835adaffffff04fffe840aeb6bffffff04ffff01a06dd75452b3a13128591f83a68263fb0dc9bedfb519af3af01933782ae65dca1bffff04ffff01b08e2ab4bd0f4b65f0e6e1cc1f54fd3a953a36afc98ec25a741958bf1f19d0a416f2b39b89d4bd9870f11d6bf09030780efe8576dd6d7fff808080ff01808080ff01ffffffa0f447a4cda2bd4e2c14398f96d1402e8ed0c35302b0c57f8219861d9433ba150cffa0eb4e5fc93add634ac692d2c28b0eed8dcdca399639cd7986dc6879c7a872e5f4ff0180ff01ffff01ffffff70c07701030213db9cb540a52c39071ef70acdf81796303189061b5aa0ee8098a05d5ceff58e2ab4bd0f4b65f0e6e1cc1f54fd3a953a36afc98ec25a741958bf1f19d0a416f2b39b89d4bd9870f11d6bf09030780e010000001c68747470733a2f2f7669702e746565706f6f6c2e636f6d3a393434330000002080ffa0a6322ec0a3d445a051349cf8289660b2d9686608484ecb42c135fd5bd4ea4b11808080ffffa077c52e138369b3a545a59f3daf2904197f350010676506eead7f5875f511f063ffff02fffe81abffff04ffff01fffe82ab5fffa00485de73367a4b49eb34c7f80df3c9b70c739411d40632428e42495da7c0ba91fe8307ad7fffff04ffff01ff02fffe835adaffffff04fffe840aeb6bffffff04ffff01a0671ce6fd24697788441f93773e5905c1f1153ba7f5d3fbb6a4e2855a05b42731ffff04ffff01b0a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7fe8576dd6d7fff808080ff01808080ff01ffffffa01dc8c9c3356a6eefee37744901b3f730c710052bd38deac264ecea45460faffeffa031460205316513dc6b11d0993462776f0994223cac2f215bf8afbeae5a0cce3fff0180ff01ffff01ffffff70c0730103e3b9adc4eb09d18d83bd56482aee566820f5afdce595b3ed095eb36c5cef9301a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7010000001868747470733a2f2f6368696170702e68706f6f6c2e636f6d0000004080ffa0fc0b1e9409ae5c3c40c50832a7aecc0b3ba4646568a00c01289c45e1f03b2b488080808080
-SPENDS:
-- coin id: 3c3412900b156403b13bb4191f1d6818619f73c97337829a4f821012b24d88eb ph: bc0e759db02410acb193d0c1c0a6841a2a821c9322570e2f23dfe220d9e6ae8f
-  ASSERT_HEIGHT_RELATIVE 32
-  CREATE_COIN: ph: 013beb3fa36f6d3f221253f7ef380e4d1197246b57b453ce32d339e9be4b2eec amount: 1
-  AGG_SIG_ME pk: afdbc8d2811665196a20931b06ffe981a2ec64aebd2d917478bf8441d77cb2b62f96194277d91983c5ca9edf0a17fdcc msg: f19e77711df9e26a0e1fda2279bd73d6dcb9afe91dafadb4c3c20b1fe441a1b3
-- coin id: 8522228562997c720038e6dca3721c36b054d766e0de80087ae9d7b4b229df29 ph: 1dc30429a17e6ee7d5b18a795da6bf838b7c87d0cf65cfb000fca5bab1ccbe19
-  CREATE_COIN: ph: c30e2a348a6a4f56fc8d4ce44cebda06f72420d68e454dd765ed40b782fca307 amount: 1
-  AGG_SIG_ME pk: 8a505367d099210c24f1be8945a83de7db6d9396a9742c8f609aebf7ba56bbaacb038819b122741211bbc9227c903573 msg: 6cbb9e5def3ed896de9651b54145afc27bcbba9c61ca853b1e3bf0e6b8a78e9a
-- coin id: a66d7b064c9fdfbcffe0755766c1a5d66899fab9f9a6cb4f93d614d676bc8292 ph: ba5089cb215c3f37dbc5718820d16d454694869e756653a516d2abb3faacd843
-  ASSERT_HEIGHT_RELATIVE 32
-  CREATE_COIN: ph: 87c64d9ef085869b1bf272816a752d093e272fa69d6840181cd48fa8eb86dcc3 amount: 1
-  AGG_SIG_ME pk: 8e2ab4bd0f4b65f0e6e1cc1f54fd3a953a36afc98ec25a741958bf1f19d0a416f2b39b89d4bd9870f11d6bf09030780e msg: 01f207c53eb38d9a0ca38981ddedf93c9d62ac0073f5706c1d513cc109206a00
-- coin id: afd297097757a8f5a3f3266933a6c29a7674c71028825562e7e4cac02b9228f6 ph: b78c1c1c0fe082b9c7f18d7e7c716b1607fd62dbdf3eef18f79e2717789ac55f
-  CREATE_COIN: ph: dca1429bcffab70d2218df91683ebe292305925337c0fffa91d5244838ffbd80 amount: 1
-  AGG_SIG_ME pk: 8116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6 msg: d497b66589f5d8bdc0631678cc488e25360d114eee51b84a3c1685771a7daa2d
-- coin id: b4fa0835dd9d595cf3d3c5e574ce081c7cca37452c4c336caaf8fbf644c5b268 ph: 0ac6539fede8c4cd50610af58f82b8cc74c774577f0a098db8ab2f42e5e90a9f
-  CREATE_COIN: ph: 948a5a1b3367d80aebc23a7ae772b140b8626f908d5b921f9980a0f01280e3c8 amount: 1
-  AGG_SIG_ME pk: ab6824901d856c5a8c1664c990d1ef94a19ed7b4ab28a6b8e064f1a11e07f5e75bdb6ff8242f517534df36ae03c81da0 msg: 38442a894ff28abb1225d3698c2e09aaea12827c9141f9e4c85267a38cec3e6f
-- coin id: ed418e8b3f49d86a0ab42343e1dc864f796026b8646c953a3bd54329a3843c1f ph: 87864b58be87e5f0fe566955088597ea0f5aafaad1ce0ed8dd02f5c84d257aa6
-  ASSERT_HEIGHT_RELATIVE 32
-  CREATE_COIN: ph: 70aea9db5a7c74a2dfa632ddac0e7cd3283c6439c1feae0417645b6392104ded amount: 1
-  AGG_SIG_ME pk: a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7 msg: 5d53d6baf98f40ce52d588135fa97fc7c6756c6fb6315298902d631548704d8c
-cost: 93787080
-removal_amount: 6
-addition_amount: 6
+use chik_protocol::Coin;
+use klvmr::allocator::{Allocator, NodePtr};
+use klvmr::serde::{node_from_bytes_backrefs, node_to_bytes, node_to_bytes_backrefs};
+use std::io;
+
+// the tuple has the Coin, puzzle-reveal and solution
+fn build_generator<BufRef, I>(a: &mut Allocator, spends: I) -> io::Result<NodePtr>
+where
+    BufRef: AsRef<[u8]>,
+    I: IntoIterator<Item = (Coin, BufRef, BufRef)>,
+{
+    // the generator we produce here is just a quoted list. Nothing fancy.
+    // Its format is as follows:
+    // (q . ( ( ( parent-id puzzle-reveal amount solution ) ... ) ) )
+
+    let mut spend_list = a.nil();
+    for s in spends {
+        let item = a.nil();
+        // solution
+        let solution = node_from_bytes_backrefs(a, s.2.as_ref())?;
+        let item = a.new_pair(solution, item)?;
+        // amount
+        let amount = a.new_number(s.0.amount.into())?;
+        let item = a.new_pair(amount, item)?;
+        // puzzle reveal
+        let puzzle = node_from_bytes_backrefs(a, s.1.as_ref())?;
+        let item = a.new_pair(puzzle, item)?;
+        // parent-id
+        let parent_id = a.new_atom(&s.0.parent_coin_info)?;
+        let item = a.new_pair(parent_id, item)?;
+
+        spend_list = a.new_pair(item, spend_list)?;
+    }
+
+    // the list of spends is the first (and only) item in an outer list
+    spend_list = a.new_pair(spend_list, a.nil())?;
+
+    let quote = a.new_pair(a.one(), spend_list)?;
+    Ok(quote)
+}
+
+// the tuple has the Coin, puzzle-reveal and solution
+pub fn solution_generator<BufRef, I>(spends: I) -> io::Result<Vec<u8>>
+where
+    BufRef: AsRef<[u8]>,
+    I: IntoIterator<Item = (Coin, BufRef, BufRef)>,
+{
+    let mut a = Allocator::new();
+    let generator = build_generator(&mut a, spends)?;
+    node_to_bytes(&a, generator)
+}
+
+pub fn solution_generator_backrefs<BufRef, I>(spends: I) -> io::Result<Vec<u8>>
+where
+    BufRef: AsRef<[u8]>,
+    I: IntoIterator<Item = (Coin, BufRef, BufRef)>,
+{
+    let mut a = Allocator::new();
+    let generator = build_generator(&mut a, spends)?;
+    node_to_bytes_backrefs(&a, generator)
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use hex_literal::hex;
+    use klvmr::{run_program, ChikDialect};
+
+    const PUZZLE1: [u8; 291] = hex!(
+        "
+        ff02ffff01ff02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff
+        1dff0bffff1effff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080
+        808080ffff01ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff
+        04ffff04ff05ffff04ffff02ff06ffff04ff02ffff04ff17ff80808080ff8080
+        8080ffff02ff17ff2f808080ff0180ffff04ffff01ff32ff02ffff03ffff07ff
+        0580ffff01ff0bffff0102ffff02ff06ffff04ff02ffff04ff09ff80808080ff
+        ff02ff06ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff0580
+        80ff0180ff018080ffff04ffff01b08cf5533a94afae0f4613d3ea565e47abc5
+        373415967ef5824fd009c602cb629e259908ce533c21de7fd7a68eb96c52d0ff
+        018080"
+    );
+
+    const SOLUTION1: [u8; 47] = hex!(
+        "
+        ff80ffff01ffff3dffa080115c1c71035a2cd60a49499fb9e5cb55be8d6e25e8
+        680bfc0409b7acaeffd48080ff8080"
+    );
+
+    const PUZZLE2: [u8; 99] = hex!(
+        "
+        ff01ffff33ffa01b7ab2079fa635554ad9bd4812c622e46ee3b1875a7813afba
+        127bb0cc9794f9ff887f808e9291e6c00080ffff33ffa06f184a7074c925ef86
+        88ce56941eb8929be320265f824ec7e351356cc745d38aff887f808e9291e6c0
+        008080"
+    );
+
+    const SOLUTION2: [u8; 1] = hex!("80");
+
+    fn run_generator(program: &[u8]) -> Vec<u8> {
+        let dialect = ChikDialect::new(0);
+        let mut a = Allocator::new();
+        let program = node_from_bytes_backrefs(&mut a, program).expect("node_from_bytes");
+        let env = a.nil();
+        let generator_output = run_program(&mut a, &dialect, program, env, 11000000000)
+            .expect("run_program")
+            .1;
+        node_to_bytes(&a, generator_output).expect("node_to_bytes")
+    }
+
+    const EXPECTED_GENERATOR_OUTPUT: [u8; 536] = hex!(
+        "
+        ffffffa0ccd5bb71183532bff220ba46c268991a000000000000000000000000
+        00000000ffff01ffff33ffa01b7ab2079fa635554ad9bd4812c622e46ee3b187
+        5a7813afba127bb0cc9794f9ff887f808e9291e6c00080ffff33ffa06f184a70
+        74c925ef8688ce56941eb8929be320265f824ec7e351356cc745d38aff887f80
+        8e9291e6c0008080ff8900ff011d2523cd8000ff8080ffffa0ccd5bb71183532
+        bff220ba46c268991a00000000000000000000000000036840ffff02ffff01ff
+        02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff1dff0bffff1e
+        ffff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080808080ffff01
+        ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff04ffff04ff05
+        ffff04ffff02ff06ffff04ff02ffff04ff17ff80808080ff80808080ffff02ff
+        17ff2f808080ff0180ffff04ffff01ff32ff02ffff03ffff07ff0580ffff01ff
+        0bffff0102ffff02ff06ffff04ff02ffff04ff09ff80808080ffff02ff06ffff
+        04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff01
+        8080ffff04ffff01b08cf5533a94afae0f4613d3ea565e47abc5373415967ef5
+        824fd009c602cb629e259908ce533c21de7fd7a68eb96c52d0ff018080ff8601
+        977420dc00ffff80ffff01ffff3dffa080115c1c71035a2cd60a49499fb9e5cb
+        55be8d6e25e8680bfc0409b7acaeffd48080ff8080808080"
+    );
+
+    #[test]
+    fn test_solution_generator() {
+        let coin1: Coin = Coin::new(
+            hex!("ccd5bb71183532bff220ba46c268991a00000000000000000000000000036840").into(),
+            hex!("fcc78a9e396df6ceebc217d2446bc016e0b3d5922fb32e5783ec5a85d490cfb6").into(),
+            1750000000000,
+        );
+        let coin2: Coin = Coin::new(
+            hex!("ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000").into(),
+            hex!("d23da14695a188ae5708dd152263c4db883eb27edeb936178d4d988b8f3ce5fc").into(),
+            18375000000000000000,
+        );
+
+        let result = solution_generator([
+            (coin1.clone(), PUZZLE1.as_ref(), SOLUTION1.as_ref()),
+            (coin2.clone(), PUZZLE2.as_ref(), SOLUTION2.as_ref()),
+        ])
+        .expect("solution_generator");
+
+        assert_eq!(
+            result,
+            hex!(
+                "
+            ff01ffffffa0
+            ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000
+
+            ff
+
+            ff01ffff33ffa01b7ab2079fa635554ad9bd4812c622e46ee3b1875a7813afba
+            127bb0cc9794f9ff887f808e9291e6c00080ffff33ffa06f184a7074c925ef86
+            88ce56941eb8929be320265f824ec7e351356cc745d38aff887f808e9291e6c0
+            008080
+
+            ff8900ff011d2523cd8000ff
+
+            80
+
+            80ffffa0
+
+            ccd5bb71183532bff220ba46c268991a00000000000000000000000000036840
+
+            ff
+
+            ff02ffff01ff02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff
+            1dff0bffff1effff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080
+            808080ffff01ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff
+            04ffff04ff05ffff04ffff02ff06ffff04ff02ffff04ff17ff80808080ff8080
+            8080ffff02ff17ff2f808080ff0180ffff04ffff01ff32ff02ffff03ffff07ff
+            0580ffff01ff0bffff0102ffff02ff06ffff04ff02ffff04ff09ff80808080ff
+            ff02ff06ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff0580
+            80ff0180ff018080ffff04ffff01b08cf5533a94afae0f4613d3ea565e47abc5
+            373415967ef5824fd009c602cb629e259908ce533c21de7fd7a68eb96c52d0ff
+            018080
+
+            ff8601977420dc00ff
+
+            ff80ffff01ffff3dffa080115c1c71035a2cd60a49499fb9e5cb55be8d6e25e8
+            680bfc0409b7acaeffd48080ff8080
+
+            808080"
+            )
+        );
+
+        let generator_output = run_generator(&result);
+        assert_eq!(generator_output, EXPECTED_GENERATOR_OUTPUT);
+
+        let result = solution_generator([(coin2.clone(), PUZZLE2.as_ref(), SOLUTION2.as_ref())])
+            .expect("solution_generator");
+
+        assert_eq!(
+            result,
+            hex!(
+                "
+            ff01ffffffa0
+            ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000
+
+            ff
+
+            ff01ffff33ffa01b7ab2079fa635554ad9bd4812c622e46ee3b1875a7813afba
+            127bb0cc9794f9ff887f808e9291e6c00080ffff33ffa06f184a7074c925ef86
+            88ce56941eb8929be320265f824ec7e351356cc745d38aff887f808e9291e6c0
+            008080
+
+            ff8900ff011d2523cd8000ff
+
+            80
+
+            808080"
+            )
+        );
+    }
+
+    #[test]
+    fn test_solution_generator_backre() {
+        let coin1: Coin = Coin::new(
+            hex!("ccd5bb71183532bff220ba46c268991a00000000000000000000000000036840").into(),
+            hex!("fcc78a9e396df6ceebc217d2446bc016e0b3d5922fb32e5783ec5a85d490cfb6").into(),
+            1750000000000,
+        );
+        let coin2: Coin = Coin::new(
+            hex!("ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000").into(),
+            hex!("d23da14695a188ae5708dd152263c4db883eb27edeb936178d4d988b8f3ce5fc").into(),
+            18375000000000000000,
+        );
+
+        let result = solution_generator_backrefs([
+            (coin1.clone(), PUZZLE1.as_ref(), SOLUTION1.as_ref()),
+            (coin2.clone(), PUZZLE2.as_ref(), SOLUTION2.as_ref()),
+        ])
+        .expect("solution_generator");
+
+        assert_eq!(
+            result,
+            hex!(
+                "
+                ff01ffffffa0
+
+                ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000
+
+                ff
+
+                ff01ffff33ffa01b7ab2079fa635554ad9bd4812c622e46ee3b1875a7813afba
+                127bb0cc9794f9ff887f808e9291e6c00080ffff33ffa06f184a7074c925ef86
+                88ce56941eb8929be320265f824ec7e351356cc745d38a
+
+                fe3b
+
+                80ff8900ff011d2523cd8000ff8080ffffa0
+
+                ccd5bb71183532bff220ba46c268991a00000000000000000000000000036840
+
+                ff
+
+                ff02ffff01ff02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff
+                1dff0bffff1effff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080
+                808080ffff01ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff
+                04ffff04ff05ffff04ff
+
+                fe8401
+
+                6b6b7fff80808080ff
+
+                fe820d
+
+                b78080
+
+                fe81f6
+
+                ffff04ffff01ff32ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff
+                06ffff04ff02ffff04ff09ff80808080ffff02ff06ffff04ff02ffff04ff0dff
+                8080808080ffff01ff0bffff0101
+
+                fe6f
+
+                80ff0180
+
+                fe3e
+
+                80ffff04ffff01b08cf5533a94afae0f4613d3ea565e47abc5373415967ef582
+                4fd009c602cb629e259908ce533c21de7fd7a68eb96c52d0
+
+                fe7f
+
+                80ff8601977420dc00ffff80ffff01ffff3dffa080115c1c71035a2cd60a4949
+                9fb9e5cb55be8d6e25e8680bfc0409b7acaeffd48080ff8080808080"
+            )
+        );
+
+        let generator_output = run_generator(&result);
+        assert_eq!(generator_output, EXPECTED_GENERATOR_OUTPUT);
+    }
+}
```

### Comparing `chik_rs-0.5.2/src/error.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/src/fast_forward.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/fast_forward.rs`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     // compute the coin being spent (before the fast-forward).
     let parent_coin = Coin {
         parent_coin_info: new_solution.lineage_proof.parent_parent_coin_id,
         puzzle_hash: parent_puzzle_hash,
         amount: new_solution.lineage_proof.parent_amount,
     };
 
-    if parent_coin.coin_id() != *coin.parent_coin_info {
+    if parent_coin.coin_id() != coin.parent_coin_info {
         return Err(Error::ParentCoinMismatch);
     }
 
     let inner_puzzle_hash = tree_hash(a, singleton.args.inner_puzzle);
     if inner_puzzle_hash != *new_solution.lineage_proof.parent_inner_puzzle_hash {
         return Err(Error::InnerPuzzleHashMismatch);
     }
@@ -162,15 +162,15 @@
     // update the solution to use the new parent coin's information
     new_solution.lineage_proof.parent_parent_coin_id = new_parent.parent_coin_info;
     new_solution.lineage_proof.parent_amount = new_parent.amount;
     new_solution.amount = new_coin.amount;
 
     let expected_new_parent = new_parent.coin_id();
 
-    if *new_coin.parent_coin_info != expected_new_parent {
+    if new_coin.parent_coin_info != expected_new_parent {
         return Err(Error::CoinMismatch);
     }
 
     Ok(new_solution.to_klvm(a)?)
 }
 
 #[cfg(test)]
@@ -199,15 +199,16 @@
             "0000000000000000000000000000000000000000000000000000000000000000",
             "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff"
         )]
         new_parents_parent: &str,
         #[values(0, 1, 3, 5)] new_amount: u64,
         #[values(0, 1, 3, 5)] prev_amount: u64,
     ) {
-        let spend_bytes = fs::read(format!("ff-tests/{spend_file}.spend")).expect("read file");
+        let spend_bytes =
+            fs::read(format!("../../ff-tests/{spend_file}.spend")).expect("read file");
         let spend = CoinSpend::from_bytes(&spend_bytes).expect("parse CoinSpend");
         let new_parents_parent = hex::decode(new_parents_parent).unwrap();
 
         let mut a = Allocator::new_limited(500000000);
         let puzzle = spend.puzzle_reveal.to_node_ptr(&mut a).expect("to_klvm");
         let solution = spend.solution.to_node_ptr(&mut a).expect("to_klvm");
         let puzzle_hash = Bytes32::from(tree_hash(&a, puzzle));
@@ -219,15 +220,15 @@
                 spend.coin.amount
             } else {
                 prev_amount
             },
         };
 
         let new_coin = Coin {
-            parent_coin_info: new_parent_coin.coin_id().into(),
+            parent_coin_info: new_parent_coin.coin_id(),
             puzzle_hash,
             amount: if new_amount == 0 {
                 spend.coin.amount
             } else {
                 new_amount
             },
         };
@@ -271,15 +272,15 @@
         assert!(conditions1.spends[0].create_coin == conditions2.spends[0].create_coin);
     }
 
     fn run_ff_test(
         mutate: fn(&mut Allocator, &mut Coin, &mut Coin, &mut Coin, &mut Vec<u8>, &mut Vec<u8>),
         expected_err: Error,
     ) {
-        let spend_bytes = fs::read("ff-tests/e3c0.spend").expect("read file");
+        let spend_bytes = fs::read("../../ff-tests/e3c0.spend").expect("read file");
         let mut spend = CoinSpend::from_bytes(&spend_bytes).expect("parse CoinSpend");
         let new_parents_parent: &[u8] =
             &hex!("abababababababababababababababababababababababababababababababab");
 
         let mut a = Allocator::new_limited(500000000);
         let puzzle = spend.puzzle_reveal.to_node_ptr(&mut a).expect("to_klvm");
         let puzzle_hash = Bytes32::from(tree_hash(&a, puzzle));
@@ -287,15 +288,15 @@
         let mut new_parent_coin = Coin {
             parent_coin_info: new_parents_parent.try_into().unwrap(),
             puzzle_hash,
             amount: spend.coin.amount,
         };
 
         let mut new_coin = Coin {
-            parent_coin_info: new_parent_coin.coin_id().into(),
+            parent_coin_info: new_parent_coin.coin_id(),
             puzzle_hash,
             amount: spend.coin.amount,
         };
 
         let mut puzzle = spend.puzzle_reveal.as_slice().to_vec();
         let mut solution = spend.solution.as_slice().to_vec();
         mutate(
@@ -458,15 +459,15 @@
                     parent_coin_info: new_solution.lineage_proof.parent_parent_coin_id,
                     puzzle_hash: parent_puzzle_hash,
                     amount: new_solution.lineage_proof.parent_amount,
                 };
 
                 new_coin.puzzle_hash = parent_puzzle_hash;
 
-                coin.parent_coin_info = new_parent.coin_id().into();
+                coin.parent_coin_info = new_parent.coin_id();
                 coin.puzzle_hash = parent_puzzle_hash;
             },
             Error::InnerPuzzleHashMismatch,
         );
     }
 
     #[test]
```

### Comparing `chik_rs-0.5.2/src/gen/coin_id.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/coin_id.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/src/gen/conditions.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/conditions.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 use super::coin_id::compute_coin_id;
-use super::condition_sanitizers::{parse_amount, sanitize_announce_msg, sanitize_hash};
+use super::condition_sanitizers::{
+    parse_amount, sanitize_announce_msg, sanitize_hash, sanitize_message_mode,
+};
 use super::opcodes::{
     compute_unknown_condition_cost, parse_opcode, ConditionOpcode, AGG_SIG_AMOUNT, AGG_SIG_COST,
     AGG_SIG_ME, AGG_SIG_PARENT, AGG_SIG_PARENT_AMOUNT, AGG_SIG_PARENT_PUZZLE, AGG_SIG_PUZZLE,
     AGG_SIG_PUZZLE_AMOUNT, AGG_SIG_UNSAFE, ASSERT_BEFORE_HEIGHT_ABSOLUTE,
     ASSERT_BEFORE_HEIGHT_RELATIVE, ASSERT_BEFORE_SECONDS_ABSOLUTE, ASSERT_BEFORE_SECONDS_RELATIVE,
     ASSERT_COIN_ANNOUNCEMENT, ASSERT_CONCURRENT_PUZZLE, ASSERT_CONCURRENT_SPEND, ASSERT_EPHEMERAL,
     ASSERT_HEIGHT_ABSOLUTE, ASSERT_HEIGHT_RELATIVE, ASSERT_MY_AMOUNT, ASSERT_MY_BIRTH_HEIGHT,
     ASSERT_MY_BIRTH_SECONDS, ASSERT_MY_COIN_ID, ASSERT_MY_PARENT_ID, ASSERT_MY_PUZZLEHASH,
     ASSERT_PUZZLE_ANNOUNCEMENT, ASSERT_SECONDS_ABSOLUTE, ASSERT_SECONDS_RELATIVE, CREATE_COIN,
-    CREATE_COIN_ANNOUNCEMENT, CREATE_COIN_COST, CREATE_PUZZLE_ANNOUNCEMENT, REMARK, RESERVE_FEE,
-    SOFTFORK,
+    CREATE_COIN_ANNOUNCEMENT, CREATE_COIN_COST, CREATE_PUZZLE_ANNOUNCEMENT, RECEIVE_MESSAGE,
+    REMARK, RESERVE_FEE, SEND_MESSAGE, SOFTFORK,
 };
 use super::sanitize_int::{sanitize_uint, SanitizedUint};
 use super::validation_error::{first, next, rest, ErrorCode, ValidationErr};
 use crate::gen::flags::{
     AGG_SIG_ARGS, COND_ARGS_NIL, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS,
     STRICT_ARGS_COUNT,
 };
+use crate::gen::messages::{Message, SpendId};
 use crate::gen::spend_visitor::SpendVisitor;
 use crate::gen::validation_error::check_nil;
 use chik_protocol::bytes::Bytes32;
 use klvmr::allocator::{Allocator, NodePtr, SExp};
 use klvmr::cost::Cost;
 use klvmr::sha2::{Digest, Sha256};
 use std::cmp::{max, min};
@@ -117,26 +120,43 @@
             Condition::AggSigParentPuzzle(_, _) => {
                 spend.flags &= !ELIGIBLE_FOR_DEDUP;
                 spend.flags &= !ELIGIBLE_FOR_FF;
             }
             Condition::AggSigUnsafe(_, _) => {
                 spend.flags &= !ELIGIBLE_FOR_DEDUP;
             }
+            Condition::SendMessage(src_mode, _dst, _msg) => {
+                if (src_mode & super::messages::PARENT) != 0 {
+                    spend.flags &= !ELIGIBLE_FOR_FF;
+                }
+                // de-duplicating a coin spend that's sending a message may
+                // leave a receiver without a message, which is a failure
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
+            Condition::ReceiveMessage(_src, dst_mode, _msg) => {
+                if (dst_mode & super::messages::PARENT) != 0 {
+                    spend.flags &= !ELIGIBLE_FOR_FF;
+                }
+                // de-duplicating a coin spend that's receiving a message may
+                // leave a sent-message un-received, which is a failure
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
             _ => {}
         }
         self.condition_counter += 1;
     }
 
     fn post_spend(&mut self, a: &Allocator, spend: &mut Spend) {
         // if this still looks like it might be a singleton, check the output coins
         // to look for something that looks like a singleton output, with the same
         // puzzle hash as our input coin
         if (spend.flags & ELIGIBLE_FOR_FF) != 0
             && !spend.create_coin.iter().any(|c| {
-                (c.amount & 1) == 1 && a.atom(spend.puzzle_hash) == c.puzzle_hash.as_slice()
+                (c.amount & 1) == 1
+                    && a.atom(spend.puzzle_hash).as_ref() == c.puzzle_hash.as_slice()
             })
         {
             spend.flags &= !ELIGIBLE_FOR_FF;
         }
     }
 }
 
@@ -164,15 +184,15 @@
 // ((<coin-parent-id> <coind-puzzle-hash> <coin-amount> (
 //  (
 //    (CREATE_COIN <puzzle-hash> <amount>)
 //    (ASSERT_HEIGHT_ABSOLUTE <height>)
 //  )
 // )))
 
-#[derive(PartialEq, Hash, Eq, Debug)]
+#[derive(Debug)]
 pub enum Condition {
     // pubkey (48 bytes) and message (<= 1024 bytes)
     AggSigUnsafe(NodePtr, NodePtr),
     AggSigMe(NodePtr, NodePtr),
     AggSigParent(NodePtr, NodePtr),
     AggSigPuzzle(NodePtr, NodePtr),
     AggSigAmount(NodePtr, NodePtr),
@@ -219,14 +239,18 @@
     AssertBeforeHeightAbsolute(u32),
     AssertEphemeral,
 
     // The softfork condition is one that we don't understand, it just applies
     // the specified cost
     Softfork(Cost),
 
+    // source, destination, message
+    SendMessage(u8, SpendId, NodePtr),
+    ReceiveMessage(SpendId, u8, NodePtr),
+
     // this means the condition is unconditionally true and can be skipped
     Skip,
     SkipRelativeCondition,
 }
 
 fn maybe_check_args_terminator(
     a: &Allocator,
@@ -247,15 +271,15 @@
 ) -> Result<Condition, ValidationErr> {
     match op {
         AGG_SIG_UNSAFE => {
             let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_UNSAFE takes exactly two parameters
-            if (flags & COND_ARGS_NIL) != 0 {
+            if (flags & COND_ARGS_NIL) != 0 || (flags & STRICT_ARGS_COUNT) != 0 {
                 // make sure there aren't more than two
                 check_nil(a, rest(a, c)?)?;
                 Ok(Condition::AggSigUnsafe(pubkey, message))
             } else if (flags & AGG_SIG_ARGS) == 0 {
                 // but the argument list still doesn't need to be terminated by NIL,
                 // just any atom will do
                 match a.sexp(rest(a, c)?) {
@@ -267,15 +291,15 @@
             }
         }
         AGG_SIG_ME => {
             let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_ME takes exactly two parameters
-            if (flags & COND_ARGS_NIL) != 0 {
+            if (flags & COND_ARGS_NIL) != 0 || (flags & STRICT_ARGS_COUNT) != 0 {
                 // make sure there aren't more than two
                 check_nil(a, rest(a, c)?)?;
                 Ok(Condition::AggSigMe(pubkey, message))
             } else if (flags & AGG_SIG_ARGS) == 0 {
                 // but the argument list still doesn't need to be terminated by NIL,
                 // just any atom will do
                 match a.sexp(rest(a, c)?) {
@@ -540,14 +564,47 @@
             let code = ErrorCode::AssertBeforeHeightAbsolute;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Ok(Condition::Skip),
                 SanitizedUint::NegativeOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertBeforeHeightAbsolute(r as u32)),
             }
         }
+        SEND_MESSAGE => {
+            let mode = sanitize_message_mode(a, first(a, c)?, flags)?;
+            c = rest(a, c)?;
+            let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
+            c = rest(a, c)?;
+            let dst = SpendId::parse(a, &mut c, (mode & 0b111) as u8)?;
+
+            if (flags & STRICT_ARGS_COUNT) != 0 {
+                check_nil(a, c)?;
+            }
+
+            Ok(Condition::SendMessage(
+                ((mode >> 3) & 0b111) as u8,
+                dst,
+                message,
+            ))
+        }
+        RECEIVE_MESSAGE => {
+            let mode = sanitize_message_mode(a, first(a, c)?, flags)?;
+            c = rest(a, c)?;
+            let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
+            c = rest(a, c)?;
+            let src = SpendId::parse(a, &mut c, ((mode >> 3) & 0b111) as u8)?;
+
+            if (flags & STRICT_ARGS_COUNT) != 0 {
+                check_nil(a, c)?;
+            }
+            Ok(Condition::ReceiveMessage(
+                src,
+                (mode & 0b111) as u8,
+                message,
+            ))
+        }
         REMARK => {
             // this condition is always true, we always ignore arguments
             Ok(Condition::Skip)
         }
         _ => Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode)),
     }
 }
@@ -697,14 +754,19 @@
     announce_puzzle: HashSet<(NodePtr, NodePtr)>,
 
     // the assert announcements are checked once everything has been parsed and
     // validated.
     assert_coin: HashSet<NodePtr>,
     assert_puzzle: HashSet<NodePtr>,
 
+    // These are just list of all the messages being sent or received. There's
+    // no deduplication. We defer resolving and checking the messages until
+    // after we're done parsing all conditions for all spends
+    messages: Vec<Message>,
+
     // the assert concurrent spend coin IDs are inserted into this set and
     // checked once everything has been parsed.
     assert_concurrent_spend: HashSet<NodePtr>,
 
     // the assert concurrent puzzle hashes are inserted into this set and
     // checked once everything has been parsed.
     assert_concurrent_puzzle: HashSet<NodePtr>,
@@ -769,15 +831,20 @@
     max_cost: &mut Cost,
 ) -> Result<(), ValidationErr> {
     let parent_id = sanitize_hash(a, parent_id, 32, ErrorCode::InvalidParentId)?;
     let puzzle_hash = sanitize_hash(a, puzzle_hash, 32, ErrorCode::InvalidPuzzleHash)?;
     let my_amount = parse_amount(a, amount, ErrorCode::InvalidCoinAmount)?;
     let amount_buf = a.atom(amount);
 
-    let coin_id = Arc::new(compute_coin_id(a, parent_id, puzzle_hash, amount_buf));
+    let coin_id = Arc::new(compute_coin_id(
+        a,
+        parent_id,
+        puzzle_hash,
+        amount_buf.as_ref(),
+    ));
 
     if state
         .spent_coins
         .insert(coin_id.clone(), ret.spends.len())
         .is_some()
     {
         // if this coin ID has already been added to this set, it's a double
@@ -834,24 +901,21 @@
     max_cost: &mut Cost,
     visitor: &mut V,
 ) -> Result<(), ValidationErr> {
     let mut announce_countdown: u32 = 1024;
 
     while let Some((mut c, next)) = next(a, iter)? {
         iter = next;
-        let op = match parse_opcode(a, first(a, c)?, flags) {
-            None => {
-                // in strict mode we don't allow unknown conditions
-                if (flags & NO_UNKNOWN_CONDS) != 0 {
-                    return Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode));
-                }
-                // in non-strict mode, we just ignore unknown conditions
-                continue;
+        let Some(op) = parse_opcode(a, first(a, c)?, flags) else {
+            // in strict mode we don't allow unknown conditions
+            if (flags & NO_UNKNOWN_CONDS) != 0 {
+                return Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode));
             }
-            Some(v) => v,
+            // in non-strict mode, we just ignore unknown conditions
+            continue;
         };
 
         // subtract the max_cost based on the current condition
         // in case we exceed the limit, we want to fail as early as possible
         match op {
             CREATE_COIN => {
                 if *max_cost < CREATE_COIN_COST {
@@ -883,15 +947,15 @@
                 ret.reserve_fee = ret
                     .reserve_fee
                     .checked_add(limit)
                     .ok_or(ValidationErr(c, ErrorCode::ReserveFeeConditionFailed))?;
             }
             Condition::CreateCoin(ph, amount, hint) => {
                 let new_coin = NewCoin {
-                    puzzle_hash: a.atom(ph).try_into().unwrap(),
+                    puzzle_hash: a.atom(ph).as_ref().try_into().unwrap(),
                     amount,
                     hint,
                 };
                 if !spend.create_coin.insert(new_coin) {
                     return Err(ValidationErr(c, ErrorCode::DuplicateOutput));
                 }
                 ret.addition_amount += amount as u128;
@@ -997,15 +1061,15 @@
                 if let Some(existing) = ret.before_height_absolute {
                     ret.before_height_absolute = Some(min(existing, h));
                 } else {
                     ret.before_height_absolute = Some(h);
                 }
             }
             Condition::AssertMyCoinId(id) => {
-                if a.atom(id) != (*spend.coin_id).as_ref() {
+                if a.atom(id).as_ref() != (*spend.coin_id).as_ref() {
                     return Err(ValidationErr(c, ErrorCode::AssertMyCoinIdFailed));
                 }
             }
             Condition::AssertMyAmount(amount) => {
                 if amount != spend.coin_amount {
                     return Err(ValidationErr(c, ErrorCode::AssertMyAmountFailed));
                 }
@@ -1030,20 +1094,20 @@
                 spend.birth_height = Some(h);
                 assert_not_ephemeral(&mut spend.flags, state, ret.spends.len());
             }
             Condition::AssertEphemeral => {
                 state.assert_ephemeral.insert(ret.spends.len());
             }
             Condition::AssertMyParentId(id) => {
-                if a.atom(id) != a.atom(spend.parent_id) {
+                if a.atom(id).as_ref() != a.atom(spend.parent_id).as_ref() {
                     return Err(ValidationErr(c, ErrorCode::AssertMyParentIdFailed));
                 }
             }
             Condition::AssertMyPuzzlehash(hash) => {
-                if a.atom(hash) != a.atom(spend.puzzle_hash) {
+                if a.atom(hash).as_ref() != a.atom(spend.puzzle_hash).as_ref() {
                     return Err(ValidationErr(c, ErrorCode::AssertMyPuzzlehashFailed));
                 }
             }
             Condition::CreateCoinAnnouncement(msg) => {
                 decrement(&mut announce_countdown, msg)?;
                 state.announce_coin.insert((spend.coin_id.clone(), msg));
             }
@@ -1093,14 +1157,46 @@
             }
             Condition::Softfork(cost) => {
                 if *max_cost < cost {
                     return Err(ValidationErr(c, ErrorCode::CostExceeded));
                 }
                 *max_cost -= cost;
             }
+            Condition::SendMessage(src_mode, dst, msg) => {
+                decrement(&mut announce_countdown, msg)?;
+                let src = SpendId::from_self(
+                    src_mode,
+                    spend.parent_id,
+                    spend.puzzle_hash,
+                    spend.coin_amount,
+                    &spend.coin_id,
+                )?;
+                state.messages.push(Message {
+                    src,
+                    dst,
+                    msg,
+                    counter: 1,
+                });
+            }
+            Condition::ReceiveMessage(src, dst_mode, msg) => {
+                decrement(&mut announce_countdown, msg)?;
+                let dst = SpendId::from_self(
+                    dst_mode,
+                    spend.parent_id,
+                    spend.puzzle_hash,
+                    spend.coin_amount,
+                    &spend.coin_id,
+                )?;
+                state.messages.push(Message {
+                    src,
+                    dst,
+                    msg,
+                    counter: -1,
+                });
+            }
             Condition::SkipRelativeCondition => {
                 assert_not_ephemeral(&mut spend.flags, state, ret.spends.len());
             }
             Condition::Skip => {}
         }
     }
 
@@ -1113,26 +1209,26 @@
 fn is_ephemeral(
     a: &Allocator,
     spend_idx: usize,
     spent_ids: &HashMap<Arc<Bytes32>, usize>,
     spends: &[Spend],
 ) -> bool {
     let spend = &spends[spend_idx];
-    let idx = match spent_ids.get(&Bytes32::try_from(a.atom(spend.parent_id)).unwrap()) {
+    let idx = match spent_ids.get(&Bytes32::try_from(a.atom(spend.parent_id).as_ref()).unwrap()) {
         None => {
             return false;
         }
         Some(idx) => *idx,
     };
 
     // then lookup the coin (puzzle hash, amount) in its set of created
     // coins. Note that hint is not relevant for this lookup
     let parent_spend = &spends[idx];
     parent_spend.create_coin.contains(&NewCoin {
-        puzzle_hash: Bytes32::try_from(a.atom(spend.puzzle_hash)).unwrap(),
+        puzzle_hash: Bytes32::try_from(a.atom(spend.puzzle_hash).as_ref()).unwrap(),
         amount: spend.coin_amount,
         hint: a.nil(),
     })
 }
 
 // This function parses, and validates aspects of, the above structure and
 // returns a list of all spends, along with all conditions, organized by
@@ -1219,34 +1315,34 @@
         }
     }
 
     // check concurrent spent assertions
     for coin_id in state.assert_concurrent_spend {
         if !state
             .spent_coins
-            .contains_key(&Bytes32::try_from(a.atom(coin_id)).unwrap())
+            .contains_key(&Bytes32::try_from(a.atom(coin_id).as_ref()).unwrap())
         {
             return Err(ValidationErr(
                 coin_id,
                 ErrorCode::AssertConcurrentSpendFailed,
             ));
         }
     }
 
     if !state.assert_concurrent_puzzle.is_empty() {
         let mut spent_phs = HashSet::<Bytes32>::new();
 
         // expand all the spent puzzle hashes into a set, to allow
         // fast lookups of all assertions
         for ph in state.spent_puzzles {
-            spent_phs.insert(a.atom(ph).try_into().unwrap());
+            spent_phs.insert(a.atom(ph).as_ref().try_into().unwrap());
         }
 
         for puzzle_assert in state.assert_concurrent_puzzle {
-            if !spent_phs.contains(&a.atom(puzzle_assert).try_into().unwrap()) {
+            if !spent_phs.contains(&a.atom(puzzle_assert).as_ref().try_into().unwrap()) {
                 return Err(ValidationErr(
                     puzzle_assert,
                     ErrorCode::AssertConcurrentPuzzleFailed,
                 ));
             }
         }
     }
@@ -1261,15 +1357,15 @@
             hasher.update(*coin_id);
             hasher.update(a.atom(announce));
             let announcement_id: [u8; 32] = hasher.finalize().into();
             announcements.insert(announcement_id.into());
         }
 
         for coin_assert in state.assert_coin {
-            if !announcements.contains(&a.atom(coin_assert).try_into().unwrap()) {
+            if !announcements.contains(&a.atom(coin_assert).as_ref().try_into().unwrap()) {
                 return Err(ValidationErr(
                     coin_assert,
                     ErrorCode::AssertCoinAnnouncementFailed,
                 ));
             }
         }
     }
@@ -1304,23 +1400,44 @@
             hasher.update(a.atom(puzzle_hash));
             hasher.update(a.atom(announce));
             let announcement_id: [u8; 32] = hasher.finalize().into();
             announcements.insert(announcement_id.into());
         }
 
         for puzzle_assert in state.assert_puzzle {
-            if !announcements.contains(&a.atom(puzzle_assert).try_into().unwrap()) {
+            if !announcements.contains(&a.atom(puzzle_assert).as_ref().try_into().unwrap()) {
                 return Err(ValidationErr(
                     puzzle_assert,
                     ErrorCode::AssertPuzzleAnnouncementFailed,
                 ));
             }
         }
     }
 
+    if !state.messages.is_empty() {
+        // the integers count the number of times the message has been sent
+        // minus the number of times it's been received. At the end we ensure
+        // all counters are 0, otherwise some message wasn't received or sent
+        // the right number of times.
+        let mut messages = HashMap::<Vec<u8>, i32>::new();
+
+        for msg in &state.messages {
+            *messages.entry(msg.make_key(a)).or_insert(0) += msg.counter as i32;
+        }
+
+        for count in messages.values() {
+            if *count != 0 {
+                return Err(ValidationErr(
+                    NodePtr::NIL,
+                    ErrorCode::MessageNotSentOrReceived,
+                ));
+            }
+        }
+    }
+
     // TODO: there may be more failures that can be detected early here, for
     // example an assert-my-birth-height that's incompatible assert-height or
     // assert-before-height. Same thing for the seconds counterpart
 
     Ok(())
 }
 
@@ -1512,14 +1629,18 @@
     subs.insert("longmsg", a.new_atom(LONGMSG).unwrap());
     // coin IDs
     subs.insert("coin11", a.new_atom(&test_coin_id(H1, H1, 123)).unwrap());
     subs.insert("coin12", a.new_atom(&test_coin_id(H1, H2, 123)).unwrap());
     subs.insert("coin21", a.new_atom(&test_coin_id(H2, H1, 123)).unwrap());
     subs.insert("coin22", a.new_atom(&test_coin_id(H2, H2, 123)).unwrap());
     subs.insert(
+        "coin21_456",
+        a.new_atom(&test_coin_id(H2, H1, 456)).unwrap(),
+    );
+    subs.insert(
         "coin12_h2_42",
         a.new_atom(&test_coin_id(
             &test_coin_id(H1, H2, 123).as_ref().try_into().unwrap(),
             H2,
             42,
         ))
         .unwrap(),
@@ -1625,15 +1746,15 @@
     // ASSERT_SECONDS_RELATIVE
     let (a, conds) = cond_test_flag("((({h1} ({h2} (123 (((80 (50 8 ))))", 0).unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP | HAS_RELATIVE_CONDITION);
 
     assert_eq!(spend.seconds_relative, Some(50));
 }
 
 #[test]
 fn test_invalid_condition_args_terminator_mempool() {
@@ -1652,15 +1773,15 @@
     // ASSERT_SECONDS_RELATIVE
     let (a, conds) = cond_test_flag("((({h1} ({h2} (123 (((80 (50 8 ))))", 0).unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP | HAS_RELATIVE_CONDITION);
 
     assert_eq!(spend.seconds_relative, Some(50));
 }
 
 #[test]
 fn test_invalid_condition_list_terminator_mempool() {
@@ -1734,32 +1855,82 @@
 #[case(AGG_SIG_PUZZLE, "{pubkey} ({msg1}")]
 #[case(AGG_SIG_AMOUNT, "{pubkey} ({msg1}")]
 #[case(AGG_SIG_PUZZLE_AMOUNT, "{pubkey} ({msg1}")]
 #[case(AGG_SIG_PARENT_PUZZLE, "{pubkey} ({msg1}")]
 #[case(AGG_SIG_PARENT_AMOUNT, "{pubkey} ({msg1}")]
 #[case(ASSERT_CONCURRENT_SPEND, "{coin12}")]
 #[case(ASSERT_CONCURRENT_PUZZLE, "{h2}")]
-fn test_extra_arg_mempool(
+fn test_strict_args_count(
     #[case] condition: ConditionOpcode,
     #[case] arg: &str,
-    #[values(MEMPOOL_MODE, 0)] mempool: u32,
+    #[values(STRICT_ARGS_COUNT, 0)] flags: u32,
 ) {
-    // extra args are disallowed in mempool mode
-    assert_eq!(
-        cond_test_flag(
-            &format!(
-                "((({{h1}} ({{h2}} (123 ((({} ({} ( 1337 )))))",
-                condition as u8, arg
-            ),
-            STRICT_ARGS_COUNT | ENABLE_SOFTFORK_CONDITION | mempool
-        )
-        .unwrap_err()
-        .1,
-        ErrorCode::InvalidCondition
+    // extra args are disallowed when STRICT_ARGS_COUNT is set
+    let ret = cond_test_flag(
+        &format!(
+            "((({{h1}} ({{h2}} (123 ((({} ({} ( 1337 )))))",
+            condition as u8, arg
+        ),
+        flags | ENABLE_SOFTFORK_CONDITION | AGG_SIG_ARGS,
     );
+    if flags == 0 {
+        // two of the cases won't pass, even when garbage at the end is allowed.
+        if condition == ASSERT_COIN_ANNOUNCEMENT {
+            assert_eq!(ret.unwrap_err().1, ErrorCode::AssertCoinAnnouncementFailed,);
+        } else if condition == ASSERT_PUZZLE_ANNOUNCEMENT {
+            assert_eq!(
+                ret.unwrap_err().1,
+                ErrorCode::AssertPuzzleAnnouncementFailed,
+            );
+        } else {
+            assert!(ret.is_ok());
+        }
+    } else {
+        assert_eq!(ret.unwrap_err().1, ErrorCode::InvalidCondition);
+    }
+}
+
+#[cfg(test)]
+#[rstest]
+#[case(0x07, "0x1337", "({coin12}")]
+#[case(0x04, "0x1337", "({h1}")]
+#[case(0x06, "0x1337", "({h1} ({h2}")]
+#[case(0x05, "0x1337", "({h1} (123")]
+#[case(0x02, "0x1337", "({h2}")]
+#[case(0x03, "0x1337", "({h2} (123")]
+#[case(0x01, "0x1337", "(123")]
+#[case(0, "0x1337", "")]
+fn test_message_strict_args_count(
+    #[values(0, 1)] pad: u8,
+    #[case] mode: u8,
+    #[case] msg: &str,
+    #[case] arg: &str,
+    #[values(STRICT_ARGS_COUNT, 0)] flags: u32,
+) {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+
+    // extra args are disallowed when STRICT_ARG_COUNT is set
+    // pad determines whether the extra (unknown) argument is added to the
+    // SEND_MESSAGE or the RECEIVE_MESSAGE condition
+    let extra1 = if pad == 0 { "(1337" } else { "" };
+    let extra2 = if pad == 1 { "(1337" } else { "" };
+    let ret = cond_test_flag(
+        &format!(
+            "((({{h1}} ({{h2}} (123 (((66 ({mode} ({msg} {arg} {extra1} ) ((67 ({mode} ({msg} {extra2} ) ))))"
+        ),
+        flags | ENABLE_SOFTFORK_CONDITION | ENABLE_MESSAGE_CONDITIONS,
+    );
+    if flags == 0 {
+        if let Err(e) = ret {
+            println!("{:?}", e);
+        }
+        assert!(ret.is_ok());
+    } else {
+        assert_eq!(ret.unwrap_err().1, ErrorCode::InvalidCondition);
+    }
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(ASSERT_SECONDS_ABSOLUTE, "104", "", |c: &SpendBundleConditions, _: &Spend| assert_eq!(c.seconds_absolute, 104))]
 #[case(ASSERT_SECONDS_RELATIVE, "101", "", |_: &SpendBundleConditions, s: &Spend| assert_eq!(s.seconds_relative, Some(101)))]
 #[case(ASSERT_HEIGHT_RELATIVE, "101", "", |_: &SpendBundleConditions, s: &Spend| assert_eq!(s.height_relative, Some(101)))]
@@ -1831,15 +2002,15 @@
 
     let expected_flags = if has_agg_sig { 0 } else { ELIGIBLE_FOR_DEDUP };
 
     assert_eq!(conds.cost, expected_cost);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!((spend.flags & ELIGIBLE_FOR_DEDUP), expected_flags);
 
     test(&conds, spend);
 }
 
 #[cfg(test)]
 #[rstest]
@@ -1880,15 +2051,15 @@
     ))
     .unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
 
     test(&conds, spend);
 }
 
 #[cfg(test)]
 #[rstest]
@@ -2024,15 +2195,15 @@
     ))
     .unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 1234));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
 
     test(&conds, spend);
 }
 
 // parse all conditions without an argument. They should all fail
 #[cfg(test)]
@@ -2081,15 +2252,15 @@
     // ASSERT_HEIGHT_RELATIVE
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((82 (0 )))))").unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP | HAS_RELATIVE_CONDITION);
 
     assert_eq!(spend.height_relative, Some(0));
 }
 
 #[test]
 fn test_reserve_fee_exceed_max() {
@@ -2139,32 +2310,32 @@
     // ASSERT_COIN_ANNOUNCEMENT
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((60 ({msg1} ) ((61 ({c11} )))))").unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_cross_coin_announces_consume() {
     // CREATE_COIN_ANNOUNCEMENT
     // ASSERT_COIN_ANNOUNCEMENT
     let (a, conds) =
         cond_test("((({h1} ({h2} (123 (((60 ({msg1} ))) (({h2} ({h2} (123 (((61 ({c11} )))))")
             .unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 2);
     assert_eq!(*conds.spends[0].coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(conds.spends[0].puzzle_hash), H2);
+    assert_eq!(a.atom(conds.spends[0].puzzle_hash).as_ref(), H2);
     assert_eq!(*conds.spends[1].coin_id, test_coin_id(H2, H2, 123));
-    assert_eq!(a.atom(conds.spends[1].puzzle_hash), H2);
+    assert_eq!(a.atom(conds.spends[1].puzzle_hash).as_ref(), H2);
 }
 
 #[test]
 fn test_failing_coin_consume() {
     // ASSERT_COIN_ANNOUNCEMENT
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((61 ({c11} )))))")
@@ -2192,32 +2363,32 @@
     // ASSERT_PUZZLE_ANNOUNCEMENT
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((62 ({msg1} ) ((63 ({p21} )))))").unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_cross_coin_puzzle_announces_consume() {
     // CREATE_PUZZLE_ANNOUNCEMENT
     // ASSERT_PUZZLE_ANNOUNCEMENT
     let (a, conds) =
         cond_test("((({h1} ({h2} (123 (((62 ({msg1} ))) (({h2} ({h2} (123 (((63 ({p21} )))))")
             .unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 2);
     assert_eq!(*conds.spends[0].coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(conds.spends[0].puzzle_hash), H2);
+    assert_eq!(a.atom(conds.spends[0].puzzle_hash).as_ref(), H2);
     assert_eq!(*conds.spends[1].coin_id, test_coin_id(H2, H2, 123));
-    assert_eq!(a.atom(conds.spends[1].puzzle_hash), H2);
+    assert_eq!(a.atom(conds.spends[1].puzzle_hash).as_ref(), H2);
 }
 
 #[test]
 fn test_failing_puzzle_consume() {
     // ASSERT_PUZZLE_ANNOUNCEMENT
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((63 ({p21} )))))")
@@ -2279,15 +2450,15 @@
     // ASSERT_MY_AMOUNT
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((73 (123 ) ((73 (123 ) ))))").unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_multiple_failing_assert_my_amount() {
     // ASSERT_MY_AMOUNT
     assert_eq!(
@@ -2327,15 +2498,15 @@
     let (a, conds) =
         cond_test("((({h1} ({h2} (123 (((70 ({coin12} ) ((70 ({coin12} ) ))))").unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_single_assert_my_coin_id_mismatch() {
     // ASSERT_MY_COIN_ID
     assert_eq!(
@@ -2364,15 +2535,15 @@
     // ASSERT_MY_PARENT_ID
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((71 ({h1} ) ((71 ({h1} ) ))))").unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_single_assert_my_parent_coin_id_mismatch() {
     // ASSERT_MY_PARENT_ID
     assert_eq!(
@@ -2402,15 +2573,15 @@
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_single_assert_my_puzzle_hash_mismatch() {
     // ASSERT_MY_PUZZLEHASH
     assert_eq!(
@@ -2440,15 +2611,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.nil());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
@@ -2463,15 +2634,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 0xffffffffffffffff);
     assert_eq!(conds.addition_amount, 0xffffffffffffffff);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 0xffffffffffffffff));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 0xffffffffffffffff_u64);
         assert_eq!(c.hint, a.nil());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP | ELIGIBLE_FOR_FF);
@@ -2529,20 +2700,20 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert!(c.puzzle_hash.as_ref() == H2);
         assert!(c.amount == 42_u64);
-        assert!(a.atom(c.hint) == H1.to_vec());
+        assert!(a.atom(c.hint).as_ref() == H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_create_coin_extra_arg() {
     // CREATE_COIN
@@ -2552,20 +2723,20 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert!(c.puzzle_hash.as_ref() == H2);
         assert!(c.amount == 42_u64);
-        assert!(a.atom(c.hint) == H1.to_vec());
+        assert!(a.atom(c.hint).as_ref() == H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_create_coin_with_multiple_hints() {
     // CREATE_COIN
@@ -2573,20 +2744,20 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert!(c.puzzle_hash.as_ref() == H2);
         assert!(c.amount == 42_u64);
-        assert!(a.atom(c.hint) == H1.to_vec());
+        assert!(a.atom(c.hint).as_ref() == H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_create_coin_with_hint_as_atom() {
     // CREATE_COIN
@@ -2595,15 +2766,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.nil());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
@@ -2616,15 +2787,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.nil());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
@@ -2649,21 +2820,21 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
 
     for c in &spend.create_coin {
         assert!(c.puzzle_hash.as_ref() == H2);
         assert!(c.amount == 42_u64);
-        assert!(a.atom(c.hint) == MSG1.to_vec());
+        assert!(a.atom(c.hint).as_ref() == MSG1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_create_coin_with_long_hint() {
     // CREATE_COIN
@@ -2671,15 +2842,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
 
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.nil());
     }
@@ -2694,21 +2865,21 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
 
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 42_u64);
-        assert_eq!(a.atom(c.hint), H1.to_vec());
+        assert_eq!(a.atom(c.hint).as_ref(), H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_create_coin_with_cons_hint() {
     // CREATE_COIN
@@ -2717,15 +2888,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
         assert_eq!(c.puzzle_hash.as_ref(), H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.nil());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
@@ -2739,15 +2910,15 @@
 
     assert_eq!(conds.cost, CREATE_COIN_COST * 2);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42 + 43);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.create_coin.len(), 2);
 
     assert!(spend.create_coin.contains(&NewCoin {
         puzzle_hash: H2.into(),
         amount: 42_u64,
         hint: a.nil()
     }));
@@ -2855,21 +3026,21 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
 
     let agg_sigs = agg_sig_vec(condition, spend);
     assert_eq!(agg_sigs.len(), 1);
     for c in agg_sigs {
-        assert_eq!(a.atom(c.0), PUBKEY);
-        assert_eq!(a.atom(c.1), MSG1);
+        assert_eq!(a.atom(c.0).as_ref(), PUBKEY);
+        assert_eq!(a.atom(c.1).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(AGG_SIG_ME)]
@@ -2892,21 +3063,21 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST * 2);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
 
     let agg_sigs = agg_sig_vec(condition, spend);
     assert_eq!(agg_sigs.len(), 2);
     for c in agg_sigs {
-        assert_eq!(a.atom(c.0), PUBKEY);
-        assert_eq!(a.atom(c.1), MSG1);
+        assert_eq!(a.atom(c.0).as_ref(), PUBKEY);
+        assert_eq!(a.atom(c.1).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(AGG_SIG_ME)]
@@ -3009,19 +3180,19 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk), PUBKEY);
-        assert_eq!(a.atom(*msg), MSG1);
+        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_extra_arg() {
     // AGG_SIG_UNSAFE
@@ -3053,15 +3224,15 @@
     )
     .unwrap();
 
     assert_eq!(conds.cost, 1200000);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert!((spend.flags & ELIGIBLE_FOR_DEDUP) == 0);
 
     let agg_sigs = agg_sig_vec(condition, spend);
     assert_eq!(agg_sigs.len(), 1);
 
     // but not in mempool mode
     assert_eq!(
@@ -3102,19 +3273,19 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk), PUBKEY);
-        assert_eq!(a.atom(*msg), MSG1);
+        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_me_extra_arg_allowed() {
     // AGG_SIG_ME
@@ -3127,19 +3298,19 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 1);
     for c in &spend.agg_sig_me {
-        assert_eq!(a.atom(c.0), PUBKEY);
-        assert_eq!(a.atom(c.1), MSG1);
+        assert_eq!(a.atom(c.0).as_ref(), PUBKEY);
+        assert_eq!(a.atom(c.1).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_terminator() {
     // AGG_SIG_UNSAFE
@@ -3149,19 +3320,19 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk), PUBKEY);
-        assert_eq!(a.atom(*msg), MSG1);
+        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_terminator_mempool() {
     // AGG_SIG_UNSAFE
@@ -3186,19 +3357,19 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk), PUBKEY);
-        assert_eq!(a.atom(*msg), MSG1);
+        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_me_invalid_terminator_mempool() {
     // AGG_SIG_ME
@@ -3225,19 +3396,19 @@
 
     assert_eq!(conds.cost, AGG_SIG_COST * 2);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 2);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk), PUBKEY);
-        assert_eq!(a.atom(*msg), MSG1);
+        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_pubkey() {
     // AGG_SIG_UNSAFE
@@ -3357,15 +3528,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
 
     // there is one spend
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_remark_with_arg() {
     // REMARK, but with one unknown argument
@@ -3381,15 +3552,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
 
     // there is one spend
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_concurrent_spend() {
     // ASSERT_CONCURRENT_SPEND
@@ -3429,21 +3600,21 @@
         assert_eq!(conds.removal_amount, 246);
         assert_eq!(conds.addition_amount, 0);
 
         // there are two spends
         assert_eq!(conds.spends.len(), 2);
         let spend = &conds.spends[0];
         assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H2);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 
         let spend = &conds.spends[1];
         assert_eq!(*spend.coin_id, test_coin_id(H2, H2, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H2);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
     }
 }
 
 #[test]
 fn test_concurrent_spend_fail() {
@@ -3508,15 +3679,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
 
     // there are two spends
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_concurrent_puzzle() {
     // ASSERT_CONCURRENT_PUZZLE
@@ -3556,21 +3727,21 @@
         assert_eq!(conds.removal_amount, 246);
         assert_eq!(conds.addition_amount, 0);
 
         // there are two spends
         assert_eq!(conds.spends.len(), 2);
         let spend = &conds.spends[0];
         assert_eq!(*spend.coin_id, test_coin_id(H1, H1, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H1);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 
         let spend = &conds.spends[1];
         assert_eq!(*spend.coin_id, test_coin_id(H2, H2, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H2);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
     }
 }
 
 #[test]
 fn test_concurrent_puzzle_fail() {
@@ -3634,15 +3805,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
 
     // there are two spends
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 // the relative constraints clash because they are on the same coin spend
 #[cfg(test)]
 #[rstest]
@@ -3739,15 +3910,15 @@
         assert_eq!(conds.cost, 0);
         assert_eq!(conds.removal_amount, 123);
         assert_eq!(conds.addition_amount, 0);
 
         assert_eq!(conds.spends.len(), 1);
         let spend = &conds.spends[0];
         assert_eq!(*spend.coin_id, test_coin_id(H1, H1, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H1);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
     }
 }
 
 // the relative constraints do not clash because they are on separate coin
 // spends. We don't know those coins' confirm block height nor timestamps,
@@ -3837,21 +4008,21 @@
         assert_eq!(conds.cost, 0);
         assert_eq!(conds.removal_amount, 246);
         assert_eq!(conds.addition_amount, 0);
 
         assert_eq!(conds.spends.len(), 2);
         let spend = &conds.spends[0];
         assert_eq!(*spend.coin_id, test_coin_id(H1, H1, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H1);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
 
         let spend = &conds.spends[1];
         assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
-        assert_eq!(a.atom(spend.puzzle_hash), H2);
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
         assert_eq!(spend.agg_sig_me.len(), 0);
         assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
     }
 }
 
 #[cfg(test)]
 #[rstest]
@@ -3886,15 +4057,15 @@
     ))
     .unwrap();
 
     assert_eq!(conds.cost, 0);
     assert_eq!(conds.spends.len(), 1);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 1234));
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
 
     test(spend);
 }
 
 #[test]
 fn test_assert_ephemeral() {
@@ -3922,24 +4093,24 @@
     // add 123. the net is a removal of 123
     assert_eq!(conds.removal_amount, 246);
     assert_eq!(conds.addition_amount, 123);
 
     assert_eq!(conds.spends.len(), 2);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H1, 123));
-    assert_eq!(a.atom(spend.puzzle_hash), H1);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 
     let spend = &conds.spends[1];
     assert_eq!(
         *spend.coin_id,
         test_coin_id((&(*conds.spends[0].coin_id)).into(), H2, 123)
     );
-    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
 fn test_assert_ephemeral_wrong_ph() {
     // ASSERT_EPHEMERAL
@@ -4077,24 +4248,24 @@
 
             assert_eq!(conds.reserve_fee, 0);
             assert_eq!(conds.cost, CREATE_COIN_COST);
 
             assert_eq!(conds.spends.len(), 2);
             let spend = &conds.spends[0];
             assert_eq!(*spend.coin_id, test_coin_id(H1, H1, 123));
-            assert_eq!(a.atom(spend.puzzle_hash), H1);
+            assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
             assert_eq!(spend.agg_sig_me.len(), 0);
             assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 
             let spend = &conds.spends[1];
             assert_eq!(
                 *spend.coin_id,
                 test_coin_id((&(*conds.spends[0].coin_id)).into(), H2, 123)
             );
-            assert_eq!(a.atom(spend.puzzle_hash), H2);
+            assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
             assert_eq!(spend.agg_sig_me.len(), 0);
             assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
         }
     }
 }
 
 #[cfg(test)]
@@ -4399,7 +4570,834 @@
     let flags = cond.spends[0].flags;
     if eligible {
         assert!((flags & ELIGIBLE_FOR_FF) != 0);
     } else {
         assert!((flags & ELIGIBLE_FOR_FF) == 0);
     }
 }
+
+// the message condition takes a mode-parameter. This is a 6-bit integer that
+// determines which aspects of the sending spend and receiving spends must
+// match. The second argument is the message. The message and mode must always
+// match between the sender and receiver
+// Additional parameters depend on the mode. If the mode specifies 0
+// committments, there are no additional parameters (however, this is not
+// allowed in mempool mode).
+// The mode integer is a bitfield, the 3 least significant bits indicate
+// properties of the destination spend, the 3 most significant bits indicate
+// properties of the sending spend.
+// 0b100000 = sender parent id
+// 0b010000 = sender puzzle hash
+// 0b001000 = sender amount
+// 0b000100 = receiver parent id
+// 0b000010 = receiver puzzle hash
+// 0b000001 = receiver amount
+
+// 66=SEND_MESSAGE
+// 67=RECEIVE_MESSAGE
+#[cfg(test)]
+enum Ex {
+    Fail,
+    FailMempool,
+    Pass,
+}
+
+#[cfg(test)]
+#[rstest]
+// no committment (not allowed in mempool mode)
+#[case("(66 (0 ({msg1} ) ((67 (0 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0 ({msg2} ) ((67 (0 ({msg1} )", Ex::Fail)]
+#[case("(66 (0 ({msg1} ) ((67 (0 ({msg2} )", Ex::Fail)]
+// only sender coin-ID committment (not allowed in mempool mode)
+#[case("(66 (0x38 ({msg1} ) ((67 (0x38 ({msg1} ({coin12} )", Ex::FailMempool)]
+#[case("(66 (0x38 ({msg1} ) ((67 (0x38 ({msg2} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x38 ({msg2} ) ((67 (0x38 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x38 ({msg1} ) ((67 (0x38 ({msg1} ({coin21} )", Ex::Fail)]
+// only receiver coin-ID committment (not allowed in mempool mode)
+#[case("(66 (0x07 ({msg1} ({coin12} ) ((67 (0x07 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x07 ({msg1} ({coin21} ) ((67 (0x07 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x07 ({msg2} ({coin12} ) ((67 (0x07 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x07 ({msg1} ({coin12} ) ((67 (0x07 ({msg2} )", Ex::Fail)]
+// only sender parent committment (not allowed in mempool mode)
+#[case("(66 (0x20 ({msg1} ) ((67 (0x20 ({msg1} ({h1} )", Ex::FailMempool)]
+#[case("(66 (0x20 ({msg1} ) ((67 (0x20 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x20 ({msg2} ) ((67 (0x20 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x20 ({msg1} ) ((67 (0x20 ({msg2} ({h1} )", Ex::Fail)]
+// only receiver parent committment (not allowed in mempool mode)
+#[case("(66 (0x04 ({msg1} ({h1} ) ((67 (0x04 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x04 ({msg1} ({h2} ) ((67 (0x04 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x04 ({msg2} ({h1} ) ((67 (0x04 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x04 ({msg1} ({h1} ) ((67 (0x04 ({msg2} )", Ex::Fail)]
+// only sender puzzle committment (not allowed in mempool mode)
+#[case("(66 (0x10 ({msg1} ) ((67 (0x10 ({msg1} ({h2} )", Ex::FailMempool)]
+#[case("(66 (0x10 ({msg1} ) ((67 (0x10 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x10 ({msg2} ) ((67 (0x10 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x10 ({msg1} ) ((67 (0x10 ({msg2} ({h2} )", Ex::Fail)]
+// only receiver puzzle committment (not allowed in mempool mode)
+#[case("(66 (0x02 ({msg1} ({h2} ) ((67 (0x02 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x02 ({msg1} ({h1} ) ((67 (0x02 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x02 ({msg2} ({h2} ) ((67 (0x02 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x02 ({msg1} ({h2} ) ((67 (0x02 ({msg2} )", Ex::Fail)]
+// only sender amount committment (not allowed in mempool mode)
+#[case("(66 (0x08 ({msg1} ) ((67 (0x08 ({msg1} (123 )", Ex::FailMempool)]
+#[case("(66 (0x08 ({msg1} ) ((67 (0x08 ({msg1} (124 )", Ex::Fail)]
+#[case("(66 (0x08 ({msg2} ) ((67 (0x08 ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x08 ({msg1} ) ((67 (0x08 ({msg2} (123 )", Ex::Fail)]
+// only receiver amount committment (not allowed in mempool mode)
+#[case("(66 (0x01 ({msg1} (123 ) ((67 (0x01 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x01 ({msg1} (124 ) ((67 (0x01 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x01 ({msg2} (123 ) ((67 (0x01 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x01 ({msg1} (123 ) ((67 (0x01 ({msg2} )", Ex::Fail)]
+// only amount committment (not allowed in mempool mode)
+#[case("(66 (0x09 ({msg1} (123 ) ((67 (0x09 ({msg1} (123 )", Ex::FailMempool)]
+#[case("(66 (0x09 ({msg1} (124 ) ((67 (0x09 ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x09 ({msg1} (123 ) ((67 (0x09 ({msg1} (124 )", Ex::Fail)]
+#[case("(66 (0x09 ({msg2} (123 ) ((67 (0x09 ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x09 ({msg1} (123 ) ((67 (0x09 ({msg2} (123 )", Ex::Fail)]
+// only amount committment on receiver (not allowed in mempool mode)
+#[case(
+    "(66 (0x39 ({msg1} (123 ) ((67 (0x39 ({msg1} ({coin12} )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x39 ({msg1} (124 ) ((67 (0x39 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x39 ({msg1} (123 ) ((67 (0x39 ({msg1} ({coin21} )", Ex::Fail)]
+#[case("(66 (0x39 ({msg2} (123 ) ((67 (0x39 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x39 ({msg1} (123 ) ((67 (0x39 ({msg2} ({coin12} )", Ex::Fail)]
+// only amount committment on sender (not allowed in mempool mode)
+#[case(
+    "(66 (0x0f ({msg1} ({coin12} ) ((67 (0x0f ({msg1} (123 )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x0f ({msg1} ({coin12} ) ((67 (0x0f ({msg1} (124 )", Ex::Fail)]
+#[case("(66 (0x0f ({msg1} ({coin21} ) ((67 (0x0f ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x0f ({msg2} ({coin12} ) ((67 (0x0f ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x0f ({msg1} ({coin12} ) ((67 (0x0f ({msg2} (123 )", Ex::Fail)]
+// sender and receiver coin ID committment (full committment)
+#[case(
+    "(66 (0x3f ({msg1} ({coin12} ) ((67 (0x3f ({msg1} ({coin12} )",
+    Ex::Pass
+)]
+#[case(
+    "(67 (0x3f ({msg1} ({coin12} ) ((66 (0x3f ({msg1} ({coin12} )",
+    Ex::Pass
+)]
+//   wrong coin-id
+#[case(
+    "(66 (0x3f ({msg1} ({coin21} ) ((67 (0x3f ({msg1} ({coin12} )",
+    Ex::Fail
+)]
+#[case(
+    "(66 (0x3f ({msg1} ({coin12} ) ((67 (0x3f ({msg1} ({coin21} )",
+    Ex::Fail
+)]
+//   wrong message
+#[case(
+    "(66 (0x3f ({msg2} ({coin12} ) ((67 (0x3f ({msg1} ({coin12} )",
+    Ex::Fail
+)]
+#[case(
+    "(66 (0x3f ({msg1} ({coin12} ) ((67 (0x3f ({msg2} ({coin12} )",
+    Ex::Fail
+)]
+//    mismatching message
+#[case(
+    "(67 (0x3f ({msg2} ({coin12} ) ((66 (0x3f ({msg1} ({coin12} )",
+    Ex::Fail
+)]
+// sender and receiver puzzle committment
+#[case("(66 (0x12 ({msg1} ({h2} ) ((67 (0x12 ({msg1} ({h2} )", Ex::Pass)]
+#[case("(67 (0x12 ({msg1} ({h2} ) ((66 (0x12 ({msg1} ({h2} )", Ex::Pass)]
+//    wrong messages
+#[case("(66 (0x12 ({msg2} ({h2} ) ((67 (0x12 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x12 ({msg1} ({h2} ) ((67 (0x12 ({msg2} ({h2} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x12 ({msg1} ({h1} ) ((67 (0x12 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x12 ({msg1} ({h2} ) ((67 (0x12 ({msg1} ({h1} )", Ex::Fail)]
+// sender parent and receiver puzzle committment
+#[case("(66 (0x22 ({msg1} ({h2} ) ((67 (0x22 ({msg1} ({h1} )", Ex::Pass)]
+#[case("(67 (0x22 ({msg1} ({h1} ) ((66 (0x22 ({msg1} ({h2} )", Ex::Pass)]
+//    wrong messages
+#[case("(66 (0x22 ({msg2} ({h2} ) ((67 (0x22 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x22 ({msg1} ({h2} ) ((67 (0x22 ({msg2} ({h1} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x22 ({msg1} ({h1} ) ((67 (0x22 ({msg1} ({h1} )", Ex::Fail)]
+//    wrong parent
+#[case("(66 (0x22 ({msg1} ({h2} ) ((67 (0x22 ({msg1} ({h2} )", Ex::Fail)]
+// sender parent and receiver puzzle & amount committment
+#[case("(66 (0x23 ({msg1} ({h2} (123 ) ((67 (0x23 ({msg1} ({h1} )", Ex::Pass)]
+#[case("(67 (0x23 ({msg1} ({h1} ) ((66 (0x23 ({msg1} ({h2} (123 )", Ex::Pass)]
+//    wrong messages
+#[case("(66 (0x23 ({msg2} ({h2} (123 ) ((67 (0x23 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x23 ({msg1} ({h2} (123 ) ((67 (0x23 ({msg2} ({h1} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x23 ({msg1} ({h1} (123 ) ((67 (0x23 ({msg1} ({h1} )", Ex::Fail)]
+//    wrong amount
+#[case("(66 (0x23 ({msg1} ({h2} (122 ) ((67 (0x23 ({msg1} ({h1} )", Ex::Fail)]
+//    wrong parent
+#[case("(66 (0x23 ({msg1} ({h2} (123 ) ((67 (0x23 ({msg1} ({h2} )", Ex::Fail)]
+// sender parent & puzzle and receiver puzzle committment
+#[case("(66 (0x32 ({msg1} ({h2} ) ((67 (0x32 ({msg1} ({h1} ({h2} )", Ex::Pass)]
+#[case("(67 (0x32 ({msg1} ({h1} ({h2} ) ((66 (0x32 ({msg1} ({h2} )", Ex::Pass)]
+//    wrong messages
+#[case("(66 (0x32 ({msg2} ({h2} ) ((67 (0x32 ({msg1} ({h1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x32 ({msg1} ({h2} ) ((67 (0x32 ({msg2} ({h1} ({h2} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x32 ({msg1} ({h1} ) ((67 (0x32 ({msg1} ({h1} ({h2} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x32 ({msg1} ({h2} ) ((67 (0x32 ({msg1} ({h1} ({h1} )", Ex::Fail)]
+//    wrong parent
+#[case("(66 (0x32 ({msg1} ({h2} ) ((67 (0x32 ({msg1} ({h2} ({h2} )", Ex::Fail)]
+// No sender or no recipient of the message
+#[case("(67 (0x12 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x12 ({msg1} ({coin12} )", Ex::Fail)]
+fn test_message_conditions_single_spend(#[case] test_case: &str, #[case] expect: Ex) {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+    for flags in &[
+        ENABLE_MESSAGE_CONDITIONS,
+        ENABLE_MESSAGE_CONDITIONS | NO_UNKNOWN_CONDS,
+    ] {
+        let ret = cond_test_flag(&format!("((({{h1}} ({{h2}} (123 (({test_case}))))"), *flags);
+
+        let mempool = (flags & NO_UNKNOWN_CONDS) != 0;
+        let expect_pass = match expect {
+            Ex::Pass => true,
+            Ex::FailMempool => !mempool,
+            Ex::Fail => false,
+        };
+
+        if let Ok((a, conds)) = ret {
+            assert_eq!(expect_pass, true);
+            assert_eq!(conds.cost, 0);
+            assert_eq!(conds.spends.len(), 1);
+            let spend = &conds.spends[0];
+            assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
+            assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
+            assert_eq!(spend.flags, 0);
+        } else if expect_pass {
+            panic!("failed: {:?}", ret.unwrap_err().1);
+        } else {
+            let actual_err = ret.unwrap_err().1;
+            println!("Error: {actual_err:?}");
+            if mempool {
+                assert!([
+                    ErrorCode::MessageNotSentOrReceived,
+                    ErrorCode::InvalidMessageMode
+                ]
+                .contains(&actual_err));
+            } else {
+                assert_eq!(ErrorCode::MessageNotSentOrReceived, actual_err);
+            }
+        }
+    }
+}
+
+#[cfg(test)]
+#[rstest]
+#[case(512, None)]
+#[case(513, Some(ErrorCode::TooManyAnnouncements))]
+fn test_limit_messages(#[case] count: i32, #[case] expect_err: Option<ErrorCode>) {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+    let r = cond_test_cb(
+        "((({h1} ({h1} (123 ({} )))",
+        ENABLE_MESSAGE_CONDITIONS,
+        Some(Box::new(move |a: &mut Allocator| -> NodePtr {
+            let mut rest: NodePtr = a.nil();
+
+            // generate a lot of announcements
+            // this builds one condition
+            // borrow-rules prevent this from being succint
+            // (66 0x3f {msg1} {coin12})
+            let send = a.nil();
+            let val = a.new_atom(&test_coin_id(H1, H1, 123)).unwrap();
+            let send = a.new_pair(val, send).unwrap();
+            let val = a.new_atom(MSG1).unwrap();
+            let send = a.new_pair(val, send).unwrap();
+            let val = a.new_small_number(0x3f).unwrap();
+            let send = a.new_pair(val, send).unwrap();
+            let val = a.new_small_number(SEND_MESSAGE.into()).unwrap();
+            let send = a.new_pair(val, send).unwrap();
+
+            // (67 0x3f {msg1} {coin12})
+            let recv = a.nil();
+            let val = a.new_atom(&test_coin_id(H1, H1, 123)).unwrap();
+            let recv = a.new_pair(val, recv).unwrap();
+            let val = a.new_atom(MSG1).unwrap();
+            let recv = a.new_pair(val, recv).unwrap();
+            let val = a.new_small_number(0x3f).unwrap();
+            let recv = a.new_pair(val, recv).unwrap();
+            let val = a.new_small_number(RECEIVE_MESSAGE.into()).unwrap();
+            let recv = a.new_pair(val, recv).unwrap();
+
+            for _ in 0..count {
+                // add the condition to the list
+                rest = a.new_pair(send, rest).unwrap();
+                rest = a.new_pair(recv, rest).unwrap();
+            }
+            rest
+        })),
+    );
+
+    if expect_err.is_some() {
+        assert_eq!(r.unwrap_err().1, expect_err.unwrap());
+    } else {
+        r.unwrap();
+    }
+}
+
+#[cfg(test)]
+#[rstest]
+#[case("(66 (0x38 ({longmsg} )", [ErrorCode::InvalidMessage, ErrorCode::InvalidMessageMode])]
+#[case("(66 (0x3c ({long} ({msg1} )", [ErrorCode::InvalidParentId, ErrorCode::InvalidParentId])]
+#[case("(66 (0x3c ({msg2} ({msg1} )", [ErrorCode::InvalidParentId, ErrorCode::InvalidParentId])]
+#[case("(66 (0x3a ({long} ({msg1} )", [ErrorCode::InvalidPuzzleHash, ErrorCode::InvalidPuzzleHash])]
+#[case("(66 (0x3a ({msg2} ({msg1} )", [ErrorCode::InvalidPuzzleHash, ErrorCode::InvalidPuzzleHash])]
+#[case("(66 (0x3f ({long} ({msg1} )", [ErrorCode::InvalidCoinId, ErrorCode::InvalidCoinId])]
+#[case("(66 (0x3f ({msg2} ({msg1} )", [ErrorCode::InvalidCoinId, ErrorCode::InvalidCoinId])]
+#[case(
+    "(66 (0x08 ({msg1} ) ((67 (0x08 ({msg1} (-1 )",
+    [ErrorCode::NegativeAmount, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x08 ({msg1} ) ((67 (0x08 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x01 ({msg1} (-1 ) ((67 (0x01 ({msg1} )",
+    [ErrorCode::NegativeAmount, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x01 ({msg1} ) ((67 (0x01 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x02 ({msg1} ({msg2} ) ((67 (0x02 ({msg1} )",
+    [ErrorCode::InvalidPuzzleHash, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x02 ({msg1} ) ((67 (0x02 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x10 ({msg1} ) ((67 (0x10 ({msg1} ({msg2} )",
+    [ErrorCode::InvalidPuzzleHash, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x10 ({msg1} ) ((67 (0x10 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x04 ({msg1} ({msg2} ) ((67 (0x04 ({msg1} )",
+    [ErrorCode::InvalidParentId, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x04 ({msg1} ) ((67 (0x04 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x20 ({msg1} ) ((67 (0x20 ({msg1} ({msg2} )",
+    [ErrorCode::InvalidParentId, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x20 ({msg1} ) ((67 (0x20 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x07 ({msg1} ({msg2} ) ((67 (0x07 ({msg1} )",
+    [ErrorCode::InvalidCoinId, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x07 ({msg1} ) ((67 (0x07 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x38 ({msg1} ) ((67 (0x38 ({msg1} ({msg2} )",
+    [ErrorCode::InvalidCoinId, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x38 ({msg1} ) ((67 (0x38 ({msg1} )",
+    [ErrorCode::InvalidCondition, ErrorCode::InvalidMessageMode]
+)]
+// message mode must be specified in canonical mode
+#[case(
+    "(66 (0x00 ({msg1} ) ((67 (0x00 ({msg1} )",
+    [ErrorCode::InvalidMessageMode, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x01 ({msg1} (123 ) ((67 (0x00 ({msg1} )",
+    [ErrorCode::InvalidMessageMode, ErrorCode::InvalidMessageMode]
+)]
+// negative messages modes are not allowed
+#[case(
+    "(66 (-1 ({msg1} (123 ) ((67 (0x01 ({msg1} )",
+    [ErrorCode::InvalidMessageMode, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x01 ({msg1} (123 ) ((67 (-1 ({msg1} )",
+    [ErrorCode::InvalidMessageMode, ErrorCode::InvalidMessageMode]
+)]
+// amounts must be specified in canonical mode
+#[case(
+    "(66 (0x01 ({msg1} (0x0040 ) ((67 (0x01 ({msg1} (123 )",
+    [ErrorCode::InvalidCoinAmount, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x01 ({msg1} (0x00 ) ((67 (0x01 ({msg1} (123 )",
+    [ErrorCode::InvalidCoinAmount, ErrorCode::InvalidMessageMode]
+)]
+// coin amounts can't be negative
+#[case(
+    "(66 (0x01 ({msg1} (-1 ) ((67 (0x01 ({msg1} (123 )",
+    [ErrorCode::NegativeAmount, ErrorCode::InvalidMessageMode]
+)]
+#[case(
+    "(66 (0x01 ({msg1} (-1 ) ((67 (0x01 ({msg1} (123 )",
+    [ErrorCode::NegativeAmount, ErrorCode::InvalidMessageMode]
+)]
+fn test_message_conditions_failures(#[case] test_case: &str, #[case] expect: [ErrorCode; 2]) {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+    for i in 0..2 {
+        let ret = cond_test_flag(
+            &format!("((({{h1}} ({{h2}} (123 (({test_case}))))"),
+            ENABLE_MESSAGE_CONDITIONS | (if i == 0 { 0 } else { MEMPOOL_MODE }),
+        );
+
+        let expect = expect[i];
+        let Err(ValidationErr(_, code)) = ret else {
+            panic!("expected failure: {expect:?}");
+        };
+        assert_eq!(code, expect);
+    }
+}
+
+#[cfg(test)]
+#[rstest]
+// no committment (not allowed in mempool mode)
+#[case("(66 (0 ({msg1} )", "(67 (0 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0 ({msg2} )", "(67 (0 ({msg1} )", Ex::Fail)]
+#[case("(66 (0 ({msg1} )", "(67 (0 ({msg2} )", Ex::Fail)]
+// only sender coin-ID committment (not allowed in mempool mode)
+#[case(
+    "(66 (0x38 ({msg1} )",
+    "(67 (0x38 ({msg1} ({coin12} )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x38 ({msg1} )", "(67 (0x38 ({msg2} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x38 ({msg2} )", "(67 (0x38 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x38 ({msg1} )", "(67 (0x38 ({msg1} ({coin21} )", Ex::Fail)]
+// only receiver coin-ID committment (not allowed in mempool mode)
+#[case(
+    "(66 (0x07 ({msg1} ({coin21} )",
+    "(67 (0x07 ({msg1} )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x07 ({msg1} ({coin12} )", "(67 (0x07 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x07 ({msg2} ({coin21} )", "(67 (0x07 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x07 ({msg1} ({coin21} )", "(67 (0x07 ({msg2} )", Ex::Fail)]
+// only sender parent committment (not allowed in mempool mode)
+#[case("(66 (0x20 ({msg1} )", "(67 (0x20 ({msg1} ({h1} )", Ex::FailMempool)]
+#[case("(66 (0x20 ({msg1} )", "(67 (0x20 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x20 ({msg2} )", "(67 (0x20 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x20 ({msg1} )", "(67 (0x20 ({msg2} ({h1} )", Ex::Fail)]
+// only receiver parent committment (not allowed in mempool mode)
+#[case("(66 (0x04 ({msg1} ({h2} )", "(67 (0x04 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x04 ({msg1} ({h1} )", "(67 (0x04 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x04 ({msg2} ({h2} )", "(67 (0x04 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x04 ({msg1} ({h2} )", "(67 (0x04 ({msg2} )", Ex::Fail)]
+// only sender puzzle committment (not allowed in mempool mode)
+#[case("(66 (0x10 ({msg1} )", "(67 (0x10 ({msg1} ({h2} )", Ex::FailMempool)]
+#[case("(66 (0x10 ({msg1} )", "(67 (0x10 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x10 ({msg2} )", "(67 (0x10 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x10 ({msg1} )", "(67 (0x10 ({msg2} ({h2} )", Ex::Fail)]
+// only receiver puzzle committment (not allowed in mempool mode)
+#[case("(66 (0x02 ({msg1} ({h1} )", "(67 (0x02 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x02 ({msg1} ({h2} )", "(67 (0x02 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x02 ({msg2} ({h1} )", "(67 (0x02 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x02 ({msg1} ({h1} )", "(67 (0x02 ({msg2} )", Ex::Fail)]
+// only sender amount committment (not allowed in mempool mode)
+#[case("(66 (0x08 ({msg1} )", "(67 (0x08 ({msg1} (123 )", Ex::FailMempool)]
+#[case("(66 (0x08 ({msg1} )", "(67 (0x08 ({msg1} (124 )", Ex::Fail)]
+#[case("(66 (0x08 ({msg2} )", "(67 (0x08 ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x08 ({msg1} )", "(67 (0x08 ({msg2} (123 )", Ex::Fail)]
+// only receiver amount committment (not allowed in mempool mode)
+#[case("(66 (0x01 ({msg1} (123 )", "(67 (0x01 ({msg1} )", Ex::FailMempool)]
+#[case("(66 (0x01 ({msg1} (124 )", "(67 (0x01 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x01 ({msg2} (123 )", "(67 (0x01 ({msg1} )", Ex::Fail)]
+#[case("(66 (0x01 ({msg1} (123 )", "(67 (0x01 ({msg2} )", Ex::Fail)]
+// only amount committment (not allowed in mempool mode)
+#[case(
+    "(66 (0x09 ({msg1} (123 )",
+    "(67 (0x09 ({msg1} (123 )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x09 ({msg1} (124 )", "(67 (0x09 ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x09 ({msg1} (123 )", "(67 (0x09 ({msg1} (124 )", Ex::Fail)]
+#[case("(66 (0x09 ({msg2} (123 )", "(67 (0x09 ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x09 ({msg1} (123 )", "(67 (0x09 ({msg2} (123 )", Ex::Fail)]
+// only amount committment on receiver (not allowed in mempool mode)
+#[case(
+    "(66 (0x39 ({msg1} (123 )",
+    "(67 (0x39 ({msg1} ({coin12} )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x39 ({msg1} (124 )", "(67 (0x39 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x39 ({msg1} (123 )", "(67 (0x39 ({msg1} ({coin21} )", Ex::Fail)]
+#[case("(66 (0x39 ({msg2} (123 )", "(67 (0x39 ({msg1} ({coin12} )", Ex::Fail)]
+#[case("(66 (0x39 ({msg1} (123 )", "(67 (0x39 ({msg2} ({coin12} )", Ex::Fail)]
+// only amount committment on sender (not allowed in mempool mode)
+#[case(
+    "(66 (0x0f ({msg1} ({coin21} )",
+    "(67 (0x0f ({msg1} (123 )",
+    Ex::FailMempool
+)]
+#[case("(66 (0x0f ({msg1} ({coin21} )", "(67 (0x0f ({msg1} (124 )", Ex::Fail)]
+#[case("(66 (0x0f ({msg1} ({coin12} )", "(67 (0x0f ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x0f ({msg2} ({coin21} )", "(67 (0x0f ({msg1} (123 )", Ex::Fail)]
+#[case("(66 (0x0f ({msg1} ({coin21} )", "(67 (0x0f ({msg2} (123 )", Ex::Fail)]
+// sender and receiver coin ID committment (full committment)
+#[case(
+    "(66 (0x3f ({msg1} ({coin21} )",
+    "(67 (0x3f ({msg1} ({coin12} )",
+    Ex::Pass
+)]
+#[case(
+    "(67 (0x3f ({msg1} ({coin21} )",
+    "(66 (0x3f ({msg1} ({coin12} )",
+    Ex::Pass
+)]
+//   wrong coin-id
+#[case(
+    "(66 (0x3f ({msg1} ({coin12} )",
+    "(67 (0x3f ({msg1} ({coin12} )",
+    Ex::Fail
+)]
+#[case(
+    "(66 (0x3f ({msg1} ({coin21} )",
+    "(67 (0x3f ({msg1} ({coin21} )",
+    Ex::Fail
+)]
+//   wrong message
+#[case(
+    "(66 (0x3f ({msg2} ({coin21} )",
+    "(67 (0x3f ({msg1} ({coin12} )",
+    Ex::Fail
+)]
+#[case(
+    "(66 (0x3f ({msg1} ({coin21} )",
+    "(67 (0x3f ({msg2} ({coin12} )",
+    Ex::Fail
+)]
+//    mismatching message
+#[case(
+    "(67 (0x3f ({msg2} ({coin21} )",
+    "(66 (0x3f ({msg1} ({coin12} )",
+    Ex::Fail
+)]
+// sender and receiver puzzle committment
+#[case("(66 (0x12 ({msg1} ({h1} )", "(67 (0x12 ({msg1} ({h2} )", Ex::Pass)]
+#[case("(67 (0x12 ({msg1} ({h1} )", "(66 (0x12 ({msg1} ({h2} )", Ex::Pass)]
+//    wrong messages
+#[case("(66 (0x12 ({msg2} ({h1} )", "(67 (0x12 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x12 ({msg1} ({h1} )", "(67 (0x12 ({msg2} ({h2} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x12 ({msg1} ({h2} )", "(67 (0x12 ({msg1} ({h2} )", Ex::Fail)]
+#[case("(66 (0x12 ({msg1} ({h1} )", "(67 (0x12 ({msg1} ({h1} )", Ex::Fail)]
+// sender parent and receiver puzzle committment
+#[case("(66 (0x22 ({msg1} ({h1} )", "(67 (0x22 ({msg1} ({h1} )", Ex::Pass)]
+#[case("(67 (0x22 ({msg1} ({h2} )", "(66 (0x22 ({msg1} ({h2} )", Ex::Pass)]
+//    wrong messages
+#[case("(66 (0x22 ({msg2} ({h1} )", "(67 (0x22 ({msg1} ({h1} )", Ex::Fail)]
+#[case("(66 (0x22 ({msg1} ({h1} )", "(67 (0x22 ({msg2} ({h1} )", Ex::Fail)]
+//    wrong puzzle
+#[case("(66 (0x22 ({msg1} ({h2} )", "(67 (0x22 ({msg1} ({h1} )", Ex::Fail)]
+//    wrong parent
+#[case("(66 (0x22 ({msg1} ({h1} )", "(67 (0x22 ({msg1} ({h2} )", Ex::Fail)]
+// sender parent and receiver puzzle & amount committment
+#[case(
+    "(66 (0x23 ({msg1} ({h1} (123 )",
+    "(67 (0x23 ({msg1} ({h1} )",
+    Ex::Pass
+)]
+#[case(
+    "(67 (0x23 ({msg1} ({h2} )",
+    "(66 (0x23 ({msg1} ({h2} (123 )",
+    Ex::Pass
+)]
+//    wrong messages
+#[case(
+    "(66 (0x23 ({msg2} ({h1} (123 )",
+    "(67 (0x23 ({msg1} ({h1} )",
+    Ex::Fail
+)]
+#[case(
+    "(66 (0x23 ({msg1} ({h1} (123 )",
+    "(67 (0x23 ({msg2} ({h1} )",
+    Ex::Fail
+)]
+//    wrong puzzle
+#[case(
+    "(66 (0x23 ({msg1} ({h2} (123 )",
+    "(67 (0x23 ({msg1} ({h1} )",
+    Ex::Fail
+)]
+//    wrong amount
+#[case(
+    "(66 (0x23 ({msg1} ({h1} (122 )",
+    "(67 (0x23 ({msg1} ({h1} )",
+    Ex::Fail
+)]
+//    wrong parent
+#[case(
+    "(66 (0x23 ({msg1} ({h1} (123 )",
+    "(67 (0x23 ({msg1} ({h2} )",
+    Ex::Fail
+)]
+// sender parent & puzzle and receiver puzzle committment
+#[case(
+    "(66 (0x32 ({msg1} ({h1} )",
+    "(67 (0x32 ({msg1} ({h1} ({h2} )",
+    Ex::Pass
+)]
+#[case(
+    "(67 (0x32 ({msg1} ({h2} ({h1} )",
+    "(66 (0x32 ({msg1} ({h2} )",
+    Ex::Pass
+)]
+//    wrong messages
+#[case(
+    "(66 (0x32 ({msg2} ({h1} )",
+    "(67 (0x32 ({msg1} ({h1} ({h2} )",
+    Ex::Fail
+)]
+#[case(
+    "(66 (0x32 ({msg1} ({h1} )",
+    "(67 (0x32 ({msg2} ({h1} ({h2} )",
+    Ex::Fail
+)]
+//    wrong puzzle
+#[case(
+    "(66 (0x32 ({msg1} ({h2} )",
+    "(67 (0x32 ({msg1} ({h1} ({h2} )",
+    Ex::Fail
+)]
+//    wrong puzzle
+#[case(
+    "(66 (0x32 ({msg1} ({h1} )",
+    "(67 (0x32 ({msg1} ({h1} ({h1} )",
+    Ex::Fail
+)]
+//    wrong parent
+#[case(
+    "(66 (0x32 ({msg1} ({h1} )",
+    "(67 (0x32 ({msg1} ({h2} ({h2} )",
+    Ex::Fail
+)]
+fn test_message_conditions_two_spends(
+    #[case] coin1_case: &str,
+    #[case] coin2_case: &str,
+    #[case] expect: Ex,
+) {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+    for flags in &[
+        ENABLE_MESSAGE_CONDITIONS,
+        ENABLE_MESSAGE_CONDITIONS | NO_UNKNOWN_CONDS,
+    ] {
+        let test = format!(
+            "(\
+            (({{h1}} ({{h2}} (123 (\
+                ({coin1_case} \
+                ))\
+            (({{h2}} ({{h1}} (123 (\
+                ({coin2_case} \
+                ))\
+            ))"
+        );
+        let ret = cond_test_flag(&test, *flags);
+
+        let mempool = (flags & NO_UNKNOWN_CONDS) != 0;
+        let expect_pass = match expect {
+            Ex::Pass => true,
+            Ex::FailMempool => !mempool,
+            Ex::Fail => false,
+        };
+
+        if let Ok((a, conds)) = ret {
+            assert_eq!(expect_pass, true);
+            assert_eq!(conds.cost, 0);
+            assert_eq!(conds.spends.len(), 2);
+
+            let spend = &conds.spends[0];
+            assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
+            assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
+            assert_eq!(spend.flags, 0);
+
+            let spend = &conds.spends[1];
+            assert_eq!(*spend.coin_id, test_coin_id(H2, H1, 123));
+            assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
+            assert_eq!(spend.flags, 0);
+        } else if expect_pass {
+            panic!("failed: {:?}", ret.unwrap_err().1);
+        } else {
+            let actual_err = ret.unwrap_err().1;
+            println!("Error: {actual_err:?}");
+            if mempool {
+                assert!([
+                    ErrorCode::MessageNotSentOrReceived,
+                    ErrorCode::InvalidMessageMode
+                ]
+                .contains(&actual_err));
+            } else {
+                assert_eq!(ErrorCode::MessageNotSentOrReceived, actual_err);
+            }
+        }
+    }
+}
+
+// generates all positive test cases between two spends
+#[test]
+fn test_all_message_conditions() {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+    for mode in 0..0b111111 {
+        let coin1_case = match mode & 0b111 {
+            0 => "",
+            0b001 => "(456 ",
+            0b010 => "({h1} ",
+            0b011 => "({h1} (456 ",
+            0b100 => "({h2} ",
+            0b101 => "({h2} (456 ",
+            0b110 => "({h2} ({h1} ",
+            0b111 => "({coin21_456} ",
+            _ => {
+                panic!("unexpected {mode}");
+            }
+        };
+
+        let coin2_case = match mode >> 3 {
+            0 => "",
+            0b001 => "(123 ",
+            0b010 => "({h2} ",
+            0b011 => "({h2} (123 ",
+            0b100 => "({h1} ",
+            0b101 => "({h1} (123 ",
+            0b110 => "({h1} ({h2} ",
+            0b111 => "({coin12} ",
+            _ => {
+                panic!("unexpected {mode}");
+            }
+        };
+
+        let test = format!(
+            "(\
+        (({{h1}} ({{h2}} (123 (\
+            ((66 ({mode} ({{msg2}} {coin1_case} )\
+            ))\
+        (({{h2}} ({{h1}} (456 (\
+            ((67 ({mode} ({{msg2}} {coin2_case} )\
+            ))\
+        ))"
+        );
+        let (a, conds) =
+            cond_test_flag(&test, ENABLE_MESSAGE_CONDITIONS).expect("condition expected to pass");
+
+        assert_eq!(conds.cost, 0);
+        assert_eq!(conds.spends.len(), 2);
+
+        let spend = &conds.spends[0];
+        assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
+        assert_eq!(spend.flags, 0);
+
+        let spend = &conds.spends[1];
+        assert_eq!(*spend.coin_id, test_coin_id(H2, H1, 456));
+        assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H1);
+        assert_eq!(spend.flags, 0);
+    }
+}
+
+#[test]
+fn test_message_eligible_for_ff() {
+    use crate::gen::flags::ENABLE_MESSAGE_CONDITIONS;
+
+    for mode in 0..0b111111 {
+        let coin1_case = match mode & 0b111 {
+            0 => "",
+            0b001 => "(123 ",
+            0b010 => "({h1} ",
+            0b011 => "({h1} (123 ",
+            0b100 => "({h2} ",
+            0b101 => "({h2} (123 ",
+            0b110 => "({h2} ({h1} ",
+            0b111 => "({coin21} ",
+            _ => {
+                panic!("unexpected {mode}");
+            }
+        };
+
+        let coin2_case = match mode >> 3 {
+            0 => "",
+            0b001 => "(123 ",
+            0b010 => "({h2} ",
+            0b011 => "({h2} (123 ",
+            0b100 => "({h1} ",
+            0b101 => "({h1} (123 ",
+            0b110 => "({h1} ({h2} ",
+            0b111 => "({coin12} ",
+            _ => {
+                panic!("unexpected {mode}");
+            }
+        };
+
+        // this is a model example of a spend that's eligible for FF
+        // it mimics the output of singleton_top_layer_v1_1
+        // The first test is where the sender is the spend that may be
+        // fast-forwarded
+        // 73=ASSERT_MY_AMOUNT
+        // 71=ASSERT_MY_PARENT_ID
+        // 51=CREATE_COIN
+        // 66=SEND_MESSAGE
+        // 67=RECEIVE_MESSAGE
+        let test = format!(
+            "(\
+       (({{h1}} ({{h2}} (123 (\
+           ((73 (123 ) \
+           ((71 ({{h1}} ) \
+           ((51 ({{h2}} (123 ) \
+           ((66 ({mode} ({{msg2}} {coin1_case} )\
+           ))\
+       (({{h2}} ({{h1}} (123 (\
+           ((67 ({mode} ({{msg2}} {coin2_case} )\
+           ))\
+       ))"
+        );
+
+        let (_a, cond) = cond_test_flag(&test, ENABLE_MESSAGE_CONDITIONS).expect("cond_test");
+        assert!(cond.spends.len() == 2);
+        assert_eq!(
+            (cond.spends[0].flags & ELIGIBLE_FOR_FF) != 0,
+            (mode & 0b100000) == 0
+        );
+        assert_eq!((cond.spends[1].flags & ELIGIBLE_FOR_FF), 0);
+
+        // flip sender and receiver. The receiving spend is the one eligible for
+        // fast-forwarding
+        let test = format!(
+            "(\
+       (({{h2}} ({{h1}} (123 (\
+           ((73 (123 ) \
+           ((71 ({{h2}} ) \
+           ((51 ({{h1}} (123 ) \
+           ((67 ({mode} ({{msg2}} {coin2_case} )\
+           ))\
+       (({{h1}} ({{h2}} (123 (\
+           ((66 ({mode} ({{msg2}} {coin1_case} )\
+           ))\
+       ))"
+        );
+
+        let (_a, cond) = cond_test_flag(&test, ENABLE_MESSAGE_CONDITIONS).expect("cond_test");
+        assert!(cond.spends.len() == 2);
+        assert_eq!(
+            (cond.spends[0].flags & ELIGIBLE_FOR_FF) != 0,
+            (mode & 0b100) == 0
+        );
+        assert_eq!((cond.spends[1].flags & ELIGIBLE_FOR_FF), 0);
+    }
+}
```

### Comparing `chik_rs-0.5.2/src/gen/flags.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/flags.rs`

 * *Files 10% similar despite different names*

```diff
@@ -29,13 +29,16 @@
 // contain back-references
 pub const ALLOW_BACKREFS: u32 = 0x2000000;
 
 // When set, the "flags" field of the Spend objects will be set depending on
 // what features are detected of the spends
 pub const ANALYZE_SPENDS: u32 = 0x4000000;
 
+// This enables support for the new SEND_MESSAGE and RECEIVE_MESSAGE conditions
+pub const ENABLE_MESSAGE_CONDITIONS: u32 = 0x8000000;
+
 pub const MEMPOOL_MODE: u32 = KLVM_MEMPOOL_MODE
     | NO_UNKNOWN_CONDS
     | COND_ARGS_NIL
     | STRICT_ARGS_COUNT
     | NO_RELATIVE_CONDITIONS_ON_EPHEMERAL
     | ANALYZE_SPENDS;
```

### Comparing `chik_rs-0.5.2/src/gen/get_puzzle_and_solution.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 use crate::gen::validation_error::{atom, check_nil, first, next, rest, ErrorCode, ValidationErr};
 use ::chik_protocol::bytes::Bytes32;
 use klvm_utils::tree_hash;
-use klvmr::allocator::{Allocator, NodePtr};
+use klvmr::allocator::{Allocator, Atom, NodePtr};
 use klvmr::op_utils::u64_from_bytes;
-use std::convert::AsRef;
 
 // returns parent-coin ID, amount, puzzle-reveal and solution
 pub fn parse_coin_spend(
     a: &Allocator,
     coin_spend: NodePtr,
-) -> Result<(&[u8], u64, NodePtr, NodePtr), ValidationErr> {
+) -> Result<(Atom, u64, NodePtr, NodePtr), ValidationErr> {
     let parent = atom(a, first(a, coin_spend)?, ErrorCode::InvalidParentId)?;
     let coin_spend = rest(a, coin_spend)?;
     let puzzle = first(a, coin_spend)?;
     let coin_spend = rest(a, coin_spend)?;
-    let amount = u64_from_bytes(atom(
-        a,
-        first(a, coin_spend)?,
-        ErrorCode::InvalidCoinAmount,
-    )?);
+    let amount =
+        u64_from_bytes(atom(a, first(a, coin_spend)?, ErrorCode::InvalidCoinAmount)?.as_ref());
     let coin_spend = rest(a, coin_spend)?;
     let solution = first(a, coin_spend)?;
     check_nil(a, rest(a, coin_spend)?)?;
     Ok((parent, amount, puzzle, solution))
 }
 
 pub fn get_puzzle_and_solution_for_coin(
@@ -41,15 +37,15 @@
     while let Some((coin_spend, next)) = next(a, iter)? {
         iter = next;
         // coin_spend is (parent puzzle amount solution)
         let (parent, amount, puzzle, solution) = parse_coin_spend(a, coin_spend)?;
 
         // we want to avoid having to compute the puzzle hash if we don't have to
         // so check parent and amount first
-        if parent != find_parent.as_ref() || amount != find_amount {
+        if parent.as_ref() != find_parent.as_ref() || amount != find_amount {
             continue;
         }
 
         let puzzle_hash = tree_hash(a, puzzle);
         if puzzle_hash != find_ph.as_ref() {
             continue;
         }
@@ -192,15 +188,15 @@
     let puzzle2 = make_dummy_puzzle(&mut a, 4);
     let solution1 = make_dummy_puzzle(&mut a, 2);
     let amount_atom = a.new_atom(&u64_to_bytes(1337)).unwrap();
 
     let spend1 = make_coin_spend(&mut a, parent, 1337, puzzle1, solution1);
     assert_eq!(
         parse_coin_spend(&a, spend1).unwrap(),
-        (parent.as_ref(), 1337, puzzle1, solution1)
+        (Atom::Borrowed(&parent), 1337, puzzle1, solution1)
     );
 
     // this is a spend where the parent is not an atom
     let spend2 = make_invalid_coin_spend(&mut a, puzzle2, amount_atom, puzzle1, solution1);
     assert_eq!(
         parse_coin_spend(&a, spend2).unwrap_err().1,
         ErrorCode::InvalidParentId
```

### Comparing `chik_rs-0.5.2/src/gen/opcodes.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/opcodes.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::gen::flags::ENABLE_SOFTFORK_CONDITION;
+use crate::gen::flags::{ENABLE_MESSAGE_CONDITIONS, ENABLE_SOFTFORK_CONDITION};
 use klvmr::allocator::{Allocator, NodePtr, SExp};
 use klvmr::cost::Cost;
 
 pub type ConditionOpcode = u16;
 
 // AGG_SIG is ascii "1"
 pub const AGG_SIG_PARENT: ConditionOpcode = 43;
@@ -23,14 +23,17 @@
 pub const CREATE_COIN_ANNOUNCEMENT: ConditionOpcode = 60;
 pub const ASSERT_COIN_ANNOUNCEMENT: ConditionOpcode = 61;
 pub const CREATE_PUZZLE_ANNOUNCEMENT: ConditionOpcode = 62;
 pub const ASSERT_PUZZLE_ANNOUNCEMENT: ConditionOpcode = 63;
 pub const ASSERT_CONCURRENT_SPEND: ConditionOpcode = 64;
 pub const ASSERT_CONCURRENT_PUZZLE: ConditionOpcode = 65;
 
+pub const SEND_MESSAGE: ConditionOpcode = 66;
+pub const RECEIVE_MESSAGE: ConditionOpcode = 67;
+
 // the conditions below let coins inquire about themselves
 pub const ASSERT_MY_COIN_ID: ConditionOpcode = 70;
 pub const ASSERT_MY_PARENT_ID: ConditionOpcode = 71;
 pub const ASSERT_MY_PUZZLEHASH: ConditionOpcode = 72;
 pub const ASSERT_MY_AMOUNT: ConditionOpcode = 73;
 pub const ASSERT_MY_BIRTH_SECONDS: ConditionOpcode = 74;
 pub const ASSERT_MY_BIRTH_HEIGHT: ConditionOpcode = 75;
@@ -106,14 +109,15 @@
 }
 
 pub fn parse_opcode(a: &Allocator, op: NodePtr, flags: u32) -> Option<ConditionOpcode> {
     let buf = match a.sexp(op) {
         SExp::Atom => a.atom(op),
         _ => return None,
     };
+    let buf = buf.as_ref();
     if buf.len() == 2 && (flags & ENABLE_SOFTFORK_CONDITION) != 0 {
         if buf[0] == 0 {
             // no redundant leading zeroes
             None
         } else {
             // These are 2-byte condition codes whose first byte is 1
             Some(ConditionOpcode::from_be_bytes(buf.try_into().unwrap()))
@@ -144,25 +148,27 @@
             | ASSERT_BEFORE_HEIGHT_ABSOLUTE
             | ASSERT_CONCURRENT_SPEND
             | ASSERT_CONCURRENT_PUZZLE
             | ASSERT_MY_BIRTH_SECONDS
             | ASSERT_MY_BIRTH_HEIGHT
             | ASSERT_EPHEMERAL => Some(b0),
             _ => {
-                if (flags & ENABLE_SOFTFORK_CONDITION) != 0
+                if ((flags & ENABLE_SOFTFORK_CONDITION) != 0
                     && [
                         SOFTFORK,
                         AGG_SIG_PARENT,
                         AGG_SIG_PUZZLE,
                         AGG_SIG_AMOUNT,
                         AGG_SIG_PUZZLE_AMOUNT,
                         AGG_SIG_PARENT_AMOUNT,
                         AGG_SIG_PARENT_PUZZLE,
                     ]
-                    .contains(&b0)
+                    .contains(&b0))
+                    || ((flags & ENABLE_MESSAGE_CONDITIONS) != 0
+                        && [SEND_MESSAGE, RECEIVE_MESSAGE].contains(&b0))
                 {
                     Some(b0)
                 } else {
                     None
                 }
             }
         }
@@ -213,15 +219,19 @@
 #[case(&[ASSERT_BEFORE_HEIGHT_RELATIVE as u8], Some(ASSERT_BEFORE_HEIGHT_RELATIVE))]
 #[case(&[ASSERT_BEFORE_HEIGHT_ABSOLUTE as u8], Some(ASSERT_BEFORE_HEIGHT_ABSOLUTE))]
 #[case(&[REMARK as u8], Some(REMARK))]
 fn test_parse_opcode(#[case] input: &[u8], #[case] expected: Option<ConditionOpcode>) {
     let mut a = Allocator::new();
     assert_eq!(opcode_tester(&mut a, input, 0), expected);
     assert_eq!(
-        opcode_tester(&mut a, input, ENABLE_SOFTFORK_CONDITION),
+        opcode_tester(
+            &mut a,
+            input,
+            ENABLE_SOFTFORK_CONDITION | ENABLE_MESSAGE_CONDITIONS
+        ),
         expected
     );
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(&[AGG_SIG_UNSAFE as u8], Some(AGG_SIG_UNSAFE), Some(AGG_SIG_UNSAFE))]
@@ -233,27 +243,59 @@
 #[case(&[AGG_SIG_PUZZLE as u8], None, Some(AGG_SIG_PUZZLE))]
 #[case(&[AGG_SIG_AMOUNT as u8], None, Some(AGG_SIG_AMOUNT))]
 #[case(&[AGG_SIG_PUZZLE_AMOUNT as u8], None, Some(AGG_SIG_PUZZLE_AMOUNT))]
 #[case(&[AGG_SIG_PARENT_AMOUNT as u8], None, Some(AGG_SIG_PARENT_AMOUNT))]
 #[case(&[AGG_SIG_PARENT_PUZZLE as u8], None, Some(AGG_SIG_PARENT_PUZZLE))]
 #[case(&[ASSERT_EPHEMERAL as u8], Some(ASSERT_EPHEMERAL), Some(ASSERT_EPHEMERAL))]
 #[case(&[ASSERT_BEFORE_SECONDS_RELATIVE as u8], Some(ASSERT_BEFORE_SECONDS_RELATIVE), Some(ASSERT_BEFORE_SECONDS_RELATIVE))]
+#[case(&[SEND_MESSAGE as u8], None, None)]
+#[case(&[RECEIVE_MESSAGE as u8], None, None)]
 fn test_parse_opcode_softfork(
     #[case] input: &[u8],
     #[case] expected: Option<ConditionOpcode>,
     #[case] expected2: Option<ConditionOpcode>,
 ) {
     let mut a = Allocator::new();
     assert_eq!(opcode_tester(&mut a, input, 0), expected);
     assert_eq!(
         opcode_tester(&mut a, input, ENABLE_SOFTFORK_CONDITION),
         expected2
     );
 }
 
+#[cfg(test)]
+#[rstest]
+#[case(&[AGG_SIG_UNSAFE as u8], Some(AGG_SIG_UNSAFE), Some(AGG_SIG_UNSAFE))]
+#[case(&[AGG_SIG_ME as u8], Some(AGG_SIG_ME), Some(AGG_SIG_ME))]
+#[case(&[CREATE_COIN as u8], Some(CREATE_COIN), Some(CREATE_COIN))]
+// the SOFTOFORK and new AGG_SIG_* condition is only recognized when the flag is set
+#[case(&[SOFTFORK as u8], None, None)]
+#[case(&[AGG_SIG_PARENT as u8], None, None)]
+#[case(&[AGG_SIG_PUZZLE as u8], None, None)]
+#[case(&[AGG_SIG_AMOUNT as u8], None, None)]
+#[case(&[AGG_SIG_PUZZLE_AMOUNT as u8], None, None)]
+#[case(&[AGG_SIG_PARENT_AMOUNT as u8], None, None)]
+#[case(&[AGG_SIG_PARENT_PUZZLE as u8], None, None)]
+#[case(&[ASSERT_EPHEMERAL as u8], Some(ASSERT_EPHEMERAL), Some(ASSERT_EPHEMERAL))]
+#[case(&[ASSERT_BEFORE_SECONDS_RELATIVE as u8], Some(ASSERT_BEFORE_SECONDS_RELATIVE), Some(ASSERT_BEFORE_SECONDS_RELATIVE))]
+#[case(&[SEND_MESSAGE as u8], None, Some(SEND_MESSAGE))]
+#[case(&[RECEIVE_MESSAGE as u8], None, Some(RECEIVE_MESSAGE))]
+fn test_parse_opcode_message(
+    #[case] input: &[u8],
+    #[case] expected: Option<ConditionOpcode>,
+    #[case] expected2: Option<ConditionOpcode>,
+) {
+    let mut a = Allocator::new();
+    assert_eq!(opcode_tester(&mut a, input, 0), expected);
+    assert_eq!(
+        opcode_tester(&mut a, input, ENABLE_MESSAGE_CONDITIONS),
+        expected2
+    );
+}
+
 #[test]
 fn test_parse_invalid_opcode() {
     // a pair is never a valid condition
     let mut a = Allocator::new();
     let v1 = a.new_atom(&[0]).unwrap();
     let v2 = a.new_atom(&[0]).unwrap();
     let p = a.new_pair(v1, v2).unwrap();
```

### Comparing `chik_rs-0.5.2/src/gen/run_block_generator.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/run_block_generator.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 use crate::gen::conditions::{
     parse_spends, process_single_spend, validate_conditions, ParseState, SpendBundleConditions,
 };
 use crate::gen::flags::ALLOW_BACKREFS;
 use crate::gen::spend_visitor::SpendVisitor;
 use crate::gen::validation_error::{first, ErrorCode, ValidationErr};
 use crate::generator_rom::{COST_PER_BYTE, GENERATOR_ROM, KLVM_DESERIALIZER};
-use klvm_utils::tree_hash;
+use klvm_utils::tree_hash_cached;
 use klvmr::allocator::{Allocator, NodePtr};
 use klvmr::chik_dialect::ChikDialect;
 use klvmr::cost::Cost;
 use klvmr::reduction::Reduction;
 use klvmr::run_program::run_program;
-use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
+use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs, node_from_bytes_backrefs_record};
+use std::collections::{HashMap, HashSet};
 
 fn subtract_cost(a: &Allocator, cost_left: &mut Cost, subtract: Cost) -> Result<(), ValidationErr> {
     if subtract > *cost_left {
         Err(ValidationErr(a.nil(), ErrorCode::CostExceeded))
     } else {
         *cost_left -= subtract;
         Ok(())
@@ -118,18 +119,18 @@
 ) -> Result<SpendBundleConditions, ValidationErr> {
     let byte_cost = program.len() as u64 * COST_PER_BYTE;
 
     let mut cost_left = max_cost;
     subtract_cost(a, &mut cost_left, byte_cost)?;
 
     let klvm_deserializer = node_from_bytes(a, &KLVM_DESERIALIZER)?;
-    let program = if (flags & ALLOW_BACKREFS) != 0 {
-        node_from_bytes_backrefs(a, program)?
+    let (program, backrefs) = if (flags & ALLOW_BACKREFS) != 0 {
+        node_from_bytes_backrefs_record(a, program)?
     } else {
-        node_from_bytes(a, program)?
+        (node_from_bytes(a, program)?, HashSet::<NodePtr>::new())
     };
 
     // iterate in reverse order since we're building a linked list from
     // the tail
     let mut blocks = a.nil();
     for g in block_refs.iter().rev() {
         let ref_gen = a.new_atom(g.as_ref())?;
@@ -150,27 +151,28 @@
 
     // at this point all_spends is a list of:
     // (parent-coin-id puzzle-reveal amount solution . extra)
     // where extra may be nil, or additional extension data
 
     let mut ret = SpendBundleConditions::default();
     let mut state = ParseState::default();
+    let mut cache = HashMap::<NodePtr, [u8; 32]>::new();
 
     while let Some((spend, rest)) = a.next(all_spends) {
         all_spends = rest;
         // process the spend
         let [parent_id, puzzle, amount, solution, _spend_level_extra] =
             extract_n::<5>(a, spend, ErrorCode::InvalidCondition)?;
 
         let Reduction(klvm_cost, conditions) =
             run_program(a, &dialect, puzzle, solution, cost_left)?;
 
         subtract_cost(a, &mut cost_left, klvm_cost)?;
 
-        let buf = tree_hash(a, puzzle);
+        let buf = tree_hash_cached(a, puzzle, &backrefs, &mut cache);
         let puzzle_hash = a.new_atom(&buf)?;
 
         process_single_spend::<V>(
             a,
             &mut ret,
             &mut state,
             parent_id,
```

### Comparing `chik_rs-0.5.2/src/gen/run_puzzle.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/run_puzzle.rs`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     let puzzle_hash = tree_hash(a, puzzle);
     let coin_id = Arc::<Bytes32>::new(
         Coin {
             parent_coin_info: parent_id.try_into().unwrap(),
             puzzle_hash: puzzle_hash.into(),
             amount,
         }
-        .coin_id()
-        .into(),
+        .coin_id(),
     );
 
     let mut spend = Spend::new(
         a.new_atom(parent_id)?,
         amount,
         a.new_atom(&puzzle_hash)?,
         coin_id,
```

### Comparing `chik_rs-0.5.2/src/gen/sanitize_int.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/sanitize_int.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     n: NodePtr,
     max_size: usize,
     code: ErrorCode,
 ) -> Result<SanitizedUint, ValidationErr> {
     assert!(max_size <= 8);
 
     let buf = atom(a, n, code)?;
+    let buf = buf.as_ref();
 
     if buf.is_empty() {
         return Ok(SanitizedUint::Ok(0));
     }
 
     // if the top bit is set, it's a negative number
     if (buf[0] & 0x80) != 0 {
```

### Comparing `chik_rs-0.5.2/src/gen/test_generators.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/test_generators.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 use super::conditions::{MempoolVisitor, NewCoin, Spend, SpendBundleConditions};
 use super::run_block_generator::{run_block_generator, run_block_generator2};
 use crate::allocator::make_allocator;
-use crate::gen::flags::{ALLOW_BACKREFS, MEMPOOL_MODE};
+use crate::gen::flags::{ALLOW_BACKREFS, ENABLE_MESSAGE_CONDITIONS, MEMPOOL_MODE};
 use chik_protocol::{Bytes, Bytes48};
 use klvmr::allocator::NodePtr;
 use klvmr::Allocator;
 use std::iter::zip;
-use std::string::String;
 use text_diff::diff;
 use text_diff::Difference;
 
 use rstest::rstest;
 
 fn print_conditions(a: &Allocator, c: &SpendBundleConditions) -> String {
     let mut ret = String::new();
@@ -28,15 +27,18 @@
         ret += &format!("ASSERT_BEFORE_SECONDS_ABSOLUTE {val}\n");
     }
     if let Some(val) = c.before_height_absolute {
         ret += &format!("ASSERT_BEFORE_HEIGHT_ABSOLUTE {val}\n");
     }
     let mut agg_sigs = Vec::<(Bytes48, Bytes)>::new();
     for (pk, msg) in &c.agg_sig_unsafe {
-        agg_sigs.push((a.atom(*pk).try_into().unwrap(), a.atom(*msg).into()));
+        agg_sigs.push((
+            a.atom(*pk).as_ref().try_into().unwrap(),
+            a.atom(*msg).as_ref().into(),
+        ));
     }
     agg_sigs.sort();
     for (pk, msg) in agg_sigs {
         ret += &format!(
             "AGG_SIG_UNSAFE pk: {} msg: {}\n",
             hex::encode(pk),
             hex::encode(msg)
@@ -82,15 +84,18 @@
                     cc.amount
                 );
             }
         }
 
         let mut agg_sigs = Vec::<(Bytes48, Bytes)>::new();
         for (pk, msg) in s.agg_sig_me {
-            agg_sigs.push((a.atom(pk).try_into().unwrap(), a.atom(msg).into()));
+            agg_sigs.push((
+                a.atom(pk).as_ref().try_into().unwrap(),
+                a.atom(msg).as_ref().into(),
+            ));
         }
         agg_sigs.sort();
         for (pk, msg) in agg_sigs {
             ret += &format!(
                 "  AGG_SIG_ME pk: {} msg: {}\n",
                 hex::encode(pk),
                 hex::encode(msg)
@@ -187,37 +192,44 @@
 #[case("many-large-ints-negative")]
 #[case("many-large-ints")]
 #[case("max-height")]
 #[case("multiple-reserve-fee")]
 #[case("negative-reserve-fee")]
 #[case("recursion-pairs")]
 #[case("unknown-condition")]
+#[case("duplicate-messages")]
 fn run_generator(#[case] name: &str) {
     use std::fs::read_to_string;
 
-    let filename = format!("generator-tests/{name}.txt");
+    let filename = format!("../../generator-tests/{name}.txt");
     println!("file: {filename}");
     let test_file = read_to_string(filename).expect("test file not found");
     let (generator, expected) = test_file.split_once('\n').expect("invalid test file");
     let generator = hex::decode(generator).expect("invalid hex encoded generator");
 
     let expected = match expected.split_once("STRICT:\n") {
         Some((c, m)) => [c, m],
         None => [expected, expected],
     };
 
     let mut block_refs = Vec::<Vec<u8>>::new();
 
-    let filename = format!("generator-tests/{name}.env");
+    let filename = format!("../../generator-tests/{name}.env");
     if let Ok(env_hex) = std::fs::read_to_string(&filename) {
         println!("block-ref file: {filename}");
         block_refs.push(hex::decode(env_hex).expect("hex decode env-file"));
     }
 
-    for (flags, expected) in zip(&[ALLOW_BACKREFS, ALLOW_BACKREFS | MEMPOOL_MODE], expected) {
+    for (flags, expected) in zip(
+        &[
+            ALLOW_BACKREFS | ENABLE_MESSAGE_CONDITIONS,
+            ALLOW_BACKREFS | MEMPOOL_MODE | ENABLE_MESSAGE_CONDITIONS,
+        ],
+        expected,
+    ) {
         println!("flags: {:x}", flags);
         let mut a = make_allocator(*flags);
         let conds = run_block_generator::<_, MempoolVisitor>(
             &mut a,
             &generator,
             &block_refs,
             11000000000,
```

### Comparing `chik_rs-0.5.2/src/gen/validation_error.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/gen/validation_error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use klvmr::allocator::{Allocator, NodePtr, SExp};
+use klvmr::allocator::{Allocator, Atom, NodePtr, SExp};
 use klvmr::reduction::EvalErr;
 use thiserror::Error;
 
 #[cfg(feature = "py-bindings")]
 use pyo3::PyErr;
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
@@ -47,14 +47,17 @@
     ImpossibleHeightRelativeConstraints,
     ImpossibleHeightAbsoluteConstraints,
     AssertEphemeralFailed,
     EphemeralRelativeCondition,
     InvalidSoftforkCondition,
     InvalidSoftforkCost,
     TooManyAnnouncements,
+    InvalidMessageMode,
+    InvalidCoinId,
+    MessageNotSentOrReceived,
 }
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, Error)]
 #[error("validation error: {1:?}")]
 pub struct ValidationErr(pub NodePtr, pub ErrorCode);
 
 impl From<EvalErr> for ValidationErr {
@@ -132,14 +135,17 @@
             ErrorCode::AssertMyBirthSecondsFailed => 138,
             ErrorCode::AssertMyBirthHeightFailed => 139,
             ErrorCode::AssertEphemeralFailed => 140,
             ErrorCode::EphemeralRelativeCondition => 141,
             ErrorCode::InvalidSoftforkCondition => 142,
             ErrorCode::InvalidSoftforkCost => 143,
             ErrorCode::TooManyAnnouncements => 144,
+            ErrorCode::InvalidMessageMode => 145,
+            ErrorCode::InvalidCoinId => 146,
+            ErrorCode::MessageNotSentOrReceived => 147,
         }
     }
 }
 
 pub fn rest(a: &Allocator, n: NodePtr) -> Result<NodePtr, ValidationErr> {
     match a.sexp(n) {
         SExp::Pair(_, right) => Ok(right),
@@ -157,21 +163,21 @@
             } else {
                 Err(ValidationErr(n, ErrorCode::InvalidCondition))
             }
         }
     }
 }
 
-pub fn atom(a: &Allocator, n: NodePtr, code: ErrorCode) -> Result<&[u8], ValidationErr> {
+pub fn atom(a: &Allocator, n: NodePtr, code: ErrorCode) -> Result<Atom, ValidationErr> {
     match a.sexp(n) {
         SExp::Atom => Ok(a.atom(n)),
         _ => Err(ValidationErr(n, code)),
     }
 }
 
 pub fn check_nil(a: &Allocator, n: NodePtr) -> Result<(), ValidationErr> {
-    if atom(a, n, ErrorCode::InvalidCondition)?.is_empty() {
+    if atom(a, n, ErrorCode::InvalidCondition)?.as_ref().is_empty() {
         Ok(())
     } else {
         Err(ValidationErr(n, ErrorCode::InvalidCondition))
     }
 }
```

### Comparing `chik_rs-0.5.2/src/generator_rom.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/generator_rom.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/src/merkle_set.rs` & `chik_rs-0.6.0/crates/chik-consensus/src/merkle_set.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/Cargo.toml` & `chik_rs-0.6.0/crates/chik-bls/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "chik-bls"
-version = "0.5.1"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "BLS signature, verification and aggregation funcions for the Chik blockchain"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
-homepage = "https://github.com/Chik-Network/chik_rs/chik-bls/"
-repository = "https://github.com/Chik-Network/chik_rs/chik-bls/"
+homepage = "https://github.com/Chik-Network/chik_rs"
+repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "chik_py_streamable_macro", "chik-traits/py-bindings"]
 
 [dependencies]
-chik-traits = { version = "0.5.1", path = "../chik-traits" }
-chik_py_streamable_macro = { version = "0.5.1", path = "../chik_py_streamable_macro", optional = true }
+chik-traits = { version = "0.6.0", path = "../chik-traits" }
+chik_py_streamable_macro = { version = "0.6.0", path = "../chik_py_streamable_macro", optional = true }
 tiny-bip39 = "1.0.0"
 anyhow = "1.0.71"
 sha2 = "0.10.8"
 hkdf = "0.12.0"
 blst = { version = "0.3.11", git = "https://github.com/supranational/blst.git", rev = "0d46eefa45fc1e57aceb42bba0e84eab3a7a9725", features = ["portable"] }
 hex = "0.4.3"
 thiserror = "1.0.44"
```

### Comparing `chik_rs-0.5.2/chik-bls/README.md` & `chik_rs-0.6.0/crates/chik-bls/README.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/benches/derive_key.rs` & `chik_rs-0.6.0/crates/chik-bls/benches/derive_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/benches/parse.rs` & `chik_rs-0.6.0/crates/chik-bls/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/benches/sign.rs` & `chik_rs-0.6.0/crates/chik-bls/benches/sign.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/benches/verify.rs` & `chik_rs-0.6.0/crates/chik-bls/benches/verify.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/derive_keys.rs` & `chik_rs-0.6.0/crates/chik-bls/src/derive_keys.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/error.rs` & `chik_rs-0.6.0/crates/chik-bls/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/gtelement.rs` & `chik_rs-0.6.0/crates/chik-bls/src/gtelement.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/lib.rs` & `chik_rs-0.6.0/crates/chik-bls/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/mnemonic.rs` & `chik_rs-0.6.0/crates/chik-bls/src/mnemonic.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use anyhow::Error;
 use bip39::{Language, Mnemonic, Seed};
 use std::array::TryFromSliceError;
-use std::result::Result;
 
 pub fn entropy_to_mnemonic(entropy: &[u8; 32]) -> String {
     Mnemonic::from_entropy(entropy, Language::English)
         .unwrap()
         .into_phrase()
 }
```

### Comparing `chik_rs-0.5.2/chik-bls/src/public_key.rs` & `chik_rs-0.6.0/crates/chik-bls/src/public_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/secret_key.rs` & `chik_rs-0.6.0/crates/chik-bls/src/secret_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik-bls/src/signature.rs` & `chik_rs-0.6.0/crates/chik-bls/src/signature.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 use crate::{Error, GTElement, PublicKey, Result, SecretKey};
 use blst::*;
 use chik_traits::{read_bytes, Streamable};
 use sha2::{Digest, Sha256};
 use std::borrow::Borrow;
-use std::convert::AsRef;
 use std::fmt;
 use std::hash::{Hash, Hasher};
 use std::io::Cursor;
 use std::mem::MaybeUninit;
 use std::ops::{Add, AddAssign, Neg, SubAssign};
 
 #[cfg(feature = "py-bindings")]
```

### Comparing `chik_rs-0.5.2/klvm-traits/Cargo.toml` & `chik_rs-0.6.0/crates/klvm-traits/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [package]
 name = "klvm-traits"
-version = "0.5.2"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Traits for encoding and decoding KLVM objects."
 authors = ["Brandon Haggstrom <b.haggstrom@chiknetwork.com>"]
-homepage = "https://github.com/Chik-Network/chik_rs/klvm-traits/"
-repository = "https://github.com/Chik-Network/chik_rs/klvm-traits/"
+homepage = "https://github.com/Chik-Network/chik_rs"
+repository = "https://github.com/Chik-Network/chik_rs"
 
 [package.metadata.docs.rs]
 features = ["derive", "chik-bls"]
 
 [features]
 derive = ["dep:klvm-derive"]
 chik-bls = ["dep:chik-bls"]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
 pyo3 = { version = ">=0.19.0", optional = true }
-klvmr = "0.5.0"
-klvm-derive = { version = "0.5.2", path = "../klvm-derive", optional = true }
-chik-bls = { version = "0.5.1", path = "../chik-bls", optional = true }
+klvmr = "0.6.1"
+klvm-derive = { version = "0.6.0", path = "../klvm-derive", optional = true }
+chik-bls = { version = "0.6.0", path = "../chik-bls", optional = true }
 num-bigint = "0.4.3"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 hex = "0.4.3"
 hex-literal = "0.4.1"
```

### Comparing `chik_rs-0.5.2/klvm-traits/docs/derive_macros.md` & `chik_rs-0.6.0/crates/klvm-traits/docs/derive_macros.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-traits/src/error.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-traits/src/from_klvm.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/from_klvm.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,27 +12,27 @@
             fn from_klvm(
                 decoder: &impl KlvmDecoder<Node = N>,
                 node: N,
             ) -> Result<Self, FromKlvmError> {
                 const LEN: usize = std::mem::size_of::<$primitive>();
 
                 let bytes = decoder.decode_atom(&node)?;
-                let number = BigInt::from_signed_bytes_be(bytes);
+                let number = BigInt::from_signed_bytes_be(bytes.as_ref());
                 let (sign, mut vec) = number.to_bytes_be();
 
                 if vec.len() < std::mem::size_of::<$primitive>() {
                     let mut zeros = vec![0; LEN - vec.len()];
                     zeros.extend(vec);
                     vec = zeros;
                 }
 
                 let value = <$primitive>::from_be_bytes(vec.as_slice().try_into().or(Err(
                     FromKlvmError::WrongAtomLength {
                         expected: LEN,
-                        found: bytes.len(),
+                        found: bytes.as_ref().len(),
                     },
                 ))?);
 
                 Ok(if sign == Sign::Minus {
                     value.wrapping_neg()
                 } else {
                     value
@@ -67,20 +67,20 @@
         Ok((first, rest))
     }
 }
 
 impl<N> FromKlvm<N> for () {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let bytes = decoder.decode_atom(&node)?;
-        if bytes.is_empty() {
+        if bytes.as_ref().is_empty() {
             Ok(())
         } else {
             Err(FromKlvmError::WrongAtomLength {
                 expected: 0,
-                found: bytes.len(),
+                found: bytes.as_ref().len(),
             })
         }
     }
 }
 
 impl<N, T, const LEN: usize> FromKlvm<N> for [T; LEN]
 where
@@ -94,20 +94,20 @@
                     return Err(FromKlvmError::ExpectedAtom);
                 } else {
                     items.push(T::from_klvm(decoder, first)?);
                     node = rest;
                 }
             } else {
                 let bytes = decoder.decode_atom(&node)?;
-                if bytes.is_empty() {
+                if bytes.as_ref().is_empty() {
                     return items.try_into().or(Err(FromKlvmError::ExpectedPair));
                 } else {
                     return Err(FromKlvmError::WrongAtomLength {
                         expected: 0,
-                        found: bytes.len(),
+                        found: bytes.as_ref().len(),
                     });
                 }
             }
         }
     }
 }
 
@@ -119,70 +119,71 @@
         let mut items = Vec::new();
         loop {
             if let Ok((first, rest)) = decoder.decode_pair(&node) {
                 items.push(T::from_klvm(decoder, first)?);
                 node = rest;
             } else {
                 let bytes = decoder.decode_atom(&node)?;
-                if bytes.is_empty() {
+                if bytes.as_ref().is_empty() {
                     return Ok(items);
                 } else {
                     return Err(FromKlvmError::WrongAtomLength {
                         expected: 0,
-                        found: bytes.len(),
+                        found: bytes.as_ref().len(),
                     });
                 }
             }
         }
     }
 }
 
 impl<N, T> FromKlvm<N> for Option<T>
 where
     T: FromKlvm<N>,
 {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
-        if let Ok(&[]) = decoder.decode_atom(&node) {
-            Ok(None)
-        } else {
-            Ok(Some(T::from_klvm(decoder, node)?))
+        if let Ok(atom) = decoder.decode_atom(&node) {
+            if atom.as_ref().is_empty() {
+                return Ok(None);
+            }
         }
+        Ok(Some(T::from_klvm(decoder, node)?))
     }
 }
 
 impl<N> FromKlvm<N> for String {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let bytes = decoder.decode_atom(&node)?;
-        Ok(Self::from_utf8(bytes.to_vec())?)
+        Ok(Self::from_utf8(bytes.as_ref().to_vec())?)
     }
 }
 
 #[cfg(feature = "chik-bls")]
 impl<N> FromKlvm<N> for chik_bls::PublicKey {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let bytes = decoder.decode_atom(&node)?;
         let error = Err(FromKlvmError::WrongAtomLength {
             expected: 48,
-            found: bytes.len(),
+            found: bytes.as_ref().len(),
         });
-        let bytes = bytes.try_into().or(error)?;
-        Self::from_bytes(bytes).map_err(|error| FromKlvmError::Custom(error.to_string()))
+        let bytes: [u8; 48] = bytes.as_ref().try_into().or(error)?;
+        Self::from_bytes(&bytes).map_err(|error| FromKlvmError::Custom(error.to_string()))
     }
 }
 
 #[cfg(feature = "chik-bls")]
 impl<N> FromKlvm<N> for chik_bls::Signature {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let bytes = decoder.decode_atom(&node)?;
         let error = Err(FromKlvmError::WrongAtomLength {
             expected: 96,
-            found: bytes.len(),
+            found: bytes.as_ref().len(),
         });
-        let bytes = bytes.try_into().or(error)?;
-        Self::from_bytes(bytes).map_err(|error| FromKlvmError::Custom(error.to_string()))
+        let bytes: [u8; 96] = bytes.as_ref().try_into().or(error)?;
+        Self::from_bytes(&bytes).map_err(|error| FromKlvmError::Custom(error.to_string()))
     }
 }
 
 #[cfg(test)]
 mod tests {
     use klvmr::{serde::node_from_bytes, Allocator, NodePtr};
```

### Comparing `chik_rs-0.5.2/klvm-traits/src/klvm_decoder.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/klvm_decoder.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-use klvmr::{allocator::SExp, Allocator, NodePtr};
+use klvmr::{allocator::SExp, Allocator, Atom, NodePtr};
 
 use crate::{FromKlvm, FromKlvmError};
 
 pub trait KlvmDecoder {
     type Node: Clone;
 
-    fn decode_atom(&self, node: &Self::Node) -> Result<&[u8], FromKlvmError>;
+    fn decode_atom(&self, node: &Self::Node) -> Result<Atom, FromKlvmError>;
     fn decode_pair(&self, node: &Self::Node) -> Result<(Self::Node, Self::Node), FromKlvmError>;
 
     /// This is a helper function that just calls `clone` on the node.
     /// It's required only because the compiler can't infer that `N` is `Clone`,
     /// since there's no `Clone` bound on the `FromKlvm` trait.
     fn clone_node(&self, node: &Self::Node) -> Self::Node {
         node.clone()
     }
 }
 
 impl KlvmDecoder for Allocator {
     type Node = NodePtr;
 
-    fn decode_atom(&self, node: &Self::Node) -> Result<&[u8], FromKlvmError> {
+    fn decode_atom(&self, node: &Self::Node) -> Result<Atom, FromKlvmError> {
         if let SExp::Atom = self.sexp(*node) {
             Ok(self.atom(*node))
         } else {
             Err(FromKlvmError::ExpectedAtom)
         }
     }
```

### Comparing `chik_rs-0.5.2/klvm-traits/src/klvm_encoder.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/klvm_encoder.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-traits/src/lib.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-traits/src/macros.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-traits/src/match_byte.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/match_byte.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         let bytes = number.to_signed_bytes_be();
         encoder.encode_atom(&bytes)
     }
 }
 
 impl<N, const BYTE: u8> FromKlvm<N> for MatchByte<BYTE> {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
-        match decoder.decode_atom(&node)? {
+        match decoder.decode_atom(&node)?.as_ref() {
             [] if BYTE == 0 => Ok(Self),
             [byte] if *byte == BYTE && BYTE > 0 => Ok(Self),
             _ => Err(FromKlvmError::Custom(format!(
                 "expected an atom with a single byte value of {}",
                 BYTE
             ))),
         }
```

### Comparing `chik_rs-0.5.2/klvm-traits/src/to_klvm.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/to_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/klvm-traits/src/wrappers.rs` & `chik_rs-0.6.0/crates/klvm-traits/src/wrappers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.5.2/chik_py_streamable_macro/src/lib.rs` & `chik_rs-0.6.0/crates/chik_py_streamable_macro/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
             py_protocol.extend(quote! {
                 #[pyo3::pymethods]
                 impl #ident {
                     #[allow(too_many_arguments)]
                     #[new]
                     #[pyo3(signature = (#(#fnames),*))]
-                    pub fn new ( #(#fnames : #ftypes),* ) -> Self {
+                    pub fn py_new ( #(#fnames : #ftypes),* ) -> Self {
                         Self { #(#fnames),* }
                     }
                 }
             });
 
             py_protocol.extend(quote! {
                 #[pyo3::pymethods]
```

### Comparing `chik_rs-0.5.2/wheel/Cargo.toml` & `chik_rs-0.6.0/crates/chik-consensus/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 [package]
-name = "chik_rs"
-version = "0.5.2"
-authors = ["Richard Kiss <him@richardkiss.com>"]
+name = "chik-consensus"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
-description = "Code useful for implementing chik consensus."
-homepage = "https://github.com/Chik-Network/chik_rs/"
-repository = "https://github.com/Chik-Network/chik_rs/"
-readme = "README.md"
+description = "Utility functions and types used by the Chik blockchain full node"
+authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chiknetwork.com>"]
+homepage = "https://github.com/Chik-Network/chik_rs"
+repository = "https://github.com/Chik-Network/chik_rs"
 
-[lib]
-name = "chik_rs"
-crate-type = ["cdylib"]
-path = "src/lib.rs"
+[features]
+py-bindings = ["dep:pyo3"]
 
 [dependencies]
-klvmr = "0.5.0"
+klvmr = "0.6.1"
 hex = "0.4.3"
-sha2 = "0.10.8"
-pyo3 = { version = "=0.19.0", features = ["extension-module", "multiple-pymethods"] }
-chik = { version = "=0.5.2", path = "..", features = ["py-bindings"] }
-chik-bls = { version = "=0.5.1", path = "../chik-bls", features = ["py-bindings"]  }
-chik-protocol = { version = "=0.5.1", path = "../chik-protocol", features = ["py-bindings"]  }
-chik-traits = { version = "=0.5.2", path = "../chik-traits", features = ["py-bindings"]  }
-klvm-traits = { version = "=0.5.2", path = "../klvm-traits", features = ["derive", "py-bindings"] }
-chik_py_streamable_macro = { version = "=0.5.1", path = "../chik_py_streamable_macro" }
-chik_streamable_macro = { version = "=0.3.0", path = "../chik_streamable_macro" }
-
-# See `../Cargo.toml` for more information on why this is necessary.
-[patch.crates-io]
-blst = { git = "https://github.com/supranational/blst.git", rev = "0d46eefa45fc1e57aceb42bba0e84eab3a7a9725" }
+pyo3 = { version = ">=0.19.0", optional = true }
+klvm-utils = { version = "0.6.0", path = "../klvm-utils" }
+chik-traits = { version = "0.6.0", path = "../chik-traits" }
+klvm-traits = { version = "0.6.0", path = "../klvm-traits" }
+klvm-derive = { version = "0.6.0", path = "../klvm-derive" }
+chik-protocol = { version = "0.6.0", path = "../chik-protocol" }
+chik-wallet = { version = "0.6.0", path = "../chik-wallet" }
+hex-literal = "0.4.1"
+thiserror = "1.0.44"
+
+[dev-dependencies]
+num-traits = "0.2.15"
+rstest = "0.16.0"
+text-diff = "0.4.0"
+criterion = "0.5.1"
+
+[lib]
+bench = false
+
+[[bench]]
+name = "run-generator"
+harness = false
+
+[[bench]]
+name = "tree-hash"
+harness = false
```

### Comparing `chik_rs-0.5.2/wheel/chik_rs.pyi` & `chik_rs-0.6.0/wheel/chik_rs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
+ENABLE_MESSAGE_CONDITIONS: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
 ENABLE_BLS_OPS: int = ...
 ENABLE_SECP_OPS: int = ...
 ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
 ENABLE_FIXED_DIV: int = ...
 ALLOW_BACKREFS: int = ...
@@ -1759,15 +1760,14 @@
     infused_challenge_chain_ip_proof: Optional[VDFProof]
     foliage: Foliage
     foliage_transaction_block: Optional[FoliageTransactionBlock]
     transactions_filter: bytes
     transactions_info: Optional[TransactionsInfo]
     prev_header_hash: bytes32
     prev_hash: bytes32
-    header_hash: bytes32
     height: uint32
     weight: uint128
     header_hash: bytes32
     total_iters: uint128
     log_string: str
     is_transaction_block: bool
     first_in_sub_slot: bool
```

### Comparing `chik_rs-0.5.2/wheel/generate_type_stubs.py` & `chik_rs-0.6.0/wheel/generate_type_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, List, Optional, Tuple
 from glob import glob
 
 output_file = Path(__file__).parent.resolve() / "chik_rs.pyi"
-input_dir = Path(__file__).parent.parent.resolve() / "chik-protocol" / "src"
+input_dir = Path(__file__).parent.parent.resolve() / "crates" / "chik-protocol" / "src"
 
 # enums are exposed to python as int
 enums = set(["NodeType", "ProtocolMessageTypes"])
 
 def transform_type(m: str) -> str:
     n, t = m.split(":")
     if "List[" in t:
@@ -176,15 +176,14 @@
         "weight: uint128",
         "def get_included_reward_coins(self) -> List[Coin]: ...",
         "def is_fully_compactified(self) -> bool: ...",
     ],
     "HeaderBlock": [
         "prev_header_hash: bytes32",
         "prev_hash: bytes32",
-        "header_hash: bytes32",
         "height: uint32",
         "weight: uint128",
         "header_hash: bytes32",
         "total_iters: uint128",
         "log_string: str",
         "is_transaction_block: bool",
         "first_in_sub_slot: bool",
@@ -273,14 +272,15 @@
 
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
+ENABLE_MESSAGE_CONDITIONS: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
 ENABLE_BLS_OPS: int = ...
 ENABLE_SECP_OPS: int = ...
 ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
 ENABLE_FIXED_DIV: int = ...
 ALLOW_BACKREFS: int = ...
```

### Comparing `chik_rs-0.5.2/wheel/src/api.rs` & `chik_rs-0.6.0/wheel/src/api.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-use crate::compression;
 use crate::run_generator::{
     convert_spend_bundle_conds, run_block_generator, run_block_generator2, PySpend,
     PySpendBundleConditions,
 };
-use chik::allocator::make_allocator;
-use chik::gen::conditions::MempoolVisitor;
-use chik::gen::flags::{
-    AGG_SIG_ARGS, ALLOW_BACKREFS, ANALYZE_SPENDS, COND_ARGS_NIL, ENABLE_SOFTFORK_CONDITION,
-    MEMPOOL_MODE, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
+use chik_consensus::allocator::make_allocator;
+use chik_consensus::gen::conditions::MempoolVisitor;
+use chik_consensus::gen::flags::{
+    AGG_SIG_ARGS, ALLOW_BACKREFS, ANALYZE_SPENDS, COND_ARGS_NIL, ENABLE_MESSAGE_CONDITIONS,
+    ENABLE_SOFTFORK_CONDITION, MEMPOOL_MODE, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS,
+    STRICT_ARGS_COUNT,
 };
-use chik::gen::run_puzzle::run_puzzle as native_run_puzzle;
-use chik::gen::solution_generator::solution_generator as native_solution_generator;
-use chik::gen::solution_generator::solution_generator_backrefs as native_solution_generator_backrefs;
-use chik::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
+use chik_consensus::gen::run_puzzle::run_puzzle as native_run_puzzle;
+use chik_consensus::gen::solution_generator::solution_generator as native_solution_generator;
+use chik_consensus::gen::solution_generator::solution_generator_backrefs as native_solution_generator_backrefs;
+use chik_consensus::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
 use chik_protocol::{
     BlockRecord, Bytes32, ChallengeBlockInfo, ChallengeChainSubSlot, ClassgroupElement, Coin,
     CoinSpend, CoinState, CoinStateUpdate, EndOfSubSlotBundle, Foliage, FoliageBlockData,
     FoliageTransactionBlock, FullBlock, HeaderBlock, InfusedChallengeChainSubSlot, NewCompactVDF,
     NewPeak, NewPeakWallet, NewSignagePointOrEndOfSubSlot, NewTransaction, NewUnfinishedBlock,
     PoolTarget, Program, ProofBlockHeader, ProofOfSpace, PuzzleSolutionResponse, RecentChainData,
     RegisterForCoinUpdates, RegisterForPhUpdates, RejectAdditionsRequest, RejectBlock,
@@ -31,34 +31,31 @@
     RespondHeaderBlocks, RespondPeers, RespondProofOfWeight, RespondPuzzleSolution,
     RespondRemovals, RespondSesInfo, RespondSignagePoint, RespondToCoinUpdates, RespondToPhUpdates,
     RespondTransaction, RespondUnfinishedBlock, RewardChainBlock, RewardChainBlockUnfinished,
     RewardChainSubSlot, SendTransaction, SpendBundle, SubEpochChallengeSegment, SubEpochData,
     SubEpochSegments, SubEpochSummary, SubSlotData, SubSlotProofs, TimestampedPeerInfo,
     TransactionAck, TransactionsInfo, UnfinishedBlock, VDFInfo, VDFProof, WeightProof,
 };
-use klvmr::serde::tree_hash_from_stream;
+use klvm_utils::tree_hash_from_bytes;
 use klvmr::{ENABLE_BLS_OPS_OUTSIDE_GUARD, ENABLE_FIXED_DIV, LIMIT_HEAP, NO_UNKNOWN_OPS};
 use pyo3::buffer::PyBuffer;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
-use pyo3::types::PyAny;
 use pyo3::types::PyBytes;
 use pyo3::types::PyList;
-use pyo3::types::PyModule;
 use pyo3::types::PyTuple;
-use pyo3::{wrap_pyfunction, PyResult, Python};
-use std::convert::TryInto;
+use pyo3::wrap_pyfunction;
 use std::iter::zip;
 
 use crate::run_program::{run_chik_program, serialized_length};
 
 use crate::adapt_response::eval_err_to_pyresult;
-use chik::fast_forward::fast_forward_singleton as native_ff;
-use chik::gen::get_puzzle_and_solution::get_puzzle_and_solution_for_coin as parse_puzzle_solution;
-use chik::gen::validation_error::ValidationErr;
+use chik_consensus::fast_forward::fast_forward_singleton as native_ff;
+use chik_consensus::gen::get_puzzle_and_solution::get_puzzle_and_solution_for_coin as parse_puzzle_solution;
+use chik_consensus::gen::validation_error::ValidationErr;
 use klvmr::allocator::NodePtr;
 use klvmr::cost::Cost;
 use klvmr::reduction::EvalErr;
 use klvmr::reduction::Reduction;
 use klvmr::run_program;
 use klvmr::serde::node_to_bytes;
 use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
@@ -83,16 +80,15 @@
 #[pyfunction]
 pub fn tree_hash(py: Python, blob: PyBuffer<u8>) -> PyResult<&PyBytes> {
     if !blob.is_c_contiguous() {
         panic!("tree_hash() must be called with a contiguous buffer");
     }
     let slice =
         unsafe { std::slice::from_raw_parts(blob.buf_ptr() as *const u8, blob.len_bytes()) };
-    let mut input = std::io::Cursor::<&[u8]>::new(slice);
-    Ok(PyBytes::new(py, &tree_hash_from_stream(&mut input)?))
+    Ok(PyBytes::new(py, &tree_hash_from_bytes(slice)?))
 }
 
 #[allow(clippy::too_many_arguments)]
 #[pyfunction]
 pub fn get_puzzle_and_solution_for_coin(
     py: Python<'_>,
     program: PyBuffer<u8>,
@@ -140,15 +136,15 @@
         let serialize = if (flags & ALLOW_BACKREFS) != 0 {
             node_to_bytes_backrefs
         } else {
             node_to_bytes
         };
     */
     match r {
-        Err(eval_err) => eval_err_to_pyresult(py, eval_err, allocator),
+        Err(eval_err) => eval_err_to_pyresult(eval_err, allocator),
         Ok((puzzle, solution)) => Ok((
             PyBytes::new(py, &serialize(&allocator, puzzle)?),
             PyBytes::new(py, &serialize(&allocator, solution)?),
         )),
     }
 }
 
@@ -284,15 +280,15 @@
     // the test function just attempts the rebase onto a dummy parent coin
     let new_parent = Coin {
         parent_coin_info: [0_u8; 32].into(),
         puzzle_hash: spend.coin.puzzle_hash,
         amount: spend.coin.amount,
     };
     let new_coin = Coin {
-        parent_coin_info: new_parent.coin_id().into(),
+        parent_coin_info: new_parent.coin_id(),
         puzzle_hash: spend.coin.puzzle_hash,
         amount: spend.coin.amount,
     };
 
     let mut a = make_allocator(LIMIT_HEAP);
     let Ok(puzzle) = node_from_bytes(&mut a, spend.puzzle_reveal.as_slice()) else {
         return false;
@@ -327,38 +323,42 @@
     Ok(PyBytes::new(
         py,
         node_to_bytes(&a, new_solution)?.as_slice(),
     ))
 }
 
 #[pymodule]
-pub fn chik_rs(py: Python, m: &PyModule) -> PyResult<()> {
+pub fn chik_rs(_py: Python, m: &PyModule) -> PyResult<()> {
     // generator functions
     m.add_function(wrap_pyfunction!(run_block_generator, m)?)?;
     m.add_function(wrap_pyfunction!(run_block_generator2, m)?)?;
     m.add_function(wrap_pyfunction!(run_puzzle, m)?)?;
     m.add_function(wrap_pyfunction!(solution_generator, m)?)?;
     m.add_function(wrap_pyfunction!(solution_generator_backrefs, m)?)?;
     m.add_function(wrap_pyfunction!(supports_fast_forward, m)?)?;
     m.add_function(wrap_pyfunction!(fast_forward_singleton, m)?)?;
     m.add_class::<PySpendBundleConditions>()?;
     m.add(
         "ELIGIBLE_FOR_DEDUP",
-        chik::gen::conditions::ELIGIBLE_FOR_DEDUP,
+        chik_consensus::gen::conditions::ELIGIBLE_FOR_DEDUP,
+    )?;
+    m.add(
+        "ELIGIBLE_FOR_FF",
+        chik_consensus::gen::conditions::ELIGIBLE_FOR_FF,
     )?;
-    m.add("ELIGIBLE_FOR_FF", chik::gen::conditions::ELIGIBLE_FOR_FF)?;
     m.add_class::<PySpend>()?;
 
     // klvm functions
     m.add("COND_ARGS_NIL", COND_ARGS_NIL)?;
     m.add("NO_UNKNOWN_CONDS", NO_UNKNOWN_CONDS)?;
     m.add("STRICT_ARGS_COUNT", STRICT_ARGS_COUNT)?;
     m.add("AGG_SIG_ARGS", AGG_SIG_ARGS)?;
     m.add("ENABLE_FIXED_DIV", ENABLE_FIXED_DIV)?;
     m.add("ENABLE_SOFTFORK_CONDITION", ENABLE_SOFTFORK_CONDITION)?;
+    m.add("ENABLE_MESSAGE_CONDITIONS", ENABLE_MESSAGE_CONDITIONS)?;
     m.add(
         "NO_RELATIVE_CONDITIONS_ON_EPHEMERAL",
         NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
     )?;
     m.add("MEMPOOL_MODE", MEMPOOL_MODE)?;
     m.add("ALLOW_BACKREFS", ALLOW_BACKREFS)?;
     m.add("ANALYZE_SPENDS", ANALYZE_SPENDS)?;
@@ -478,11 +478,9 @@
 
     m.add_class::<PublicKey>()?;
     m.add_class::<Signature>()?;
     m.add_class::<GTElement>()?;
     m.add_class::<SecretKey>()?;
     m.add_class::<AugSchemeMPL>()?;
 
-    compression::add_submodule(py, m)?;
-
     Ok(())
 }
```

### Comparing `chik_rs-0.5.2/wheel/src/run_generator.rs` & `chik_rs-0.6.0/wheel/src/run_generator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use chik::allocator::make_allocator;
-use chik::gen::conditions::{EmptyVisitor, MempoolVisitor, Spend, SpendBundleConditions};
-use chik::gen::flags::ANALYZE_SPENDS;
-use chik::gen::run_block_generator::run_block_generator as native_run_block_generator;
-use chik::gen::run_block_generator::run_block_generator2 as native_run_block_generator2;
-use chik::gen::validation_error::ValidationErr;
+use chik_consensus::allocator::make_allocator;
+use chik_consensus::gen::conditions::{EmptyVisitor, MempoolVisitor, Spend, SpendBundleConditions};
+use chik_consensus::gen::flags::ANALYZE_SPENDS;
+use chik_consensus::gen::run_block_generator::run_block_generator as native_run_block_generator;
+use chik_consensus::gen::run_block_generator::run_block_generator2 as native_run_block_generator2;
+use chik_consensus::gen::validation_error::ValidationErr;
 use chik_protocol::bytes::{Bytes, Bytes32, Bytes48};
 
 use klvmr::allocator::{Allocator, NodePtr};
 use klvmr::cost::Cost;
 
 use pyo3::buffer::PyBuffer;
 use pyo3::prelude::*;
@@ -64,38 +64,41 @@
     // the sum of all amounts of CREATE_COIN conditions
     pub addition_amount: u128,
 }
 
 fn convert_agg_sigs(a: &Allocator, agg_sigs: &[(NodePtr, NodePtr)]) -> Vec<(Bytes48, Bytes)> {
     let mut ret = Vec::<(Bytes48, Bytes)>::new();
     for (pk, msg) in agg_sigs {
-        ret.push((a.atom(*pk).try_into().unwrap(), a.atom(*msg).into()));
+        ret.push((
+            a.atom(*pk).as_ref().try_into().unwrap(),
+            a.atom(*msg).as_ref().into(),
+        ));
     }
     ret
 }
 
 fn convert_spend(a: &Allocator, spend: Spend) -> PySpend {
     let mut create_coin =
         Vec::<(Bytes32, u64, Option<Bytes>)>::with_capacity(spend.create_coin.len());
     for c in spend.create_coin {
         create_coin.push((
             c.puzzle_hash,
             c.amount,
             if c.hint != a.nil() {
-                Some(a.atom(c.hint).into())
+                Some(a.atom(c.hint).as_ref().into())
             } else {
                 None
             },
         ));
     }
 
     PySpend {
         coin_id: *spend.coin_id,
-        parent_id: a.atom(spend.parent_id).try_into().unwrap(),
-        puzzle_hash: a.atom(spend.puzzle_hash).try_into().unwrap(),
+        parent_id: a.atom(spend.parent_id).as_ref().try_into().unwrap(),
+        puzzle_hash: a.atom(spend.puzzle_hash).as_ref().try_into().unwrap(),
         coin_amount: spend.coin_amount,
         height_relative: spend.height_relative,
         seconds_relative: spend.seconds_relative,
         before_height_relative: spend.before_height_relative,
         before_seconds_relative: spend.before_seconds_relative,
         birth_height: spend.birth_height,
         birth_seconds: spend.birth_seconds,
@@ -118,15 +121,18 @@
     let mut spends = Vec::<PySpend>::new();
     for s in sb.spends {
         spends.push(convert_spend(a, s));
     }
 
     let mut agg_sigs = Vec::<(Bytes48, Bytes)>::with_capacity(sb.agg_sig_unsafe.len());
     for (pk, msg) in sb.agg_sig_unsafe {
-        agg_sigs.push((a.atom(pk).try_into().unwrap(), a.atom(msg).into()));
+        agg_sigs.push((
+            a.atom(pk).as_ref().try_into().unwrap(),
+            a.atom(msg).as_ref().into(),
+        ));
     }
 
     PySpendBundleConditions {
         spends,
         reserve_fee: sb.reserve_fee,
         height_absolute: sb.height_absolute,
         seconds_absolute: sb.seconds_absolute,
```

### Comparing `chik_rs-0.5.2/wheel/src/run_program.rs` & `chik_rs-0.6.0/wheel/src/run_program.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use super::adapt_response::eval_err_to_pyresult;
-use chik::allocator::make_allocator;
-use chik::gen::flags::ALLOW_BACKREFS;
+use chik_consensus::allocator::make_allocator;
+use chik_consensus::gen::flags::ALLOW_BACKREFS;
 use chik_protocol::LazyNode;
 use klvmr::chik_dialect::ChikDialect;
 use klvmr::cost::Cost;
 use klvmr::reduction::Response;
 use klvmr::run_program::run_program;
 use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs, serialized_length_from_bytes};
 use pyo3::buffer::PyBuffer;
@@ -46,10 +46,10 @@
         Ok(py.allow_threads(|| run_program(&mut allocator, &dialect, program, args, max_cost)))
     })()?;
     match r {
         Ok(reduction) => {
             let val = LazyNode::new(Rc::new(allocator), reduction.1);
             Ok((reduction.0, val))
         }
-        Err(eval_err) => eval_err_to_pyresult(py, eval_err, allocator),
+        Err(eval_err) => eval_err_to_pyresult(eval_err, allocator),
     }
 }
```

