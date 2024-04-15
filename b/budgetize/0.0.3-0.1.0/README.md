# Comparing `tmp/budgetize-0.0.3.tar.gz` & `tmp/budgetize-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "budgetize-0.1.0.tar", max compression
```

## Comparing `budgetize-0.0.3.tar` & `budgetize-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 budgetize-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 budgetize-0.0.3/Pipfile
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 budgetize-0.0.3/main.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 budgetize-0.0.3/mypy.ini
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 budgetize-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/__main__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/_currency_manager.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/_entry_point.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/consts.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/__init__.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/_database.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/orm/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/orm/_account.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/orm/_account_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/orm/_base.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/db/orm/_transactions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/tui_app.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/modals/__init__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/modals/_confirm_quit.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/modals/_transaction_details.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/modals/css/confirm_quit.tcss
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/modals/css/transaction_details.tcss
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/_add_transaction.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/_create_account.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/_initial_config.py
--rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/_main_menu.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/_manage_accounts.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/_startup.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/css/create_account.tcss
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/css/initial_config.tcss
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/css/main_menu.tcss
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 budgetize-0.0.3/budgetize/tui/screens/css/startup.tcss
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 budgetize-0.0.3/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 budgetize-0.0.3/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 budgetize-0.0.3/LICENSE
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 budgetize-0.0.3/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 budgetize-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 budgetize-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      160 2024-04-15 02:44:25.935559 budgetize-0.1.0/budgetize/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-12 15:46:05.277708 budgetize-0.1.0/budgetize/__main__.py
+-rw-r--r--   0        0        0      152 2024-04-15 02:44:25.936559 budgetize-0.1.0/budgetize/console.py
+-rw-r--r--   0        0        0     7103 2024-04-15 02:44:25.937559 budgetize-0.1.0/budgetize/consts.py
+-rw-r--r--   0        0        0    12200 2024-04-15 02:44:25.938560 budgetize-0.1.0/budgetize/currency_manager.py
+-rw-r--r--   0        0        0    13135 2024-04-15 02:44:25.939559 budgetize-0.1.0/budgetize/db/database.py
+-rw-r--r--   0        0        0      192 2024-01-13 20:02:45.319258 budgetize-0.1.0/budgetize/db/orm/_base.py
+-rw-r--r--   0        0        0      603 2024-04-15 02:44:25.940559 budgetize-0.1.0/budgetize/db/orm/account.py
+-rw-r--r--   0        0        0     1235 2024-04-15 02:44:25.941559 budgetize-0.1.0/budgetize/db/orm/transactions.py
+-rw-r--r--   0        0        0      215 2024-04-15 02:44:25.942560 budgetize-0.1.0/budgetize/exceptions.py
+-rw-r--r--   0        0        0     3196 2024-04-15 02:44:25.943560 budgetize-0.1.0/budgetize/settings_manager.py
+-rw-r--r--   0        0        0    15437 2024-04-15 02:44:25.947560 budgetize-0.1.0/budgetize/translations/es/es.po
+-rw-r--r--   0        0        0     7913 2024-04-15 02:44:25.946561 budgetize-0.1.0/budgetize/translations/es/LC_MESSAGES/budgetize.mo
+-rw-r--r--   0        0        0    11725 2024-04-15 02:44:25.944561 budgetize-0.1.0/budgetize/translations/TRANSLATION_TEMPLATE.po
+-rw-r--r--   0        0        0       58 2024-01-13 20:17:48.972282 budgetize-0.1.0/budgetize/tui/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-15 02:44:25.949561 budgetize-0.1.0/budgetize/tui/modals/categories_modal.py
+-rw-r--r--   0        0        0     1077 2024-04-15 02:44:25.949561 budgetize-0.1.0/budgetize/tui/modals/confirm_quit.py
+-rw-r--r--   0        0        0      231 2024-04-15 02:44:25.951562 budgetize-0.1.0/budgetize/tui/modals/css/confirm_quit.tcss
+-rw-r--r--   0        0        0      180 2024-04-15 02:44:25.952563 budgetize-0.1.0/budgetize/tui/modals/css/error_modal.tcss
+-rw-r--r--   0        0        0      207 2024-04-15 02:44:25.952563 budgetize-0.1.0/budgetize/tui/modals/css/input_modal.tcss
+-rw-r--r--   0        0        0      175 2024-03-06 00:21:46.072627 budgetize-0.1.0/budgetize/tui/modals/css/transaction_details.tcss
+-rw-r--r--   0        0        0     1769 2024-04-15 02:44:25.954562 budgetize-0.1.0/budgetize/tui/modals/error_modal.py
+-rw-r--r--   0        0        0     3492 2024-04-15 02:44:25.955565 budgetize-0.1.0/budgetize/tui/modals/input_modal.py
+-rw-r--r--   0        0        0     3101 2024-04-15 02:44:25.956563 budgetize-0.1.0/budgetize/tui/modals/transaction_details.py
+-rw-r--r--   0        0        0     6594 2024-04-15 02:44:25.958563 budgetize-0.1.0/budgetize/tui/screens/add_transaction.py
+-rw-r--r--   0        0        0     4088 2024-04-15 02:44:25.959564 budgetize-0.1.0/budgetize/tui/screens/create_account.py
+-rw-r--r--   0        0        0      146 2024-01-14 23:18:00.878680 budgetize-0.1.0/budgetize/tui/screens/css/create_account.tcss
+-rw-r--r--   0        0        0        0 2024-01-11 16:15:44.882149 budgetize-0.1.0/budgetize/tui/screens/css/initial_config.tcss
+-rw-r--r--   0        0        0      160 2024-04-15 02:44:25.960565 budgetize-0.1.0/budgetize/tui/screens/css/main_menu.tcss
+-rw-r--r--   0        0        0      188 2024-04-15 02:44:25.961564 budgetize-0.1.0/budgetize/tui/screens/css/transfer.tcss
+-rw-r--r--   0        0        0     3217 2024-04-15 02:44:25.962564 budgetize-0.1.0/budgetize/tui/screens/initial_config.py
+-rw-r--r--   0        0        0    19698 2024-04-15 02:44:25.963564 budgetize-0.1.0/budgetize/tui/screens/main_menu.py
+-rw-r--r--   0        0        0     5434 2024-04-15 02:44:25.964566 budgetize-0.1.0/budgetize/tui/screens/manage_accounts.py
+-rw-r--r--   0        0        0     3368 2024-04-15 02:44:25.966565 budgetize-0.1.0/budgetize/tui/screens/settings.py
+-rw-r--r--   0        0        0    10622 2024-04-15 02:44:25.967565 budgetize-0.1.0/budgetize/tui/screens/transfer.py
+-rw-r--r--   0        0        0     1510 2024-04-15 02:44:25.968566 budgetize-0.1.0/budgetize/tui/tui_app.py
+-rw-r--r--   0        0        0     1194 2024-04-15 02:44:25.969566 budgetize-0.1.0/budgetize/utils.py
+-rw-r--r--   0        0        0    35823 2024-01-13 20:50:14.408983 budgetize-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1273 2024-04-15 02:44:25.976567 budgetize-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2351 2024-04-15 02:44:25.934559 budgetize-0.1.0/README.md
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 budgetize-0.1.0/PKG-INFO
```

### Comparing `budgetize-0.0.3/budgetize/db/_database.py` & `budgetize-0.1.0/budgetize/db/database.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,233 @@
 """Definition of Database class that handles database operations"""
 
