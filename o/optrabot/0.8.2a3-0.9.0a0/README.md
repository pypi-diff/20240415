# Comparing `tmp/optrabot-0.8.2a3.tar.gz` & `tmp/optrabot-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.8.2a3.tar", max compression
+gzip compressed data, was "optrabot-0.9.0a0.tar", max compression
```

## Comparing `optrabot-0.8.2a3.tar` & `optrabot-0.9.0a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.2a3/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.2a3/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.2a3/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.2a3/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.2a3/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.2a3/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.2a3/optrabot/alembic.ini
--rw-r--r--   0        0        0    11856 2024-04-10 09:35:09.326796 optrabot-0.8.2a3/optrabot/config.py
--rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.2a3/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.2a3/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-04-10 09:35:05.013016 optrabot-0.8.2a3/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.2a3/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.2a3/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.2a3/optrabot/optionhelper.py
--rw-r--r--   0        0        0    10529 2024-04-10 10:47:37.272398 optrabot-0.8.2a3/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.2a3/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.2a3/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.2a3/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.2a3/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.2a3/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.2a3/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.2a3/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.2a3/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.2a3/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    35316 2024-04-08 18:36:39.426454 optrabot-0.8.2a3/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      821 2024-04-10 10:48:31.209652 optrabot-0.8.2a3/pyproject.toml
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.8.2a3/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.0a0/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.0a0/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.0a0/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.0a0/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.0a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.0a0/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11856 2024-04-15 10:03:53.634164 optrabot-0.9.0a0/optrabot/config.py
+-rw-r--r--   0        0        0     3133 2024-04-15 10:03:22.750198 optrabot-0.9.0a0/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.0a0/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-04-10 09:35:05.013016 optrabot-0.9.0a0/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.0a0/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.0a0/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.0a0/optrabot/optionhelper.py
+-rw-r--r--   0        0        0    10551 2024-04-15 10:03:53.634677 optrabot-0.9.0a0/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.0a0/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.0a0/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.0a0/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.0a0/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.9.0a0/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.0a0/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.0a0/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.9.0a0/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.0a0/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    39299 2024-04-15 10:03:53.634965 optrabot-0.9.0a0/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      821 2024-04-15 10:13:49.235821 optrabot-0.9.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.9.0a0/PKG-INFO
```

### Comparing `optrabot-0.8.2a3/README.md` & `optrabot-0.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/alembic/env.py` & `optrabot-0.9.0a0/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/alembic/script.py.mako` & `optrabot-0.9.0a0/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.9.0a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/alembic.ini` & `optrabot-0.9.0a0/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/config.py` & `optrabot-0.9.0a0/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/crud.py` & `optrabot-0.9.0a0/optrabot/crud.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,21 @@
 def getMaxTransactionId(session: Session, tradeId: int) -> int:
 	statement = select(func.max(models.Transaction.id)).filter_by(tradeid=tradeId)
 	maxId = session.scalar(statement)
 	if maxId == None:
 		maxId = 0
 	return maxId
 
