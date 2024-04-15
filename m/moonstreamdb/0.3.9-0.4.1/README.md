# Comparing `tmp/moonstreamdb-0.3.9.tar.gz` & `tmp/moonstreamdb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-0.3.9.tar", last modified: Thu Mar 28 12:52:03 2024, max compression
+gzip compressed data, was "moonstreamdb-0.4.1.tar", last modified: Mon Apr 15 11:07:53 2024, max compression
```

## Comparing `moonstreamdb-0.3.9.tar` & `moonstreamdb-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/moonstreamdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    47298 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/moonstreamdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:51:54.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/moonstreamdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61400 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/moonstreamdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:07:43.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/setup.py
```

### Comparing `moonstreamdb-0.3.9/PKG-INFO` & `moonstreamdb-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.3.9
+Version: 0.4.1
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.3.9/README.md` & `moonstreamdb-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.9/moonstreamdb/blockchain.py` & `moonstreamdb-0.4.1/moonstreamdb/blockchain.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 from enum import Enum
 from typing import Type, Union
 
 from .models import (
+    AmoyBlock,
+    AmoyLabel,
+    AmoyTransaction,
     ArbitrumNovaBlock,
     ArbitrumNovaLabel,
     ArbitrumNovaTransaction,
     ArbitrumSepoliaBlock,
     ArbitrumSepoliaLabel,
     ArbitrumSepoliaTransaction,
     AvalancheBlock,
     AvalancheFujiBlock,
     AvalancheFujiLabel,
     AvalancheFujiTransaction,
     AvalancheLabel,
     AvalancheTransaction,
+    BlastBlock,
+    BlastLabel,
+    BlastSepoliaBlock,
+    BlastSepoliaLabel,
+    BlastSepoliaTransaction,
+    BlastTransaction,
     EthereumBlock,
     EthereumLabel,
     EthereumTransaction,
     MumbaiBlock,
     MumbaiLabel,
     MumbaiTransaction,
     PolygonBlock,
     PolygonLabel,
     PolygonTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
     XaiBlock,
     XaiLabel,
+    XaiSepoliaBlock,
+    XaiSepoliaLabel,
+    XaiSepoliaTransaction,
     XaiTransaction,
     XDaiBlock,
     XDaiLabel,
     XDaiTransaction,
     ZkSyncEraBlock,
     ZkSyncEraLabel,
     ZkSyncEraSepoliaBlock,
@@ -44,72 +56,85 @@
 )
 
 
 class AvailableBlockchainType(Enum):
     ETHEREUM = "ethereum"
     POLYGON = "polygon"
     MUMBAI = "mumbai"
+    AMOY = "amoy"
     XDAI = "xdai"
     WYRM = "wyrm"
     ZKSYNC_ERA = "zksync_era"
     ZKSYNC_ERA_TESTNET = "zksync_era_testnet"
     ZKSYNC_ERA_SEPOLIA = "zksync_era_sepolia"
     ARBITRUM_NOVA = "arbitrum_nova"
     ARBITRUM_SEPOLIA = "arbitrum_sepolia"
     XAI = "xai"
+    XAI_SEPOLIA = "xai_sepolia"
     AVALANCHE = "avalanche"
     AVALANCHE_FUJI = "avalanche_fuji"