-from typing import Iterator
+from typing import Iterator, Optional
 
 from arrow import Arrow
 from sqlalchemy import create_engine, select, update
 from sqlalchemy.orm import Session
 from textual.app import App
 
+from budgetize import CurrencyManager, SettingsManager
 from budgetize.consts import PROD_DB_URL
-
-from .orm import Account, Base, Transaction
+from budgetize.db.orm._base import Base
+from budgetize.db.orm.account import Account
+from budgetize.db.orm.transactions import Transaction
 
 
 class Database:
-    """Class that handles database operations"""
+    """This class is the API for interacting with the database.
+    All read and writes are done here which may include utilities for converting currencies, for example.
+    """
 
     engine = create_engine(PROD_DB_URL)
 
-    def __init__(self, app: App):
-        if app is None:
-            return
+    def __init__(self, app: Optional[App] = None):
+        """Initializes a Database instance.
 
-        Database.engine = create_engine(
-            PROD_DB_URL
-            if not "devtools" in app.features
-            else "sqlite:///test_db.sqlite"
-        )
+        Args:
+            app (App): The application instance.
+        """
+        if app is None:
+            Database.engine = create_engine("sqlite:///test_db.sqlite")
+        else:
+            Database.engine = create_engine(
+                PROD_DB_URL
+                if not "devtools" in app.features
+                else "sqlite:///test_db.sqlite"
+            )
         Base.metadata.create_all(self.engine)
+        self.settings = SettingsManager()
 
     def get_transactions_from_account(self, account_id: int) -> Iterator[Transaction]:
-        """Returns an iterator of transactions from the specified account"""
+        """Returns an iterator of transactions from the specified account.
+
+        Args:
+            account_id (int): The ID of the account.
+
+        Yields:
+            Transaction: A transaction from the specified account.
+        """
         stmt = select(Transaction).where(Transaction.account_id == account_id)
 
         with Session(Database.engine) as session:
             for transaction in session.scalars(stmt):
                 yield transaction
 
     def get_monthly_transactions_from_account(
         self, account_id: int, month: str, year: str
     ) -> Iterator[Transaction]:
-        """
-        Returns an iterator of transactions from
-        the specified account within the specified month and year
+        """Returns an iterator of transactions from the specified account within the specified month and year.
+
+        Args:
+            account_id (int): The ID of the account.
+            month (str): The month in format 'MM'.
+            year (str): The year in format 'YYYY'.
+
+        Yields:
+            Transaction: A transaction from the specified account within the specified month and year.
         """
         transactions = self.get_transactions_from_account(account_id)
 
         # Filter transactions by month and year
         for transaction in transactions:
             date = Arrow.fromtimestamp(transaction.timestamp)
-            ar = Arrow.fromtimestamp(transaction.timestamp)
-            print("===================================")
-            print(f"Date for transaction #{transaction.id}: {ar.format('M/D/YYYY')}")
-
-            print(f"Ar m/y: {ar.format('M')} | {ar.format('YYYY')}")
-            print(f"Received: {month} | {year}")
 
             if date.format("M") == month and date.format("YYYY") == year:
                 yield transaction
 
     def get_accounts(self) -> Iterator[Account]:
-        """Returns an iterator of all accounts"""
+        """Returns an iterator of all accounts.
+
+        Yields:
+            Account: An account from the database.
+        """
         stmt = select(Account)
 
         with Session(Database.engine) as session:
             for account in session.scalars(stmt):
                 yield account
 
     def get_account_by_id(self, account_id: int) -> Account:
-        """Returns the account with the specified id"""
+        """Returns the account with the specified ID.
+
+        Args:
+            account_id (int): The ID of the account.
 