+def getTransactionById(session: Session, tradeId: int, transactionId: int) -> models.Transaction:
+	""" Fetches the transaction based on the Trade ID and Transaction ID
+	"""
+	statement = select(models.Transaction).filter_by(tradeid=tradeId, id=transactionId)
+	transaction = session.scalars(statement).first()
+	return transaction
+
 def createTransaction(session: Session, newTransaction: schemas.TransactionCreate) -> models.Transaction:
 	""" Creates a new transaction record for the given trade
 	"""
 	dbTransaction = models.Transaction(tradeid=newTransaction.tradeid, id=newTransaction.id,
 									type=newTransaction.type,
 									sectype=newTransaction.sectype,
 									timestamp=newTransaction.timestamp,
```

### Comparing `optrabot-0.8.2a3/optrabot/database.py` & `optrabot-0.9.0a0/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/main.py` & `optrabot-0.9.0a0/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/marketdatatype.py` & `optrabot-0.9.0a0/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/models.py` & `optrabot-0.9.0a0/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/optionhelper.py` & `optrabot-0.9.0a0/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/optrabot.py` & `optrabot-0.9.0a0/optrabot/optrabot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import array
 from collections import OrderedDict
 import asyncio
 import datetime as dt
 import json
-import logging
 from fastapi import FastAPI
 from ib_insync import *
-from ib_insync import util
 from loguru import logger
 from sqlalchemy.orm import Session
 from optrabot import schemas
 from optrabot.marketdatatype import MarketDataType
 from optrabot.optionhelper import OptionHelper
 from optrabot.config import Config
 from .tradinghubclient import TradinghubClient
@@ -118,14 +116,15 @@
 		try:
 			ib: IB = self['ib']
 			ib.errorEvent += self.onErrorEvent
 			await ib.connectAsync(twshost, twsport, clientId=twsclient)
 			logger.debug("Connected to IB")
 			ib.disconnectedEvent += self.onDisconnected
 			ib.execDetailsEvent += self.thc.onExecDetailsEvent
+			ib.commissionReportEvent += self.thc.onCommissionReportEvent
 			with Session(get_db_engine()) as session:
 				for managedAccount in ib.managedAccounts():
 					logger.debug('Managed Account: {}', managedAccount)
 					known_account = crud.get_account(session, managedAccount)
 					if known_account == None:
 						logger.debug('Account is new. Adding it to the Database')
 						new_account = schemas.AccountCreate( id = managedAccount, name = managedAccount, broker = 'IBKR', pdt=False)
```

### Comparing `optrabot-0.8.2a3/optrabot/schemas.py` & `optrabot-0.9.0a0/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/stoplossadjuster.py` & `optrabot-0.9.0a0/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/tradehelper.py` & `optrabot-0.9.0a0/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/tradetemplate/template.py` & `optrabot-0.9.0a0/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.9.0a0/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.9.0a0/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a3/optrabot/tradinghubclient.py` & `optrabot-0.9.0a0/optrabot/tradinghubclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 		self._ironFlyShortComboContract = None
 		self._longLegFillsPrice = 0.0
 		self._longLegFillsReceived = 0
 		self._shuttingdown = False
 		#self._positionMonitorTask = None
 		self._position = False
 		self._closingLongLegs = False
+		self._fillTransactionMap = {}
 		self._entryOrderFilled = 0   # Number of fills for the entry order
 		
 	async def shutdown(self):
 		logger.info('Shutting down Trading Hub Client.')
 		self._shuttingdown = True
 		self._stopPositionMonitoring()
 
@@ -279,14 +280,15 @@
 						order = LimitOrder('BUY', amount, limitPrice)
 						with Session(get_db_engine()) as session:
 							newTrade = schemas.TradeCreate(account=accountNo, symbol='SPX', strategy=self._currentTemplate.strategy)
 							self._currentTrade = crud.create_trade(session, newTrade)
 							order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + triggeredTemplate.name + ' - Open'
 						order.account = accountNo
 						order.outsideRth = True
+						self._fillTransactionMap.clear()
 						self._entryTrade = ib.placeOrder(self._ironFlyComboContract, order)
 						self._entryTrade.statusEvent += self.onOrderStatusEvent
 						self._entryTradeContract = self._ironFlyComboContract
 						self._ironFlyAskPrice = 0.0
 						self._longLegFillsPrice = 0.0
 						self._longLegFillsReceived = 0
 						self._slShortTrade = None
@@ -406,26 +408,39 @@
 					asyncio.create_task(self._reportExecutedTrade(trade, executedAmount)).add_done_callback(self.optraBot.handleTaskDone)
 				self._entryOrderFilled = self._entryTrade.order.totalQuantity - trade.orderStatus.remaining
 
 		elif trade == self._tpTrade:
 			logger.debug('TP Order Status has been raised. Status: {}', trade.orderStatus.status)
 			if trade.orderStatus.status == OrderStatus.Cancelled:
 				logger.info('TP Order has been cancelled!')
-				self._tpTrade = None
+
 			elif trade.orderStatus.status == OrderStatus.Filled:
 				logger.success('TP Order has been filled. Trade finished')
 				self._tpTrade = None
 				self._slShortTrade = None
 				self._onPositionClose()
 
 		elif trade == self._slShortTrade:
 			logger.debug('SL order for Short Legs status has been changed. Status: {}', trade.orderStatus.status)
 			if trade.orderStatus.status == OrderStatus.Cancelled:
-				logger.info('SL order for Short Legs has been cancelled!')
-				self._slShortTrade = None
+				logEntry: TradeLogEntry = None
+				for logEntry in trade.log:
+					if logEntry.status != 'Cancelled':
+						continue
+				if logEntry == None:
+					logger.error('No log entry found for SL order cancellation!')
+					return
+				if logEntry.errorCode == 201:
+					# 201: Order rejected - reason:Stop price revision is disallowed after order has triggered
+					logger.info('Adjustment of SL order has been rejected, because Stop Order was triggered already.')
+				elif logEntry.errorCode == 0:
+					logger.info('SL Order for Short Legs has been cancelled.')
+				else:
+					logger.error('SL order for Short legs has been cancelled with error code {} and message: {}', logEntry.errorCode, logEntry.message)					
+
 			elif trade.orderStatus.status == OrderStatus.Filled:
 				logger.info('SL order for Short Legs has been filled. Trade finished')
 				logger.info('Now....Long Legs need to be closed if possible')
 				if self._closingLongLegs == False:
 					asyncio.create_task(self._close_long_legs(self._entryTrade.orderStatus.filled, self._currentTemplate.name, self._currentTemplate.account, tradeId=self._currentTrade.id )).add_done_callback(self.optraBot.handleTaskDone)
 					self._onPositionClose()
 
@@ -505,20 +520,47 @@
 			max_transactionid += 1
 			transactionType = ''
 			if fill.execution.side == 'BOT':
 				transactionType = 'BUY'
 			else:
 				transactionType = 'SELL'
 			expirationDate = datetime.strptime(fill.contract.lastTradeDateOrContractMonth, '%Y%m%d')
-			newTransaction = schemas.TransactionCreate(tradeid=tradeId, id=max_transactionid, type=transactionType, sectype=fill.contract.right, timestamp=fill.execution.time, expiration=expirationDate, strike=fill.contract.strike, contracts=fill.execution.shares, price=fill.execution.avgPrice, fee=0, commission=fill.commissionReport.commission, notes='')
+			newTransaction = schemas.TransactionCreate(tradeid=tradeId, id=max_transactionid, type=transactionType, sectype=fill.contract.right, timestamp=fill.execution.time, expiration=expirationDate, strike=fill.contract.strike, contracts=fill.execution.shares, price=fill.execution.avgPrice, fee=0, commission=0, notes='')
+			self._fillTransactionMap[fill.execution.execId] = newTransaction.id # Memorize Execution ID of the fill for later commission report
 			crud.createTransaction(session, newTransaction)
 
 			# Check if trade is closed with all these transactions
 			TradeHelper.updateTrade(dbTrade)
 			session.commit()
+	
+	async def onCommissionReportEvent(self, trade: Trade, fill: Fill, report: CommissionReport):
+		"""
+		Handles the Commission Report Event
+		"""
+		logger.debug('Commission Report order id {} and fill {}', trade.order.orderId, fill)
+		logger.debug('Commission Report: {}', report)
+		tradeId = TradeHelper.getTradeIdFromOrderRef(fill.execution.orderRef)
+		if tradeId == 0:
+			logger.debug('Fill not from OptraBot trade...ignoring it.')
+			return
+		
+		# Get Transaction ID for the fills execution id
+		try:
+			transactionId = self._fillTransactionMap[fill.execution.execId]
+		except KeyError as keyError:
+			logger.error('No trade transaction found for fill execution id {}', fill.execution.execId)
+			return
+		
+		with Session(get_db_engine()) as session:
+			transaction = crud.getTransactionById(session, tradeId, transactionId)
+			if transaction == None:
+				logger.error('Transaction with id {} for trade {} not found in database!', transactionId, tradeId)
+				return
+			transaction.commission = report.commission
+			session.commit()
 
 	async def _reportExecutedTrade(self, trade: Trade, executedAmount: int):
 		"""
 		Report the entry trade execution to Optrabot Hub
 		"""
 		try:
 			executedContracts = 0
@@ -634,24 +676,28 @@
 		self._position = False
 		self._closingLongLegs = False
 		self._currentTemplate = None
 		self._currentTrade = None
 		self._stopPositionMonitoring()
 
 	async def _monitorPosition(self):
-		logger.debug('Monitor position()')
+		logger.debug('Enter Monitor position()')
 		if self._position == False:
 			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
 			#self._positionMonitorTask = None
 			self._stopPositionMonitoring()
 			return
 
 		asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
 
 		ib: IB = self.optraBot['ib']
+		if not ib.isConnected():
+			logger.error('Interactive Brokers is not connected. Unable to monitor position!')
+			return
+		
 		tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
 		longLegsValue = 0
 		currentIronFlyAskPrice = 0
 		currentIronFlyBidPrice = 0
 		adjustedStopLossPrice = None
 		for ticker in tickers:
 			if ticker.contract in self._ironFlyLongLegContracts:
@@ -677,37 +723,77 @@
 					self._ironFlyStopPrice = adjustedStopLossPrice
 					logger.info('Performing stop loss adjustment. New Stop Loss price: {}', self._ironFlyStopPrice)
 			else:
 				logger.debug('Stoploss adjustment has been performed already.')
 		else:
 			logger.debug('No StopLoss adjustment configured.')
 		desiredStopPrice = OptionHelper.roundToTickSize(self._ironFlyStopPrice + longLegsValue)
-		if not self._slShortTrade and self._position == True:
-			logger.error('Caution: Stop Loss order for Short Strikes is missing. Please check in TWS!')
-			return
 		currentStopPrice = OptionHelper.roundToTickSize(self._slShortTrade.order.auxPrice)
 		logger.debug('Long Legs value {} Current Short SL Price: {} Desired Short SL Pice: {}', round(longLegsValue,2), currentStopPrice, desiredStopPrice)
 		openTrades = await ib.reqOpenOrdersAsync()
-		if self._slShortTrade in openTrades and self._slShortTrade.isActive():
-			if currentStopPrice != desiredStopPrice:
-				self._slShortTrade.order.auxPrice = desiredStopPrice
-				logger.info('Adjusting Stop Loss price to ${}', desiredStopPrice)
-				ib.placeOrder(self._slShortTrade.contract, self._slShortTrade.order)
-				logger.debug('Updated SL order with id: {}', self._slShortTrade.order.orderId)
+		if self._slShortTrade in openTrades:
+			if self._slShortTrade.isActive():
+				if currentStopPrice != desiredStopPrice:
+					self._slShortTrade.order.auxPrice = desiredStopPrice
+					logger.info('Adjusting Stop Loss price to ${}', desiredStopPrice)
+					ib.placeOrder(self._slShortTrade.contract, self._slShortTrade.order)
+					logger.debug('Updated SL order with id: {}', self._slShortTrade.order.orderId)
+				else:
+					logger.debug('No adjustment of Stop Loss price required.')
 			else:
-				logger.debug('No adjustment of Stop Loss price required.')
+				logger.debug('SL Order is not active anymore.')
 		else:
-			logger.debug('SL Order is not active anymore.')
+			logger.warning('Caution: Stop Loss order for Short Strikes is missing. Trying to reestablish the Stop Loss order now!')
+			await self._reestablishStopLossOrder(desiredStopPrice)
+		logger.debug('Leave Monitor position()')
 
 	async def _monitorPositionDelayed(self):
 		logger.debug('Waiting 10 seconds for next position monitoring.')
 		await asyncio.sleep(10)
 		if self._position == True:
 			asyncio.create_task(self._monitorPosition(), name='MonitorPosition').add_done_callback(self.optraBot.handleTaskDone)
 
+	async def _reestablishStopLossOrder(self, desiredStopPrice: float):
+		"""
+		Tries to create a new Stop Loss order for the open position based on the given stop price.
+		"""
+		logger.debug('Reestablishing Stop Loss order for Short Legs')
+		ib: IB = self.optraBot['ib']
+		if not ib.isConnected():
+			logger.error('Interactive Brokers is not connected. Unable to monitor position!')
+			return
+		
+		now = datetime.now()
+		ocaGroup = self._currentTemplate.account + '_' + now.strftime('%H%M%S')
+		stopShortsOrder = StopOrder('BUY', self._entryTrade.orderStatus.filled, desiredStopPrice)
+		stopShortsOrder.account = self._currentTemplate.account
+		stopShortsOrder.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - SL Short Legs'
+		stopShortsOrder.ocaGroup = ocaGroup
+		try:
+			self._slShortTrade = ib.placeOrder(self._ironFlyShortComboContract, stopShortsOrder)
+			self._slShortTrade.statusEvent += self.onOrderStatusEvent
+		except Exception as excp:
+			logger('Exception beim Erstellen der Short Leg Stoploss order')
+		logger.info('Stop Loss order for Short Legs has been reestablished.')
+
+		# Check if Take Profit Order is still in place and recreate it, if it's missing
+		openTrades = await ib.reqOpenOrdersAsync()
+		if self._tpTrade in openTrades:
+			logger.info('Take Profit order is still in place.')
+		else:
+			logger.warning('Take Profit order is missing. Trying to reestablish the Take Profit order now!')
+			order = LimitOrder('SELL', self._tpTrade.order.totalQuantity, self._tpTrade.order.lmtPrice)
+			order.account = self._currentTemplate.account
+			order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - Take Profit'
+			order.ocaGroup = ocaGroup
+			order.outsideRth = True
+			self._tpTrade = ib.placeOrder(self._ironFlyComboContract, order)
+			logger.debug('Created TP order with id: {}', self._tpTrade.order.orderId)
+			self._tpTrade.statusEvent += self.onOrderStatusEvent
+
 	def _meetsMinimumPremium(self, premium: float) -> bool:
 		""" Checks if given premium meets minimum premium
 
 		Parameters
 		----------
 		premium : float
 			As premium is a typically a credit, a negative number is expected.
```

### Comparing `optrabot-0.8.2a3/pyproject.toml` & `optrabot-0.9.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.8.2a3"
+version = "0.9.0a0"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
```

### Comparing `optrabot-0.8.2a3/PKG-INFO` & `optrabot-0.9.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.8.2a3
+Version: 0.9.0a0
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

