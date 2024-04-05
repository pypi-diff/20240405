# Comparing `tmp/optrabot-0.8.0a0.tar.gz` & `tmp/optrabot-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.8.0a0.tar", max compression
+gzip compressed data, was "optrabot-0.8.1a0.tar", max compression
```

## Comparing `optrabot-0.8.0a0.tar` & `optrabot-0.8.1a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.0a0/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.0a0/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.0a0/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.0a0/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.0a0/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.0a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.0a0/optrabot/alembic.ini
--rw-r--r--   0        0        0    11822 2024-03-29 23:00:56.372952 optrabot-0.8.0a0/optrabot/config.py
--rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.0a0/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.0a0/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-02-22 12:22:44.565504 optrabot-0.8.0a0/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.0a0/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.0a0/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.0a0/optrabot/optionhelper.py
--rw-r--r--   0        0        0     9791 2024-03-29 23:03:25.087211 optrabot-0.8.0a0/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.0a0/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.0a0/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.0a0/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.0a0/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.0a0/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.0a0/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.0a0/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.0a0/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.0a0/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    34410 2024-03-29 23:03:25.087913 optrabot-0.8.0a0/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      821 2024-03-29 23:07:03.283625 optrabot-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.1a0/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.1a0/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.1a0/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.1a0/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.1a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.1a0/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11822 2024-03-29 23:18:40.612397 optrabot-0.8.1a0/optrabot/config.py
+-rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.1a0/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.1a0/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-02-22 12:22:44.565504 optrabot-0.8.1a0/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.1a0/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.1a0/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.1a0/optrabot/optionhelper.py
+-rw-r--r--   0        0        0     9791 2024-04-05 07:43:33.069681 optrabot-0.8.1a0/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.1a0/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.1a0/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.1a0/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.1a0/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.1a0/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.1a0/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.1a0/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.1a0/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.1a0/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    35316 2024-04-05 07:43:42.185859 optrabot-0.8.1a0/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      821 2024-04-05 07:45:05.901663 optrabot-0.8.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.8.1a0/PKG-INFO
```

### Comparing `optrabot-0.8.0a0/README.md` & `optrabot-0.8.1a0/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/alembic/env.py` & `optrabot-0.8.1a0/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/alembic/script.py.mako` & `optrabot-0.8.1a0/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.8.1a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/alembic.ini` & `optrabot-0.8.1a0/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/config.py` & `optrabot-0.8.1a0/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/crud.py` & `optrabot-0.8.1a0/optrabot/crud.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/database.py` & `optrabot-0.8.1a0/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/main.py` & `optrabot-0.8.1a0/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/marketdatatype.py` & `optrabot-0.8.1a0/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/models.py` & `optrabot-0.8.1a0/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/optionhelper.py` & `optrabot-0.8.1a0/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/optrabot.py` & `optrabot-0.8.1a0/optrabot/optrabot.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/schemas.py` & `optrabot-0.8.1a0/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/stoplossadjuster.py` & `optrabot-0.8.1a0/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/tradehelper.py` & `optrabot-0.8.1a0/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/tradetemplate/template.py` & `optrabot-0.8.1a0/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.8.1a0/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.8.1a0/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.0a0/optrabot/tradinghubclient.py` & `optrabot-0.8.1a0/optrabot/tradinghubclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,84 +242,54 @@
 						await self._scheduleNextPoll()
 						return
 					if longCallContract.strike != longCallStrike:
 						logger.warning('Using different Long Call strike {}, because of existing open orders on desired strike {}.', longCallContract.strike, longCallStrike)
 
 					self._ironFlyLongLegContracts = [longCallContract, longPutContract]
 					self._ironFlyContracts = [shortPutContract, shortCallContract, longPutContract, longCallContract]
-					ironFlyComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD',
-						comboLegs=[]
-					)
-
+					self._ironFlyComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD', comboLegs=[])
 					self._ironFlyShortComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD', comboLegs=[])
 