+    BLAST = "blast"
+    BLAST_SEPOLIA = "blast_sepolia"
 
 
 def get_block_model(
     blockchain_type: AvailableBlockchainType,
 ) -> Type[
     Union[
         EthereumBlock,
         PolygonBlock,
         MumbaiBlock,
+        AmoyBlock,
         XDaiBlock,
         WyrmBlock,
         ZkSyncEraTestnetBlock,
         ZkSyncEraBlock,
         ZkSyncEraSepoliaBlock,
         ArbitrumNovaBlock,
         ArbitrumSepoliaBlock,
         XaiBlock,
+        XaiSepoliaBlock,
         AvalancheBlock,
         AvalancheFujiBlock,
+        BlastBlock,
+        BlastSepoliaBlock,
     ]
 ]:
     """
-    Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm, ZkSyncEra, ZkSyncEraTestnet, ArbitrumNovaBlock, ArbitrumSepoliaBlock, XaiBlock
-    set proper blocks model.
+    Depends on provided blockchain type set proper blocks model.
     """
     block_model: Type[
         Union[
             EthereumBlock,
             PolygonBlock,
             MumbaiBlock,
+            AmoyBlock,
             XDaiBlock,
             WyrmBlock,
             ZkSyncEraTestnetBlock,
             ZkSyncEraBlock,
             ZkSyncEraSepoliaBlock,
             ArbitrumNovaBlock,
             ArbitrumSepoliaBlock,
             XaiBlock,
+            XaiSepoliaBlock,
             AvalancheBlock,
             AvalancheFujiBlock,
+            BlastBlock,
+            BlastSepoliaBlock,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         block_model = EthereumBlock
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         block_model = PolygonBlock
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
         block_model = MumbaiBlock
+    elif blockchain_type == AvailableBlockchainType.AMOY:
+        block_model = AmoyBlock
     elif blockchain_type == AvailableBlockchainType.XDAI:
         block_model = XDaiBlock
     elif blockchain_type == AvailableBlockchainType.WYRM:
         block_model = WyrmBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         block_model = ZkSyncEraTestnetBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
@@ -118,70 +143,85 @@
         block_model = ZkSyncEraSepoliaBlock
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         block_model = ArbitrumNovaBlock
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         block_model = ArbitrumSepoliaBlock
     elif blockchain_type == AvailableBlockchainType.XAI:
         block_model = XaiBlock
+    elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
+        block_model = XaiSepoliaBlock
     elif blockchain_type == AvailableBlockchainType.AVALANCHE:
         block_model = AvalancheBlock
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         block_model = AvalancheFujiBlock
+    elif blockchain_type == AvailableBlockchainType.BLAST:
+        block_model = BlastBlock
+    elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
+        block_model = BlastSepoliaBlock
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return block_model
 
 
 def get_label_model(
     blockchain_type: AvailableBlockchainType,
 ) -> Type[
     Union[
         EthereumLabel,
         PolygonLabel,
         MumbaiLabel,
+        AmoyLabel,
         XDaiLabel,
         WyrmLabel,
         ZkSyncEraTestnetLabel,
         ZkSyncEraLabel,
         ZkSyncEraSepoliaLabel,
         ArbitrumNovaLabel,
         ArbitrumSepoliaLabel,
         XaiLabel,
+        XaiSepoliaLabel,
         AvalancheLabel,
         AvalancheFujiLabel,
+        BlastLabel,
+        BlastSepoliaLabel,
     ]
 ]:
     """
-    Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm, ZkSyncEra, ZkSyncEraTestnet, ArbitrumNovaLabel, ArbitrumSepoliaLabel, XaiLabel
-    set proper block label model.
+    Depends on provided blockchain type set proper block label model.
     """
     label_model: Type[
         Union[
             EthereumLabel,
             PolygonLabel,
             MumbaiLabel,
+            AmoyLabel,
             XDaiLabel,
             WyrmLabel,
             ZkSyncEraTestnetLabel,
             ZkSyncEraLabel,
             ZkSyncEraSepoliaLabel,
             ArbitrumNovaLabel,
             ArbitrumSepoliaLabel,
             XaiLabel,
+            XaiSepoliaLabel,
             AvalancheLabel,
             AvalancheFujiLabel,
+            BlastLabel,
+            BlastSepoliaLabel,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         label_model = EthereumLabel
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         label_model = PolygonLabel
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
         label_model = MumbaiLabel
+    elif blockchain_type == AvailableBlockchainType.AMOY:
+        label_model = AmoyLabel
     elif blockchain_type == AvailableBlockchainType.XDAI:
         label_model = XDaiLabel
     elif blockchain_type == AvailableBlockchainType.WYRM:
         label_model = WyrmLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         label_model = ZkSyncEraTestnetLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
@@ -190,71 +230,85 @@
         label_model = ZkSyncEraSepoliaLabel
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         label_model = ArbitrumNovaLabel
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         label_model = ArbitrumSepoliaLabel
     elif blockchain_type == AvailableBlockchainType.XAI:
         label_model = XaiLabel
+    elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
+        label_model = XaiSepoliaLabel
     elif blockchain_type == AvailableBlockchainType.AVALANCHE:
         label_model = AvalancheLabel
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         label_model = AvalancheFujiLabel
-
+    elif blockchain_type == AvailableBlockchainType.BLAST:
+        label_model = BlastLabel
+    elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
+        label_model = BlastSepoliaLabel
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return label_model
 
 
 def get_transaction_model(
     blockchain_type: AvailableBlockchainType,
 ) -> Type[
     Union[
         EthereumTransaction,
         PolygonTransaction,
         MumbaiTransaction,
+        AmoyTransaction,
         XDaiTransaction,
         WyrmTransaction,
         ZkSyncEraTestnetTransaction,
         ZkSyncEraTransaction,
         ZkSyncEraSepoliaTransaction,
         ArbitrumNovaTransaction,
         ArbitrumSepoliaTransaction,
         XaiTransaction,
+        XaiSepoliaTransaction,
         AvalancheTransaction,
         AvalancheFujiTransaction,
+        BlastTransaction,
+        BlastSepoliaTransaction,
     ]
 ]:
     """
-    Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm, ZkSyncEra, ZkSyncEraTestnet, ArbitrumNovaTransaction, ArbitrumSepoliaTransaction, XaiTransaction
-    set proper block transactions model.
+    Depends on provided blockchain type set proper block transactions model.
     """
     transaction_model: Type[
         Union[
             EthereumTransaction,
             PolygonTransaction,
             MumbaiTransaction,
+            AmoyTransaction,
             XDaiTransaction,
             WyrmTransaction,
             ZkSyncEraTestnetTransaction,
             ZkSyncEraTransaction,
             ZkSyncEraSepoliaTransaction,
             ArbitrumNovaTransaction,
             ArbitrumSepoliaTransaction,
             XaiTransaction,
+            XaiSepoliaTransaction,
             AvalancheTransaction,
             AvalancheFujiTransaction,
+            BlastTransaction,
+            BlastSepoliaTransaction,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         transaction_model = EthereumTransaction
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         transaction_model = PolygonTransaction
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
         transaction_model = MumbaiTransaction
+    elif blockchain_type == AvailableBlockchainType.AMOY:
+        transaction_model = AmoyTransaction
     elif blockchain_type == AvailableBlockchainType.XDAI:
         transaction_model = XDaiTransaction
     elif blockchain_type == AvailableBlockchainType.WYRM:
         transaction_model = WyrmTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         transaction_model = ZkSyncEraTestnetTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
@@ -263,15 +317,21 @@
         transaction_model = ZkSyncEraSepoliaTransaction
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         transaction_model = ArbitrumNovaTransaction
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         transaction_model = ArbitrumSepoliaTransaction
     elif blockchain_type == AvailableBlockchainType.XAI:
         transaction_model = XaiTransaction
+    elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
+        transaction_model = XaiSepoliaTransaction
     elif blockchain_type == AvailableBlockchainType.AVALANCHE:
         transaction_model = AvalancheTransaction
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         transaction_model = AvalancheFujiTransaction
+    elif blockchain_type == AvailableBlockchainType.BLAST:
+        transaction_model = BlastTransaction
+    elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
+        transaction_model = BlastSepoliaTransaction
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return transaction_model
```

### Comparing `moonstreamdb-0.3.9/moonstreamdb/cli.py` & `moonstreamdb-0.4.1/moonstreamdb/cli.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.9/moonstreamdb/db.py` & `moonstreamdb-0.4.1/moonstreamdb/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.9/moonstreamdb/models.py` & `moonstreamdb-0.4.1/moonstreamdb/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -364,14 +364,121 @@
     block_timestamp = Column(BigInteger, index=True)
     log_index = Column(Integer, nullable=True)
     created_at = Column(
         DateTime(timezone=True), server_default=utcnow(), nullable=False
     )
 
 
+class AmoyBlock(Base):  # type: ignore
+    __tablename__ = "amoy_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
+class AmoyTransaction(Base):  # type: ignore
+    __tablename__ = "amoy_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("amoy_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
+class AmoyLabel(Base):  # type: ignore
+    __tablename__ = "amoy_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_amoy_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_amoy_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
 class XDaiBlock(Base):  # type: ignore
     __tablename__ = "xdai_blocks"
 
     author = Column(VARCHAR(128))
     block_number = Column(
         BigInteger, primary_key=True, unique=True, nullable=False, index=True
     )
@@ -1212,14 +1319,144 @@
 
     y_parity = Column(BigInteger, nullable=True)
 
 
 class XaiLabel(Base):  # type: ignore
     __tablename__ = "xai_labels"
 
+    __table_args__ = (
+        Index(
+            "ix_xai_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_xai_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
+class XaiSepoliaBlock(Base):  # type: ignore
+    __tablename__ = "xai_sepolia_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+    l1_block_number = Column(BigInteger, nullable=True)
+    send_count = Column(BigInteger, nullable=True)
+    send_root = Column(VARCHAR(256), nullable=True)
+    mix_hash = Column(VARCHAR(256), nullable=True)
+
+
+class XaiSepoliaTransaction(Base):  # type: ignore
+    __tablename__ = "xai_sepolia_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("xai_sepolia_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    y_parity = Column(BigInteger, nullable=True)
+
+
+class XaiSepoliaLabel(Base):  # type: ignore
+    __tablename__ = "xai_sepolia_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_xai_sepolia_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_xai_sepolia_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
     id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
         nullable=False,
     )
@@ -1272,15 +1509,15 @@
     transactions_root = Column(VARCHAR(256))
 
     indexed_at = Column(
         DateTime(timezone=True), server_default=utcnow(), nullable=False
     )
 
     mix_hash = Column(VARCHAR(256), nullable=True)
-    block_extra_data = Column(VARCHAR(256), nullable=True)
+    block_extra_data = Column(Text, nullable=True)
     block_gas_cost = Column(VARCHAR(256), nullable=True)
     ext_data_gas_used = Column(VARCHAR(256), nullable=True)
     ext_data_hash = Column(VARCHAR(256), nullable=True)
 
 
 class AvalancheTransaction(Base):  # type: ignore
     __tablename__ = "avalanche_transactions"
@@ -1439,14 +1676,240 @@
             "address",
             "block_timestamp",
             unique=False,
         ),
     )
 
     id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
+class BlastBlock(Base):  # type: ignore
+    __tablename__ = "blast_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+    withdrawals_root = Column(VARCHAR(256), nullable=True)
+    mix_hash = Column(VARCHAR(256), nullable=True)
+
+
+class BlastTransaction(Base):  # type: ignore
+    __tablename__ = "blast_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("blast_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    y_parity = Column(BigInteger, nullable=True)
+
+
+class BlastLabel(Base):  # type: ignore
+    __tablename__ = "blast_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_blast_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_blast_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
+class BlastSepoliaBlock(Base):  # type: ignore
+    __tablename__ = "blast_sepolia_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+    withdrawals_root = Column(VARCHAR(256), nullable=True)
+    mix_hash = Column(VARCHAR(256), nullable=True)
+
+
+class BlastSepoliaTransaction(Base):  # type: ignore
+    __tablename__ = "blast_sepolia_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("blast_sepolia_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    y_parity = Column(BigInteger, nullable=True)
+
+
+class BlastSepoliaLabel(Base):  # type: ignore
+    __tablename__ = "blast_sepolia_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_blast_sepolia_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_blast_sepolia_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
         nullable=False,
     )
     label = Column(VARCHAR(256), nullable=False, index=True)
```

### Comparing `moonstreamdb-0.3.9/moonstreamdb.egg-info/PKG-INFO` & `moonstreamdb-0.4.1/moonstreamdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.3.9
+Version: 0.4.1
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.3.9/setup.py` & `moonstreamdb-0.4.1/setup.py`

 * *Files identical despite different names*