+        Returns:
+            Account: The account with the specified ID.
+        """
         with Session(Database.engine) as session:
             found_account: Account = session.get_one(Account, account_id)
             return found_account
 
+    def get_account_by_name(self, name: str) -> Account:
+        """Returns the account with the specified name.
+
+        Args:
+            name (str): The name of the account.
+
+        Returns:
+            Account: The account with the specified name.
+        """
+        with Session(Database.engine) as session:
+            stmt = select(Account).where(Account.name == name)
+            account: Account = session.execute(stmt).scalars().first()  # type:ignore
+            return account
+
+    def account_name_exists(self, name: str) -> bool:
+        """Returns True if an account with the specified name exists, False otherwise.
+
+        Args:
+            name (str): The name of the account.
+
+        Returns:
+            bool: True if an account with the specified name exists, False otherwise.
+        """
+        with Session(Database.engine) as session:
+            stmt = select(Account).where(Account.name == name)
+            account = session.execute(stmt).scalars().first()
+            return account is not None
+
     def get_transaction_by_id(self, transaction_id: int) -> Transaction:
-        """Returns the transaction with the specified id"""
+        """Returns the transaction with the specified ID.
+
+        Args:
+            transaction_id (int): The ID of the transaction.
 
+        Returns:
+            Transaction: The transaction with the specified ID.
+        """
         with Session(Database.engine) as session:
             found_transaction: Transaction = session.get_one(
                 Transaction, transaction_id
             )
             return found_transaction
 
-    def add_account(self, account: Account) -> None:
-        """Adds a new account to the user"""
+    def add_account(
+        self,
+        name: str,
+        currency: str,
+        starting_balance: float,
+    ) -> None:
+        """Adds a new account to the user.
+
+        Args:
+            name (str): The name of the account.
+            currency (str): The currency of the account.
+            starting_balance (float): The starting balance of the account.
+            account_type_name (str): The type of the account.
+        """
+
         with Session(Database.engine) as session:
-            session.add(account)
+            new_account = Account(name=name, currency=currency)
+            session.add(new_account)
+            session.commit()
+
+            initial_balance_transaction = Transaction(
+                account_id=new_account.id,
+                amount=starting_balance,
+                description="Initial balance",
+                category="-",
+                timestamp=Arrow.now().timestamp(),
+                visible=False,
+            )
+            session.add(initial_balance_transaction)
             session.commit()
 
     def add_transaction(
         self,
         account_id: int,
         amount: float,
         description: str,
         category: str,
         timestamp: float,
+        visible: bool = True,
     ) -> None:
-        """Registers a new transaction"""
+        """Registers a new transaction.
 
+        Args:
+            account_id (int): The ID of the account.
+            amount (float): The amount of the transaction.
+            description (str): The description of the transaction.
+            category (str): The category of the transaction.
+            timestamp (float): The timestamp of the transaction.
+        """
         transaction = Transaction(
             account_id=account_id,
             amount=amount,
             description=description,
             category=category,
             timestamp=timestamp,
+            visible=visible,
         )
 
         with Session(Database.engine) as session:
             session.add(transaction)
-
-            # Update the account balance
-            account = session.get_one(Account, account_id)
-            account.balance += float(amount)
             session.commit()
 
     def update_transaction(
         self,
         transaction_id: int,
         account_id: int,
         amount: float,
         description: str,
         category: str,
         timestamp: float,
     ) -> None:
-        """Updates the specified transaction in the database"""
+        """Updates the specified transaction in the database.
 
+        Args:
+            transaction_id (int): The ID of the transaction to update.
+            account_id (int): The ID of the account.
+            amount (float): The new amount of the transaction.
+            description (str): The new description of the transaction.
+            category (str): The new category of the transaction.
+            timestamp (float): The new timestamp of the transaction.
+        """
         values = {
             "account_id": account_id,
             "amount": amount,
             "description": description,
             "category": category,
             "timestamp": timestamp,
         }
@@ -139,80 +238,136 @@
                 .values(values)
                 .where(Transaction.id == transaction_id)
             )
             session.execute(upd)
             session.commit()
 
     def get_all_recent_transactions(self) -> list[Transaction]:
-        """Returns a list with the last 5 transactions saved across all accounts."""
+        """Returns a list with the last 5 transactions saved across all accounts.
 
