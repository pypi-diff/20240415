# Comparing `tmp/qtlink-1.1.4.tar.gz` & `tmp/qtlink-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.1.4.tar", last modified: Thu Apr 11 06:30:30 2024, max compression
+gzip compressed data, was "qtlink-1.2.0.tar", last modified: Mon Apr 15 02:22:16 2024, max compression
```

## Comparing `qtlink-1.1.4.tar` & `qtlink-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.202021 qtlink-1.1.4/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-11 06:30:30.175553 qtlink-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.127411 qtlink-1.1.4/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.1.4/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.165566 qtlink-1.1.4/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.1.4/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.1.4/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-11 02:31:03.000000 qtlink-1.1.4/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1406 2024-04-10 12:21:37.000000 qtlink-1.1.4/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     1086 2024-04-10 11:53:14.000000 qtlink-1.1.4/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.165566 qtlink-1.1.4/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.4/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2042 2024-04-10 12:40:42.000000 qtlink-1.1.4/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.168686 qtlink-1.1.4/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.4/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     6668 2024-04-10 12:00:18.000000 qtlink-1.1.4/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     5455 2024-04-10 11:53:14.000000 qtlink-1.1.4/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     1919 2024-04-10 11:59:10.000000 qtlink-1.1.4/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     3547 2024-04-11 06:29:02.000000 qtlink-1.1.4/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.172450 qtlink-1.1.4/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.1.4/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.1.4/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.1.4/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:30:30.175553 qtlink-1.1.4/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-11 06:30:30.000000 qtlink-1.1.4/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-11 06:30:30.000000 qtlink-1.1.4/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:30:30.000000 qtlink-1.1.4/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-11 06:30:30.000000 qtlink-1.1.4/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 06:30:30.000000 qtlink-1.1.4/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 06:30:30.202021 qtlink-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-11 06:29:47.000000 qtlink-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.663329 qtlink-1.2.0/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-15 02:22:16.663329 qtlink-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.623572 qtlink-1.2.0/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.0/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.648157 qtlink-1.2.0/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.0/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1730 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0     1357 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1981 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     1926 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.660172 qtlink-1.2.0/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.0/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.663329 qtlink-1.2.0/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.0/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.0/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.0/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.663329 qtlink-1.2.0/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.0/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.2.0/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.0/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:22:16.663329 qtlink-1.2.0/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-15 02:22:16.000000 qtlink-1.2.0/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-15 02:22:16.000000 qtlink-1.2.0/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 02:22:16.000000 qtlink-1.2.0/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 02:22:16.000000 qtlink-1.2.0/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 02:22:16.000000 qtlink-1.2.0/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 02:22:16.663329 qtlink-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-15 02:20:21.000000 qtlink-1.2.0/setup.py
```

### Comparing `qtlink-1.1.4/LICENSE` & `qtlink-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.4/PKG-INFO` & `qtlink-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.1.4
+Version: 1.2.0
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.1.4/qtlink/dialog/dialog_choice.py` & `qtlink-1.2.0/qtlink/dialog/dialog_choice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QLabel, QPushButton, QHBoxLayout
 
 
-def show_dialog_choice(text: str, click_btn_confirm, show_or_exec: str = 'exec'):
-    dialog = DialogChoice(text, click_btn_confirm)
+def show_dialog_choice(text: str, click_btn_confirm, show_or_exec: str = 'exec', parent=None):
+    """以函数形式直接启动对话框
+    :param text: 对话框的消息文本
+    :param click_btn_confirm: 点击确定按钮后自动调用的函数
+    :param show_or_exec: 对话框的运行方式，'exec' or 'show'
+    :param parent: 对话框所属的父类
+    """
+    dialog = DialogChoice(text, click_btn_confirm=click_btn_confirm, parent=parent)
     if show_or_exec == 'exec':
         dialog.exec()
     else:
         dialog.show()
 
 
 class DialogChoice(QDialog):