-					ironFlyMidPrice = 0.0
-					tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
-					for ticker in tickers:
-						tickerContract = ticker.contract
-						if tickerContract.conId == shortPutContract.conId:
-							midPrice = (ticker.ask + ticker.bid) / 2
-							if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
-								midPrice = 100
-							ironFlyMidPrice -= midPrice
-							if not util.isNan(ticker.bid):
-								self._ironFlyAskPrice -= ticker.bid
-							ironFlyComboContract.comboLegs.append(ComboLeg(conId=shortPutContract.conId, ratio=1, action='SELL', exchange='SMART'))
-							self._ironFlyShortComboContract.comboLegs.append(ComboLeg(conId=shortPutContract.conId, ratio=1, action='BUY', exchange='SMART'))
-						if tickerContract.conId == shortCallContract.conId:
-							midPrice = (ticker.ask + ticker.bid) / 2
-							if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
-								midPrice = 100
-							ironFlyMidPrice -= midPrice
-							if not util.isNan(ticker.bid):
-								self._ironFlyAskPrice -= ticker.bid
-							ironFlyComboContract.comboLegs.append(ComboLeg(conId=shortCallContract.conId, ratio=1, action='SELL', exchange='SMART'))
-							self._ironFlyShortComboContract.comboLegs.append(ComboLeg(conId=shortCallContract.conId, ratio=1, action='BUY', exchange='SMART'))
-						if tickerContract.conId == longPutContract.conId:
-							midPrice = (ticker.ask + ticker.bid) / 2
-							if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
-								midPrice = 0.05
-							ironFlyMidPrice += midPrice
-							if not util.isNan(ticker.ask):
-								self._ironFlyAskPrice += ticker.ask
-							ironFlyComboContract.comboLegs.append(ComboLeg(conId=longPutContract.conId, ratio=1, action='BUY', exchange='SMART'))
-						if tickerContract.conId == longCallContract.conId:
-							midPrice = (ticker.ask + ticker.bid) / 2
-							if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
-								midPrice = 0.05
-							ironFlyMidPrice += midPrice
-							if not util.isNan(ticker.ask):
-								self._ironFlyAskPrice += ticker.ask
-							ironFlyComboContract.comboLegs.append(ComboLeg(conId=longCallContract.conId, ratio=1, action='BUY', exchange='SMART'))
-
-					logger.debug("Tickers {}", tickers)
-					ticker = tickers[0]
-					if util.isNan(ironFlyMidPrice):
+					ironFlyMidPrice = None
+					for i in range(5):
+						tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
+						logger.debug("Tickers {}", tickers)
+						ironFlyMidPrice = self._calculateIronFlyMidPrice(tickers, ironFlyComboContract=self._ironFlyComboContract, 
+													   ironFlyShortComboContract=self._ironFlyShortComboContract, 
+													   shortPutContract=shortPutContract,
+													   shortCallContract=shortCallContract,
+													   longPutContract=longPutContract,
+													   longCallContract=longCallContract)
+						if ironFlyMidPrice != None:
+							break
+						await asyncio.sleep(1)
+					
+					#if util.isNan(ironFlyMidPrice):
+					if ironFlyMidPrice == None:
 						logger.error("No Mid Price for combo could be calculated!")
 						await self._scheduleNextPoll()
 						return
 
-					limitPrice = OptionHelper.roundToTickSize(ironFlyMidPrice)
+					limitPrice = ironFlyMidPrice
 
 					logger.info("IronFly Combo Mid Price: {} Ask Price: {}", ironFlyMidPrice, self._ironFlyAskPrice)
 
 					if not self._meetsMinimumPremium(limitPrice):
 						logger.info('Premium below configured minimum premium of ${}. Trade is not executed!', self._currentTemplate.minPremium)
 					else:
 						order = LimitOrder('BUY', amount, limitPrice)
 						with Session(get_db_engine()) as session:
 							newTrade = schemas.TradeCreate(account=accountNo, symbol='SPX', strategy=self._currentTemplate.strategy)
 							self._currentTrade = crud.create_trade(session, newTrade)
 							order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + triggeredTemplate.name + ' - Open'
 						order.account = accountNo
 						order.outsideRth = True
-						self._entryTrade = ib.placeOrder(ironFlyComboContract, order)
+						self._entryTrade = ib.placeOrder(self._ironFlyComboContract, order)
 						self._entryTrade.statusEvent += self.onOrderStatusEvent
-						self._entryTradeContract = ironFlyComboContract
-						self._ironFlyComboContract = ironFlyComboContract
+						self._entryTradeContract = self._ironFlyComboContract
 						self._ironFlyAskPrice = 0.0
 						self._longLegFillsPrice = 0.0
 						self._longLegFillsReceived = 0
 						self._slShortTrade = None
 						self._tpTrade = None
 						self._entryOrderFilled = 0
 						self._closingLongLegs = False
@@ -330,14 +300,61 @@
 						logger.error("Exception: {}", excp)
 
 		except Exception as anyEcxp:
 			logger.error("Exception occured during poll: {}", anyEcxp)
 
 		await self._scheduleNextPoll()
 