+        Returns:
+            list[Transaction]: A list of recent transactions.
+        """
         with Session(Database.engine) as session:
-            stmt = select(Transaction).order_by(Transaction.timestamp.desc()).limit(5)
+            stmt = (
+                select(Transaction)
+                .where(Transaction.visible == True)
+                .order_by(Transaction.timestamp.desc())
+                .limit(5)
+            )
             transactions: list[Transaction] = session.execute(stmt).scalars().all()  # type: ignore
             return transactions
 
-    def get_monthly_income(self) -> float:
-        """Returns the total income for the current month"""
+    def get_account_balance(self, account_id: int) -> float:
+        """Returns the balance of the specified account.
+
+        Args:
+            account_id (int): The ID of the account.
+
+        Returns:
+            float: The balance of the account.
+        """
+
+        stmt = select(Transaction).where(Transaction.account_id == account_id)
+        with Session(Database.engine) as session:
+            transactions = session.execute(stmt).scalars().all()
+
+            balance = 0.0
+            for transaction in transactions:
+                balance += transaction.amount
+
+            return balance
 
+    async def get_monthly_income(self) -> float:
+        """(Coroutine) Returns the total income for the current month.
+
+        Returns:
+            float: The total income for the current month.
+        """
         now = Arrow.now()
 
         income = 0.0
         for account in self.get_accounts():
+
+            exchange_rate = 1.0
+            if account.currency != self.settings.get_base_currency():
+                exchange_rate = await CurrencyManager(
+                    self.settings.get_base_currency()
+                ).get_exchange(account.currency)
+
             for transaction in self.get_monthly_transactions_from_account(
                 account.id, now.format("M"), now.format("YYYY")
             ):
-                if transaction.amount > 0:
-                    income += transaction.amount
+                if transaction.amount > 0 and transaction.visible:
+                    income += transaction.amount / exchange_rate
 
-        return income
+        return round(income, 2)
 
     def delete_account(self, account_id: int) -> None:
-        """Deletes the specified account from the database."""
+        """Deletes the specified account from the database.
+
+        Args:
+            account_id (int): The ID of the account to delete.
+        """
         stmt = select(Account).where(Account.id == account_id)
 
         with Session(Database.engine) as session:
             res = session.execute(stmt)
 
             row = res.fetchone()
             if row is None:
                 return
 
-            acc = row.tuple()[0]
-            session.delete(acc)
+            account = row.tuple()[0]
+            session.delete(account)
 
             # Delete transactions from the account
-
             transaction_stmt = select(Transaction).where(
                 Transaction.account_id == account_id
             )
-            rows = session.execute(transaction_stmt).fetchall()
+            transaction_rows = session.execute(transaction_stmt).fetchall()
 
-            for row in rows:
-                transaction = row.tuple()[0]
-                session.delete(transaction)
+            for transaction in transaction_rows:
+                transaction_obj = transaction.tuple()[0]
+                session.delete(transaction_obj)
 
             session.commit()
 
-    def get_monthly_expense(self) -> float:
-        """Returns the total expenses for the current month"""
+    async def get_monthly_expense(self) -> float:
+        """(Coroutine) Returns the total expenses for the current month.
+
+        Returns:
+            float: The total expenses for the current month.
+        """
         now = Arrow.now()
 
         expense = 0.0
         for account in self.get_accounts():
+            rate = 1.0
+            if account.currency != self.settings.get_base_currency():
+                rate = await CurrencyManager(
+                    self.settings.get_base_currency()
+                ).get_exchange(account.currency)
             for transaction in self.get_monthly_transactions_from_account(
                 account.id, now.format("M"), now.format("YYYY")
             ):
-                if transaction.amount < 0:
-                    expense += transaction.amount
+                if transaction.amount < 0 and transaction.visible:
+                    expense += transaction.amount / rate
 
-        return expense
+        return round(expense, 2)
 
     def delete_transaction(self, transaction_id: int) -> Transaction:
-        """Deletes the specified transaction from the DB and returns it."""
+        """Deletes the specified transaction from the DB and returns it.
+
+        Args:
+            transaction_id (int): The ID of the transaction to delete.
 