-    def __init__(self, text: str, click_btn_confirm):
-        super().__init__()
+    """带有确定/取消按钮的对话框类"""
+
+    def __init__(self, text: str, click_btn_confirm, parent=None):
+        """
+        :param text: 对话框的文本消息
+        :param click_btn_confirm: 点击确定按钮后自动调用的函数
+        :param parent: 对话框所属的父类
+        """
+        super().__init__(parent=parent)
         vLayout = QVBoxLayout()
         self.click_btn_confirm = click_btn_confirm
         label = QLabel(text, self)
         label.setWordWrap(True)
         vLayout.addWidget(label)
 
         hLayout = QHBoxLayout()
```

### Comparing `qtlink-1.1.4/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.0/qtlink/dialog/dialog_table_check.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,28 +3,42 @@
 from qtlink import create_signal
 from qtlink.dialog.dialog_table_display import DialogTableDisplay
 from qtlink.table.table_controller_multiple_check import TableControllerMultipleCheck
 from qtlink.table.table_controller_single_check import TableControllerSingleCheck
 
 
 class DialogTableCheck(DialogTableDisplay):
-    def __init__(self, text: str, table_data: list[dict], check_type: str = 'single', parent=None):
+    """可以显示并选择表格数据的对话框"""
+
+    def __init__(self, text: str,
+                 table_data: list[dict],
+                 check_type: str = 'single',
+                 parent=None,
+                 *args, **kwargs):
+        """
+        :param text: 对话框的消息文本
+        :param table_data: 表格数据
+        :param check_type: 表格数据的选择方式，单选：'single'，多选：'multiple'
+        :param parent: 对话框所属的父类
+        :param args: 表格控制器可能使用的其他参数
+        :param kwargs: 表格控制器可能使用的其他参数
+        """
         super().__init__(text=text, table_data=table_data, parent=parent)
 
         self.btn_ok = QPushButton('确定')
         self.v_layout.addWidget(self.btn_ok)
         self.setLayout(self.v_layout)
 
         if check_type == 'single':
             self.table_controller = TableControllerSingleCheck(tableview=self.tableview)
         elif check_type == 'multiple':
             self.table_controller = TableControllerMultipleCheck(tableview=self.tableview)
         else:
             raise ValueError(f"check_type的值只允许是：'single' 或 'multiple'，但得到的是：{check_type}")
-        self.update_table_data(table_data)
+        self.table_controller.update_table_data(table_data, *args, **kwargs)
 
         self.signal_checked_rows = create_signal(list)
         self.btn_ok.clicked.connect(self.click_btn_ok)
 
     def click_btn_ok(self):
         checked_data = self.table_controller.get_checked_rows()
         self.signal_checked_rows.signal.emit(checked_data)
```

### Comparing `qtlink-1.1.4/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.0/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 from PySide6.QtWidgets import QWidget
 
 
 class MplCanvas(QWidget):
+    """在qt中使用matplotlib绘制图像"""
+
     def __init__(self, width: float = 5, height: float = 4, dpi: int = 100, enable_toolbar: bool = True, parent=None):
+        """
+        :param width: 图像宽度
+        :param height: 图像高度
+        :param dpi: 图像dpi
+        :param enable_toolbar: 是否启用顶部工具栏
+        :param parent: 所属的ui父类
+        """
         from matplotlib import pyplot as plt
         from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas, \
             NavigationToolbar2QT as NavigationToolbar
         from matplotlib.figure import Figure
         from PySide6.QtWidgets import QVBoxLayout
         plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
         plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
@@ -19,23 +28,29 @@
         if enable_toolbar:
             self.toolbar = NavigationToolbar(self.canvas, self)
             self.vertical_layout.addWidget(self.toolbar)
         self.vertical_layout.addWidget(self.canvas)
         self.setLayout(self.vertical_layout)
 
     def clear_canvas(self):