+	def _calculateIronFlyMidPrice(self, tickers: List[Ticker], ironFlyComboContract: Contract, ironFlyShortComboContract: Contract, shortPutContract: Option, shortCallContract: Option, longPutContract: Option, longCallContract: Option) -> float:
+		"""
+		Calculate the Iron Fly Mid Price based on the given tickers. It returns
+		None if one of the legs got no valid price.
+		"""
+		ironFlyMidPrice = 0
+		self._ironFlyAskPrice = 0
+		ironFlyComboContract.comboLegs.clear()
+		ironFlyShortComboContract.comboLegs.clear()
+		for ticker in tickers:
+			tickerContract = ticker.contract
+			if tickerContract.conId == shortPutContract.conId:
+				midPrice = (ticker.ask + ticker.bid) / 2
+				if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
+					return None
+				ironFlyMidPrice -= midPrice
+				if not util.isNan(ticker.bid):
+					self._ironFlyAskPrice -= ticker.bid
+					ironFlyComboContract.comboLegs.append(ComboLeg(conId=shortPutContract.conId, ratio=1, action='SELL', exchange='SMART'))
+					ironFlyShortComboContract.comboLegs.append(ComboLeg(conId=shortPutContract.conId, ratio=1, action='BUY', exchange='SMART'))
+			if tickerContract.conId == shortCallContract.conId:
+				midPrice = (ticker.ask + ticker.bid) / 2
+				if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
+					return None
+				ironFlyMidPrice -= midPrice
+				if not util.isNan(ticker.bid):
+					self._ironFlyAskPrice -= ticker.bid
+					ironFlyComboContract.comboLegs.append(ComboLeg(conId=shortCallContract.conId, ratio=1, action='SELL', exchange='SMART'))
+					ironFlyShortComboContract.comboLegs.append(ComboLeg(conId=shortCallContract.conId, ratio=1, action='BUY', exchange='SMART'))
+			if tickerContract.conId == longPutContract.conId:
+				midPrice = (ticker.ask + ticker.bid) / 2
+				if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
+					midPrice = 0.05
+				ironFlyMidPrice += midPrice
+				if not util.isNan(ticker.ask):
+					self._ironFlyAskPrice += ticker.ask
+					ironFlyComboContract.comboLegs.append(ComboLeg(conId=longPutContract.conId, ratio=1, action='BUY', exchange='SMART'))
+			if tickerContract.conId == longCallContract.conId:
+				midPrice = (ticker.ask + ticker.bid) / 2
+				if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
+					midPrice = 0.05
+				ironFlyMidPrice += midPrice
+				if not util.isNan(ticker.ask):
+					self._ironFlyAskPrice += ticker.ask
+					ironFlyComboContract.comboLegs.append(ComboLeg(conId=longCallContract.conId, ratio=1, action='BUY', exchange='SMART'))
+		return OptionHelper.roundToTickSize(ironFlyMidPrice)
+
 	async def _trackEntryOrder(self):
 		await asyncio.sleep(5) # Wait 5 seconds for order Execution
 		ib: IB = self.optraBot['ib']
 		if self._entryTrade == None:
 			return
 		
 		if self._entryTrade.orderStatus.status == OrderStatus.Cancelled or self._entryTrade.orderStatus.status == OrderStatus.Inactive:
@@ -381,15 +398,16 @@
 					logger.debug('Additionally fill quantity (Qty: {}) for the entry order...depending orders need to be adjusted.', trade.orderStatus.filled)
 					asyncio.create_task(self._adjustTakeProfitAndStop(trade)).add_done_callback(self.optraBot.handleTaskDone)
 
 				if trade.orderStatus.remaining > 0:
 					logger.warning('Partial fill for entry order. Remaining: {}', trade.orderStatus.remaining)
 				executedAmount = trade.orderStatus.filled - self._entryOrderFilled
 				logger.debug('Executed amount for entry trade: {}', executedAmount)
-				asyncio.create_task(self._reportExecutedTrade(trade, executedAmount)).add_done_callback(self.optraBot.handleTaskDone)
+				if executedAmount > 0:
+					asyncio.create_task(self._reportExecutedTrade(trade, executedAmount)).add_done_callback(self.optraBot.handleTaskDone)
 				self._entryOrderFilled = self._entryTrade.order.totalQuantity - trade.orderStatus.remaining
 
 		elif trade == self._tpTrade:
 			logger.debug('TP Order Status has been raised. Status: {}', trade.orderStatus.status)
 			if trade.orderStatus.status == OrderStatus.Cancelled:
 				logger.info('TP Order has been cancelled!')
 				self._tpTrade = None
```

### Comparing `optrabot-0.8.0a0/pyproject.toml` & `optrabot-0.8.1a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.8.0a0"
+version = "0.8.1a0"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
```

### Comparing `optrabot-0.8.0a0/PKG-INFO` & `optrabot-0.8.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.8.0a0
+Version: 0.8.1a0
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