+        Returns:
+            Transaction: The deleted transaction.
+        """
         stmt = select(Transaction).where(Transaction.id == transaction_id)
         with Session(Database.engine) as session:
             res = session.execute(stmt)
             row = res.fetchone()
 
             selected_transaction: Transaction = row.tuple()[0]  # type: ignore
             session.delete(selected_transaction)
```

### Comparing `budgetize-0.0.3/budgetize/db/orm/_transactions.py` & `budgetize-0.1.0/budgetize/db/orm/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 
 
 class Transaction(Base):  # pylint: disable=too-few-public-methods
     """Database ORM for transactions table. Represents a transaction on an account."""
 
     __tablename__ = "transactions"
 
-    id: Mapped[int] = mapped_column(primary_key=True, nullable=False)
+    id: Mapped[int] = mapped_column(primary_key=True)
     account_id: Mapped[Optional[str]] = mapped_column(ForeignKey("accounts.id"))
     amount: Mapped[float]
     description: Mapped[Optional[str]] = mapped_column(String(255))
     category: Mapped[str]
     timestamp: Mapped[float]
 
+    # If its visible it will contribute to balance and expenses. If not, its an hidden expense. For example the initial balance or transfers
+    visible: Mapped[bool] = mapped_column(default=True)
+
     def __repr__(self) -> str:
         """String representation of the Transaction object."""
 
         return f"""<Transaction(
         id={self.id}, 
         account_id={self.account_id}, 
         amount={self.amount},
```

### Comparing `budgetize-0.0.3/budgetize/tui/modals/_confirm_quit.py` & `budgetize-0.1.0/budgetize/tui/modals/confirm_quit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """Module that defines the ConfirmQuit modal"""
 
 from textual.app import ComposeResult
 from textual.containers import Center, Horizontal
 from textual.screen import ModalScreen
 from textual.widgets import Button, Label
 
+from budgetize.utils import _
+
 
 class ConfirmQuit(ModalScreen):
     """Modal that shows up when user is trying to quit the app."""
 
     CSS_PATH = "css/confirm_quit.tcss"
 
     def compose(self) -> ComposeResult:
         """Called when screen is composed"""
 
         yield Center(
-            Label("Are you sure you want to quit?", id="question"),
+            Label(_("Are you sure you want to quit?"), id="question"),
             Horizontal(
-                Button.error("Yes", id="yes-button"),
-                Button("No", id="no-button", variant="primary"),
+                Button.error(_("Exit"), id="yes-button"),
+                Button(_("Cancel"), id="no-button", variant="primary"),
+                id="horizontal-container",
             ),
             id="dialog",
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Called when a button is pressed"""
```

### Comparing `budgetize-0.0.3/budgetize/tui/modals/_transaction_details.py` & `budgetize-0.1.0/budgetize/tui/modals/transaction_details.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from arrow import Arrow
 from textual.app import ComposeResult
 from textual.containers import Center, Horizontal
 from textual.screen import ModalScreen
 from textual.widgets import Button, Label
 
-from budgetize.db import Database
-from budgetize.db.orm import Transaction
-from budgetize.tui.screens import AddTransaction
+from budgetize.db.database import Database
+from budgetize.tui.screens.add_transaction import AddTransaction
+from budgetize.utils import _
 
 
 class TransactionDetails(ModalScreen):
     """Modal screen for displaying transaction details."""
 
     DB: Database = None  # type: ignore
     CSS_PATH = "css/transaction_details.tcss"
@@ -20,30 +20,47 @@
         TransactionDetails.DB = Database(self.app)
         self.transaction = self.DB.get_transaction_by_id(transaction_id)
         self.from_manage_accounts = from_manage_accounts
 
         super().__init__()
 
     def compose(self) -> ComposeResult:
+
+        if self.transaction.account_id is None:
+            raise RuntimeError("Transaction must have an account_id")
+
         """Called when modal needs to be composed."""
         date_str = Arrow.fromtimestamp(self.transaction.timestamp).format("MM/DD/YYYY")
 
         with Center(id="dialog"):
-            yield Label(f"Transaction #{self.transaction.id} Details", id="title")
-            yield Label(f"Date: {date_str}")
             yield Label(
-                f"Account: {self.DB.get_account_by_id(int(self.transaction.account_id)).name}"
+                _("Transaction #{transaction_id} Details").format(
+                    transaction_id=self.transaction.id
+                ),
+                id="title",
+            )
+            yield Label(_("Date: {date_str}").format(date_str=date_str))
+            yield Label(
+                _("Account: {account_name}").format(
+                    account_name=self.DB.get_account_by_id(
+                        int(self.transaction.account_id)
+                    ).name
+                )
+            )
+            yield Label(_("Amount: {amt}").format(amt=self.transaction.amount))
+            yield Label(
+                _("Description: {desc}").format(desc=self.transaction.description)
+            )
+            yield Label(
+                _("Category: {category}").format(category=self.transaction.category)
             )
-            yield Label(f"Amount: {self.transaction.amount}")
-            yield Label(f"Description: {self.transaction.description}")
-            yield Label(f"Category: {self.transaction.category}")
             with Horizontal(id="buttons"):
-                yield Button("Close", id="close-button")
-                yield Button("Edit", id="edit-button", variant="primary")
-                yield Button.error("Delete", id="delete-button")
+                yield Button(_("Close"), id="close-button")
+                yield Button(_("Edit"), id="edit-button", variant="primary")
+                yield Button.error(_("Delete"), id="delete-button")
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Button handler"""
 
         if event.button.id == "close-button":
             self.app.pop_screen()
 
@@ -51,14 +68,14 @@
             self.DB.delete_transaction(self.transaction.id)
             self.app.pop_screen()
 
             if self.from_manage_accounts:
                 self.app.pop_screen()
 
             self.notify(
-                "The transaction has been successfully deleted.",
-                title="Transaction Deleted",
+                _("The transaction has been successfully deleted."),
+                title=_("Transaction Deleted"),
             )
 
         if event.button.id == "edit-button":
             self.app.pop_screen()
             self.app.push_screen(AddTransaction(self.transaction))
```

### Comparing `budgetize-0.0.3/budgetize/tui/screens/_add_transaction.py` & `budgetize-0.1.0/budgetize/tui/screens/add_transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 """Module that defines the AddTransaction screen"""
 
+import logging
 from datetime import date as date_func
-from traceback import print_exc
+from traceback import format_exc
 from typing import Optional
 
 from arrow import Arrow
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.screen import Screen
-from textual.types import NoSelection
 from textual.validation import Number
 from textual.widgets import Button, Footer, Header, Input, Label, Select
 
-from budgetize.consts import DEFAULT_CATEGORIES
-from budgetize.db import Database
-from budgetize.db.orm import Transaction
+from budgetize.db.database import Database
+from budgetize.db.orm.transactions import Transaction
+from budgetize.settings_manager import SettingsManager
+from budgetize.utils import _
 
 
 class AddTransaction(Screen):
     """Screen that handles adding a new transaction"""
 
     DB: Database = None  # type: ignore
     BINDINGS = [
         Binding(
             key="q,Q",
             key_display="Q",
             action="pop_screen",
-            description="Cancel Transaction",
+            description=_("Cancel Transaction"),
         ),
     ]
 
     def __init__(self, transaction: Optional[Transaction] = None) -> None:
         """Creates a new AddTransaction screen"""
         AddTransaction.DB = Database(self.app)
         self.transaction = transaction
         super().__init__()
 
     def compose(self) -> ComposeResult:
+        """Called when screen is composed"""
+
+        logging.info("Composing AddTransaction Screen...")
         self.app.sub_title = (
             "Edit Transaction" if self.transaction else "Add Transaction"
         )
         yield Header()
         yield Footer()
 
-        yield Label("Account", id="account-label")
+        yield Label(_("Account"), id="account-label")
         yield Select(
             self._get_account_options(),
             id="account-select",
             allow_blank=False,
             value=self.transaction.account_id if self.transaction else Select.BLANK,
             prompt="Select an account",
         )
-        yield Label("Amount", id="amount-label")
+        yield Label(_("Amount"), id="amount-label")
         yield Input(
             type="number",
             placeholder="250",
             id="amount-input",
             value=str(self.transaction.amount) if self.transaction else "",
             validators=[Number(failure_description="Please enter a valid number")],
         )
@@ -64,62 +68,74 @@
 
         transaction_date = (
             Arrow.fromtimestamp(self.transaction.timestamp)
             if self.transaction
             else today
         )
         # TODO: Implement a day and a time picker
-        yield Label("Date", id="date-label")
+        yield Label(_("Date"), id="date-label")
         yield Input(
             placeholder=today.format("M/D/YYYY"),
             id="date-input",
             value=transaction_date.format("M/D/YYYY"),
         )
 
         yield Select(
             self.get_category_select_options(), allow_blank=False, id="category-select"
         )
 
-        yield Label("Description", id="description-label")
+        yield Label(_("Description"), id="description-label")
         yield Input(
             max_length=255,
             placeholder="Description for your income/expense",
             id="description-input",
             value=self.transaction.description if self.transaction else "",
         )
 
-        lbl = "Update Transaction" if self.transaction else "Add Transaction"
+        lbl = _("Update Transaction") if self.transaction else _("Add Transaction")
         yield Button(lbl, id="add-transaction-button")
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Handles button presses"""
 
+        logging.info("Adding Transaction")
         account_selected: int = self.get_widget_by_id("account-select").value  # type: ignore
         account = self.DB.get_account_by_id(account_selected)
         currency = account.currency
 
         amount = self.get_widget_by_id("amount-input").value  # type: ignore
 
         category = self.get_widget_by_id("category-select").value  # type: ignore
         description = self.get_widget_by_id("description-input").value  # type: ignore
 
         # Attempt to parse the date from the user in M/D/YYYY/
         # If parsing fails, use the current date and time for saving the transaction
 
+        logging.debug(
+            f"Amount: {amount}, Category: {category}, Description: {description}"
+        )
         date = Arrow.now()
 
         try:
+            # TODO: Parse date based on locale
+
             date_strs: list[str] = self.get_widget_by_id("date-input").value.split("/")  # type: ignore
             date_from_input = date_func(
                 int(date_strs[2]), int(date_strs[0]), int(date_strs[1])
             )
             date = Arrow.fromdate(date_from_input)
+            logging.warning(
+                "PARSE DATE BASED ON LOCALE. THIS PARSING IS DONE MANUALLY."
+            )
+            logging.debug(f"Parsed Date: {date}")
 
         except Exception:
-            print_exc()
+            traceback_str = format_exc()
+            logging.critical("An error ocurred parsing the date.\n" + traceback_str)
+            logging.info("Using current date and time for transaction")
             date = Arrow.now()
 
         # Clear fields
         self.get_widget_by_id("amount-input").value = ""  # type: ignore
         self.get_widget_by_id("date-input").value = ""  # type: ignore
 
         if self.transaction:
@@ -128,32 +144,39 @@
                 account_id=account.id,
                 amount=amount,
                 description=description,
                 category=category,
                 timestamp=date.timestamp(),
             )
             self.app.pop_screen()
-            self.app.notify(f"Sucessfully updated transaction!")
+            self.app.notify(
+                _("Sucessfully updated transaction!"), title=_("Transaction Updated")
+            )
             return
 
         self.DB.add_transaction(
             account_id=account.id,
             amount=amount,
             description=description,
             category=category,
             timestamp=date.timestamp(),
         )
 
         self.app.pop_screen()
-        self.app.notify(f"Sucessfully added transaction of {currency} {amount}")
+        self.app.notify(
+            _("Sucessfully added transaction of {currency} {amount}").format(
+                currency=currency, amount=amount
+            ),
+            title=_("Transaction Added"),
+        )
 
     def _get_account_options(self) -> list[tuple[str, int]]:
         """Returns a list of tuples (name, id) for the TUI to show"""
         return [(account.name, account.id) for account in self.DB.get_accounts()]
 
     def get_category_select_options(self) -> list[tuple[str, str]]:
         """Returns a list of tuples (name, id) for the TUI to show"""
         categories = []
-        for category in DEFAULT_CATEGORIES:
+        for category in SettingsManager().get_categories():
             categories.append((category, category))
 
         return categories
```

### Comparing `budgetize-0.0.3/budgetize/tui/screens/_create_account.py` & `budgetize-0.1.0/budgetize/tui/screens/create_account.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,106 @@
 """Module that defines the CreateAccount screen."""
 
+import logging
+
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Grid, Horizontal, VerticalScroll
 from textual.screen import Screen
 from textual.validation import Number
 from textual.widgets import Button, Footer, Header, Input, Label, Select
 
-from budgetize.consts import CURRENCIES
-from budgetize.db import Database
-from budgetize.db.orm import Account, AccountType
+from budgetize.db.database import Database
+from budgetize.tui.modals.error_modal import ErrorModal
+from budgetize.utils import _, get_select_currencies
 
 
 class CreateAccount(Screen):
     """Screen that allows the user to create a new account."""
 
     CSS_PATH = "css/create_account.tcss"
 
     DB: Database = None  # type: ignore
     BINDINGS = [
-        Binding(key="c,C", key_display="C", action="pop_screen", description="Cancel"),
+        Binding(
+            key="c,C", key_display="C", action="pop_screen", description=_("Cancel")
+        ),
     ]
 
     def __init__(self) -> None:
         """Creates a new CreateAccount Screen"""
         CreateAccount.DB = Database(self.app)
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Called when the screen is composed."""
 
-        self.app.sub_title = "Create Account"
+        logging.info("Composing CreateAccount Screen...")
+        self.app.sub_title = _("Create Account")
         yield Header()
         yield Footer()
 
         yield VerticalScroll(
             Grid(
                 # Place them in this way because grids are filled in row-order
-                Label("Account Currency", id="currency-label"),
-                Label("Account Name", id="name-label"),
+                Label(_("Account Currency"), id="currency-label"),
+                Label(_("Account Name"), id="name-label"),
                 Select(
-                    self.get_currency_choices(), id="currency-select", allow_blank=False
+                    get_select_currencies(), id="currency-select", allow_blank=False
                 ),
-                Input(placeholder="Bank Account", id="account-name-input"),
+                Input(placeholder=_("Bank Account"), id="account-name-input"),
             ),
-            Label("Starting Balance", id="balance-label"),
+            Label(_("Starting Balance"), id="balance-label"),
             Input(
                 type="number",
                 placeholder="250",
                 id="balance-input",
                 validators=[
                     Number(
                         minimum=0,
-                        failure_description="Initial Balance must be atleast zero.",
+                        failure_description=_("Initial Balance must be atleast zero."),
                     )
                 ],
             ),
-            Label("Account Type", id="account-type-label"),
-            Select(
-                self.get_account_type_choices(),
-                id="account-type-select",
-                allow_blank=False,
-            ),
             Horizontal(
-                Button.success("Create Account", id="create-account-button"),
-                Button.error("Cancel", id="cancel-button"),
+                Button.success(_("Create Account"), id="create-account-button"),
+                Button.error(_("Cancel"), id="cancel-button"),
             ),
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Button press handlers"""
 
         if event.button.id == "create-account-button":
             name: str = self.get_widget_by_id("account-name-input").value  # type: ignore
             currency: str = self.get_widget_by_id("currency-select").value  # type: ignore
-            balance: float = self.get_widget_by_id("balance-input").value  # type: ignore
-            account_type_name: str = self.get_widget_by_id("account-type-select").value  # type: ignore #pylint: disable=line-too-long
+            starting_balance: float = self.get_widget_by_id("balance-input").value  # type: ignore
+
+            logging.debug(f"Creating Account: {name} {currency} {starting_balance}")
+
+            if self.DB.account_name_exists(name):
+                logging.warning("Account Name already exists! Showing error")
+                self.app.push_screen(
+                    ErrorModal(
+                        _("Account Name already Exists"),
+                        traceback_msg=_(
+                            "You cannot have 2 accounts with the same name!"
+                        ),
+                    )
+                )
+                return
 
-            new_account = Account(
-                account_type_name=account_type_name.upper(),
+            self.DB.add_account(
                 name=name,
                 currency=currency,
-                balance=balance,
+                starting_balance=starting_balance,
             )
 
-            self.DB.add_account(new_account)
+            self.notify(_("Account created successfully."), title="Account Created")
+            self.get_widget_by_id("account-name-input").value = ""  # type: ignore
+            self.get_widget_by_id("balance-input").value = ""  # type: ignore
             self.app.pop_screen()
-            self.notify("Account created successfully.", title="Account Created")
-
-        elif event.button.id == "cancel-button":
+        else:
+            # Clear the input fields
             self.get_widget_by_id("account-name-input").value = ""  # type: ignore
             self.get_widget_by_id("balance-input").value = ""  # type: ignore
             self.app.pop_screen()
-
-    def get_currency_choices(self) -> list[tuple[str, str]]:
-        """Returns a list of tuples for the currency select widget"""
-        res = []
-        for curr in CURRENCIES:
-            res.append((f"({curr[0]}) {curr[1]}", curr[0]))
-
-        return res
-
-    def get_account_type_choices(self) -> list[tuple[str, str]]:
-        """Returns a list of tuples for the account type select widget"""
-        res = []
-        for acc in AccountType:
-            res.append((acc.name.capitalize(), acc.name.capitalize()))
-
-        return res
```

### Comparing `budgetize-0.0.3/budgetize/tui/screens/_manage_accounts.py` & `budgetize-0.1.0/budgetize/tui/screens/manage_accounts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,98 @@
 """Screen that allows the user to manage their accounts."""
 
+import gettext
+import logging
 from typing import Generator
 
 from arrow import Arrow
+from babel.numbers import format_currency
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.screen import Screen
 from textual.widgets import (
     Button,
     DataTable,
     Footer,
     Header,
     Label,
     TabbedContent,
     TabPane,
 )
 
-from budgetize.db import Database
-from budgetize.tui.modals import TransactionDetails
+from budgetize import SettingsManager
+from budgetize.db.database import Database
+from budgetize.tui.modals.transaction_details import TransactionDetails
+from budgetize.utils import _
 
 
 class ManageAccounts(Screen):
     """Screen that allows the user to manage their accounts."""
 
     DB: Database = None  # type: ignore
-    BINDINGS = [Binding("Q,q", "pop_screen", "Back to Main Menu", key_display="Q")]
+    BINDINGS = [Binding("Q,q", "pop_screen", _("Back to Main Menu"), key_display="Q")]
 
     def __init__(self) -> None:
         """Creates a new ManageAccounts Screen"""
         ManageAccounts.DB = Database(self.app)
         super().__init__()
 
     def compose(self) -> ComposeResult:
-        self.app.sub_title = "Manage Accounts"
+        logging.info("Composing ManageAccounts Screen")
+
+        self.app.sub_title = _("Manage Accounts")
         yield Header()
         yield Footer()
 
         with TabbedContent():
             accounts = self.DB.get_accounts()
             for acc in accounts:
+                logging.info(f"Generating tab for account {acc.name}")
                 with TabPane(acc.name, id=f"tab-{acc.name.replace(' ', '-')}"):
-                    yield Label(f"Balance: {acc.balance}")
+
+                    account_balance = self.DB.get_account_balance(acc.id)
+                    yield Label(
+                        _("Balance: {balance}").format(
+                            balance=format_currency(
+                                number=account_balance,
+                                currency=acc.currency,
+                                locale=SettingsManager().get_locale(),
+                            )
+                        )
+                    )
                     yield self.get_transactions_table(acc.id)
-                    yield Button.error(f"Delete Account", id=f"delete-acc-{acc.id}")
+                    yield Button.error(_("Delete Account"), id=f"delete-acc-{acc.id}")
 
     def generate_accounts_tab(self) -> Generator:
         """Generates the accounts tab including all user accounts"""
 
         with TabbedContent() as tabs:
             accounts = self.DB.get_accounts()
             for acc in accounts:
                 with TabPane(acc.name, id=f"tab-{acc.name.replace(' ', '-')}"):
-                    yield Label(f"Balance: {acc.balance}")
+                    account_balance = self.DB.get_account_balance(acc.id)
+                    yield Label(
+                        _("Balance: {balance}").format(
+                            balance=format_currency(
+                                number=account_balance,
+                                currency=acc.currency,
+                                locale=SettingsManager().get_locale(),
+                            )
+                        )
+                    )
                     yield self.get_transactions_table(acc.id)
-                    yield Button(f"Delete Account", id=f"delete-acc-{acc.id}")
+                    yield Button(_("Delete Account"), id=f"delete-acc-{acc.id}")
             return tabs
 
     def get_transactions_table(self, account: int) -> DataTable:
         """Returns the data table containing the transactions for an account."""
 
+        logging.info(f"Building transactions table for Account #{account}")
         table: DataTable = DataTable(id=f"management-table-{str(account)}")  # type: ignore
-        table.add_columns("Date", "Amount", "Category", "Description")
+        table.add_columns(_("Date"), _("Amount"), _("Category"), _("Description"))
 
         now = Arrow.now()
         month = now.format("M")
         year = now.format("YYYY")
         transactions = self.DB.get_monthly_transactions_from_account(
             account, month=month, year=year
         )
@@ -73,40 +101,41 @@
             color = "[green]" if trans.amount > 0 else "[red]"
             date = Arrow.fromtimestamp(trans.timestamp).format("M/D/YYYY")
             table.add_row(
                 date,
                 color + str(trans.amount),
                 trans.category,
                 trans.description,
-                key=trans.id,
+                key=str(trans.id),
             )
-
+        logging.info("Table done building.")
         return table
 
     def on_data_table_cell_selected(self, event: DataTable.CellSelected) -> None:
         """Cell selection handler"""
 
         selected_cell = event.coordinate.row
         current_row = 0
         for row in event.data_table.rows:
             if current_row == selected_cell and row.value is not None:
                 details_screen = TransactionDetails(
                     int(row.value), from_manage_accounts=True
                 )
+                logging.info("Showing Transaction Details modal")
                 self.app.push_screen(details_screen)
                 break
             current_row += 1
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Button push handler"""
 
-        if event.button.id is None:
-            return
-
-        if "delete-acc" in event.button.id:
+        if event.button.id == "delete-acc":
             # Format of btn is delete-acc-{Account.id}
 
             account_id = int(event.button.id.split("-")[-1])
             account_name = self.DB.get_account_by_id(account_id).name
             self.DB.delete_account(account_id=account_id)
-            self.notify(f"{account_name} has been deleted.", title="Account Deleted")
+            self.notify(
+                _("{account_name} has been deleted.").format(account_name=account_name),
+                title=_("Account Deleted"),
+            )
             self.app.pop_screen()
```

### Comparing `budgetize-0.0.3/LICENSE` & `budgetize-0.1.0/LICENSE`

 * *Files identical despite different names*