+        """清空画布"""
         self.canvas.figure.clear()
         self.ax = self.canvas.figure.subplots()
         self.canvas.draw_idle()
 
     def plot_lines(self, data: list[dict],
                    x_label: str = '',
                    y_label: str = '',
                    title: str = ''):
-
+        """绘制点线图
+        :param data: 每个点的数据使用字典存储，大致结构为{'x': , 'y': , 'label': }
+        :param x_label: x轴名称
+        :param y_label: y轴名称
+        :param title: 图像名称
+        """
         enable_legend = False
         for item in data:
             if item.get('label'):
                 enable_legend = True
                 self.ax.plot(item['x'], item['y'], marker='o', markersize=3, label=item['label'])
             else:
                 self.ax.plot(item['x'], item['y'], marker='o', markersize=3)
```

### Comparing `qtlink-1.1.4/qtlink/util.py` & `qtlink-1.2.0/qtlink/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from PySide6.QtCore import QObject, Signal
 
 
 def force_draw():
-    """强制绘制挂起的事件，如弹窗"""
+    """强制绘制挂起的事件，如弹窗，如果一次调用仍然存在未绘制的情况，可以多调用几次，在show前show后均调用"""
     from PySide6.QtWidgets import QApplication
     QApplication.processEvents()
 
 
 def create_signal(signal_type):
-    """根据传入类型，创建相应的信号类。"""
+    """根据传入类型，创建相应的信号类。
+    :param signal_type: 任意的数据类型，如int, str, list等
+    :return: qt信号类
+    """
 
     class CustomSignal(QObject):
         signal = Signal(signal_type)
 
     return CustomSignal()
 
 
 class ProgressSignalSlot:
     """需要某个类继承它，并连接response_signal方法到tuple类型的信号。
     然后根据需要实现各种when_xxx方法，即可根据不同状态自动调用相应的处理方法。"""
 
     def response_signal(self, state: tuple):
+        """内置方法，直接连接外部的qt信号"""
         flag, data = state
         if flag == Progress.flag_start:
             self.when_start(data)
         elif flag == Progress.flag_doing:
             self.when_doing(data)
         elif flag == Progress.flag_success:
             self.when_success(data)
@@ -40,43 +44,70 @@
             self.when_other2(data)
         elif flag == Progress.flag_other3:
             self.when_other3(data)
         else:
             raise ValueError(f'传递的信号数据错误。应该是 tuple ，但得到的是 {type(state)}')
 
     def when_start(self, data: list = None):
+        """事件刚开始
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_doing(self, data: list = None):
+        """事件正在进行中
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_success(self, data: list = None):
+        """事件成功
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_failed(self, data: list = None):
+        """事件失败
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_end(self, data: list = None):
+        """事件结束
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_info(self, data: list = None):
+        """事件信息
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_other1(self, data: list = None):
+        """预留的任意状态
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_other2(self, data: list = None):
+        """预留的任意状态
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
     def when_other3(self, data: list = None):
+        """预留的任意状态
+        :param data: 当需要传输数据时，使用此参数
+        """
         pass
 
 
 class Progress:
-    """发射信号时应该使用此类来传输数据。
+    """搭配ProgressSignalSlot使用，发射信号时应该使用此类来传输数据。
 
     Example:
         # 具体数据应使用list包裹，这利于处理复杂形态的数据。
         some_signal.emit(Progress.start(['处理开始']))
 
     """
     flag_start = 0
```

### Comparing `qtlink-1.1.4/qtlink/widgets/drop_widget.py` & `qtlink-1.2.0/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.4/qtlink.egg-info/PKG-INFO` & `qtlink-1.2.0/qtlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.1.4
+Version: 1.2.0
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.1.4/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.0/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.4/setup.py` & `qtlink-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.1.4",
+    version="1.2.0",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6', 'matplotlib', 'numpy'],
```

