# Comparing `tmp/JayttleProcess-0.1.6-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 35407 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     2458 b- defN 24-Apr-11 07:02 JayttleProcess/CommonDecorator.py
+Zip file size: 44169 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat     2602 b- defN 24-Apr-13 06:50 JayttleProcess/CommonDecorator.py
 -rw-rw-rw-  2.0 fat     4727 b- defN 24-Mar-19 06:31 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
--rw-rw-rw-  2.0 fat    16907 b- defN 24-Apr-11 07:08 JayttleProcess/SQLCommonUse.py
+-rw-rw-rw-  2.0 fat     5642 b- defN 24-Apr-11 13:31 JayttleProcess/JsonCommonManage.py
+-rw-rw-rw-  2.0 fat    12990 b- defN 24-Apr-14 09:17 JayttleProcess/RinexCommonManage.py
+-rw-rw-rw-  2.0 fat    29613 b- defN 24-Apr-13 11:31 JayttleProcess/SQLCommonUse.py
 -rw-rw-rw-  2.0 fat   117579 b- defN 24-Apr-08 05:24 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      861 b- defN 24-Apr-11 07:15 JayttleProcess-0.1.6.dist-info/RECORD
-10 files, 143883 bytes uncompressed, 33923 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat      656 b- defN 24-Apr-14 23:24 JayttleProcess-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 23:24 JayttleProcess-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-14 23:24 JayttleProcess-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1045 b- defN 24-Apr-14 23:24 JayttleProcess-0.1.7.dist-info/RECORD
+12 files, 175574 bytes uncompressed, 42395 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -3,29 +3,35 @@
 
 Filename: JayttleProcess/ComputerControl.py
 Comment: 
 
 Filename: JayttleProcess/EntertainmentCode.py
 Comment: 
 
+Filename: JayttleProcess/JsonCommonManage.py
+Comment: 
+
+Filename: JayttleProcess/RinexCommonManage.py
+Comment: 
+
 Filename: JayttleProcess/SQLCommonUse.py
 Comment: 
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.1.6.dist-info/METADATA
+Filename: JayttleProcess-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.1.6.dist-info/WHEEL
+Filename: JayttleProcess-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.1.6.dist-info/top_level.txt
+Filename: JayttleProcess-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.1.6.dist-info/RECORD
+Filename: JayttleProcess-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/CommonDecorator.py

```diff
@@ -8,23 +8,23 @@
     def wrapper(*args, **kwargs):
         # 记录函数调用时间
         call_time = datetime.now()
         start_time = time.time()  # 记录函数开始执行的时间
 
         print(f"Function '{func.__name__}' called at {call_time}")
 
-        # 记录传入的参数
-        args_str = ', '.join(map(repr, args))
-        kwargs_str = ', '.join(f"{key}={value!r}" for key, value in kwargs.items())
-        all_args = ', '.join(filter(None, [args_str, kwargs_str]))
-        print(f"Arguments: {all_args}")
+        # 记录传入的参数类型
+        args_type_str = ', '.join(map(lambda arg: f"{type(arg).__name__}", args))
+        kwargs_type_str = ', '.join(f"{key}={type(value).__name__}" for key, value in kwargs.items())
+        all_args_type = ', '.join(filter(None, [args_type_str, kwargs_type_str]))
+        print(f"Arguments type: {all_args_type}")
 
         # 调用函数并记录返回值
         result = func(*args, **kwargs)
-        print(f"Returned: {result}")
+        print(f"Returned data type: {type(result).__name__}")  # 打印返回值的数据类型
         end_time = time.time()  # 记录函数执行完毕的时间
         print(f"executed in {(end_time - start_time):.4f}s")  # 打印执行时间
         print()
         return result
 
     return wrapper
```

## JayttleProcess/SQLCommonUse.py

```diff
@@ -1,33 +1,36 @@
 import pymysql
 import functools
 import matplotlib.pyplot as plt
+import matplotlib.dates as mdates
 import numpy as np
+import pandas as pd
 import time
 from datetime import datetime, timedelta
 from typing import Union
+from tabulate import tabulate
 
 def log_function_call(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         # 记录函数调用时间
         call_time = datetime.now()
         start_time = time.time()  # 记录函数开始执行的时间
 
         print(f"Function '{func.__name__}' called at {call_time}")
 
-        # 记录传入的参数
-        args_str = ', '.join(map(repr, args))
-        kwargs_str = ', '.join(f"{key}={value!r}" for key, value in kwargs.items())
-        all_args = ', '.join(filter(None, [args_str, kwargs_str]))
-        print(f"Arguments: {all_args}")
+        # 记录传入的参数类型
+        args_type_str = ', '.join(map(lambda arg: f"{type(arg).__name__}", args))
+        kwargs_type_str = ', '.join(f"{key}={type(value).__name__}" for key, value in kwargs.items())
+        all_args_type = ', '.join(filter(None, [args_type_str, kwargs_type_str]))
+        print(f"Arguments type: {all_args_type}")
 
         # 调用函数并记录返回值
         result = func(*args, **kwargs)
-        print(f"Returned: {result}")
+        print(f"Returned data type: {type(result).__name__}")  # 打印返回值的数据类型
         end_time = time.time()  # 记录函数执行完毕的时间
         print(f"executed in {(end_time - start_time):.4f}s")  # 打印执行时间
         print()
         return result
 
     return wrapper
 
@@ -275,28 +278,28 @@
     print("\t\"host\": \"localhost\",")
     print("\t\"user\": \"Jayttle\",")
     print("\t\"password\": \"@JayttleRoot\",")
     print("\t\"database\": \"jayttle\"")
     print("}")
 
 
-def create_table() -> None:
+def create_table(listName: str) -> None:
     """创建表的 SQL 语句 """
     create_table_query = """
-    CREATE TABLE IF NOT EXISTS met (
+    CREATE TABLE IF NOT EXISTS {0}} (
         Time DATETIME NOT NULL,
         StationID INT NOT NULL,
         Temperature FLOAT,
         Humidness FLOAT,
         Pressure FLOAT,
         WindSpeed FLOAT,
         WindDirection VARCHAR(20),
         PRIMARY KEY (Time, StationID)
     )
-    """
+    """.format(listName)
     execute_sql(create_table_query)
 
 
 def create_table_id() -> None:
     """创建表的 SQL 语句 """
     create_table_query = """
     CREATE TABLE IF NOT EXISTS met_id (
@@ -304,43 +307,14 @@
         Name VARCHAR(255) NOT NULL,
         PRIMARY KEY (StationID)
     )
     """
     execute_sql(create_table_query)
 
 
-def insert_data(*args, **kwargs):
-    if len(args) == 2 and isinstance(args[0], str) and isinstance(args[1], int):
-        station_id, name = args
-        insert_query = """
-        INSERT INTO met 
-        (Time, StationID, Temperature, Humidness, Pressure, WindSpeed, WindDirection)
-        VALUES 
-        (%s, %s, 25.5, 50.0, 1013.25, 10.0, 'N')
-        """
-        values = (args[0], args[1])  # 使用 %s 占位符，并传入参数值的元组
-        execute_sql_params(insert_query, values)
-    else:
-        default_insert_data_query = """
-        INSERT INTO met (Time, StationID, Temperature, Humidness, Pressure, WindSpeed, WindDirection)
-        VALUES ('2024-04-08 12:00:00', 7, 25.5, 50.0, 1013.25, 10.0, 'N')
-        """
-        execute_sql(default_insert_data_query)
-
-
-def insert_data_id() -> None:
-    """插入数据的 SQL 语句 """
-    insert_data_query = """
-    INSERT INTO met_id (StationID, Name)
-    VALUES
-    (7, 'M07')
-    """
-    execute_sql(insert_data_query)  
-
-
 def delete_data(station_id: int) -> None:
     """删除数据"""
     delete_query = """
     DELETE FROM met_id
     WHERE StationID = %s
     """
     execute_sql_params(delete_query, (station_id,))
@@ -360,31 +334,33 @@
     UPDATE met_id
     SET Name = %s
     WHERE StationID = %s
     """
     execute_sql_params(update_query, (new_name, station_id))
 
 
-def get_min_max_time() -> tuple:
+@log_function_call
+def get_min_max_time(listName: str) -> tuple:
     # 查询 Time 列的最小值和最大值
-    query = "SELECT MIN(Time) AS min_time, MAX(Time) AS max_time FROM met;"
+    query = "SELECT MIN(Time) AS min_time, MAX(Time) AS max_time FROM {0};".format(listName)
     conn = pymysql.connect(**SQL_CONFIG)
     cursor = conn.cursor()
     try:
         cursor.execute(query)
         result = cursor.fetchone()
         return result
     except Exception as e:
         print("Error executing SQL statement:", e)
         return None
     finally:
         cursor.close()
         conn.close()
 
 
+@log_function_call
 def query_time_difference(listName: str, StartTime: datetime, EndTime: datetime) -> tuple:
     # 构建带有参数的查询语句
     sql_statement = """
     WITH TimeDiffCTE AS (
         SELECT
             time,
             LAG(time) OVER (ORDER BY time) AS PreviousTime,
@@ -418,24 +394,26 @@
         print("Error executing SQL statement:", e)
         return None
     finally:
         cursor.close()
         conn.close()
 
 
-def extract_time_data() -> list[tuple[datetime]]:
+@log_function_call
+def extract_time_data(listName: str) -> list[tuple[datetime]]:
     # 查询 Time 属性的数据
-    query = "SELECT Time FROM met"
+    query = "SELECT Time FROM {0}".format(listName)
     
     # 执行查询语句
     results = execute_sql(query)
     
     return results
 
 
+@log_function_call
 def preprocess_time_data(time_data: list[tuple[datetime]]) -> list[datetime]:
     processed_time_data = []
     current_year = datetime.now().year  # 获取当前年份
 
     for row in time_data:
         if row[0] is not None:  # 确保数据不是空值
             # 修改年份为当前年份，保持月、日、时、分、秒不变
@@ -445,14 +423,15 @@
         else:
             # 处理空值的情况（根据需要实现）
             print("Found None value, skipping...")
 
     return processed_time_data
 
 
+@log_function_call
 def aggregate_data_by_time(time_data: list[datetime], frequency: str) -> dict[datetime, list[str]]:
     aggregated_data = {}
 
     for time_point in time_data:
         # 根据给定的频率调整时间点
         if frequency == 'daily':
             aggregated_time = time_point.replace(hour=0, minute=0, second=0, microsecond=0)  # 将时间调整为当天的午夜
@@ -501,14 +480,15 @@
     plt.xlabel('属性名', fontproperties='SimHei')  # 使用中文标签
     plt.ylabel('时间', fontproperties='SimHei')  # 使用中文标签
     plt.title('数据存在情况热图', fontproperties='SimHei')  # 使用中文标题
     plt.tight_layout()
     plt.show()
 
 
+@log_function_call
 def count_records_in_table(table_name: str) -> int:
     """查看数据库中的表有多少个数据"""
     # 建立数据库连接
     conn = pymysql.connect(**SQL_CONFIG)
     cursor = conn.cursor()
 
     try:
@@ -532,7 +512,351 @@
         conn.rollback()
         raise e  # 将异常抛出，由调用者处理
 
     finally:
         # 关闭游标和数据库连接
         cursor.close()
         conn.close()
+
+
+@log_function_call
+def count_time_differences(tableName: list, startTime: datetime, stopTime: datetime) -> dict[float, int]:
+    # 构造查询 SQL 语句
+    sql_statement = f"SELECT Time FROM {tableName} WHERE Time >= %s AND Time <= %s"
+
+    # 建立数据库连接
+    conn = pymysql.connect(**SQL_CONFIG)
+    cursor = conn.cursor()
+
+    try:
+        # 执行 SQL 查询
+        cursor.execute(sql_statement, (startTime, stopTime))
+
+        # 获取查询结果
+        results = cursor.fetchall()
+
+        # 计算相邻时间差并统计
+        time_list = [row[0] for row in results]
+        time_list.sort()  # 将时间列表排序
+
+        # 计算相邻时间差
+        time_diffs = [(time_list[i + 1] - time_list[i]).total_seconds() for i in range(len(time_list) - 1)]
+
+        # 统计不同时间差的个数
+        diff_count = {}
+        for diff in time_diffs:
+            diff_count[diff] = diff_count.get(diff, 0) + 1
+
+        return diff_count
+
+    except Exception as e:
+        # 发生错误时回滚
+        conn.rollback()
+        print("Error executing SQL statement:", str(e))
+        return None
+
+    finally:
+        # 关闭游标和数据库连接
+        cursor.close()
+        conn.close()
+
+
+def calculate_missing_percentage(
+    start_time: datetime, 
+    end_time: datetime, 
+    missing_intervals: list[tuple[datetime, datetime, int]]
+) -> list[float]:
+    # Calculate total duration in hours
+    total_duration_hours = (end_time - start_time).total_seconds() / 3600
+
+    # Initialize weekly missing time list
+    weeks_count = (end_time - start_time).days // 7 + 1
+    weekly_missing_hours = [0] * weeks_count
+
+    # Accumulate missing hours per week
+    for interval_start, interval_end, missing_seconds in missing_intervals:
+        interval_duration_hours = missing_seconds / 3600
+        for week_index in range(weeks_count):
+            week_start = start_time + timedelta(days=week_index * 7)
+            week_end = week_start + timedelta(days=6)
+            if interval_start <= week_end and interval_end >= week_start:
+                overlap_start = max(interval_start, week_start)
+                overlap_end = min(interval_end, week_end)
+                overlap_duration_hours = (overlap_end - overlap_start).total_seconds() / 3600
+                weekly_missing_hours[week_index] += overlap_duration_hours
+
+    # Calculate missing percentage per week
+    weekly_missing_percentage = [(hours / total_duration_hours * 100) for hours in weekly_missing_hours]
+
+    return weekly_missing_percentage
+
+def visualize_missing_data(
+    start_time: datetime, 
+    end_time: datetime, 
+    missing_intervals: list[tuple[datetime, datetime, int]]
+) -> None:
+    # Calculate weekly missing percentage
+    weekly_missing_percentage = calculate_missing_percentage(start_time, end_time, missing_intervals)
+
+    # Create plot
+    weeks_count = len(weekly_missing_percentage)
+    week_labels = [f'Week {i+1}' for i in range(weeks_count)]
+    
+    plt.figure(figsize=(12, 6))
+    plt.bar(week_labels, weekly_missing_percentage, color='skyblue')
+    plt.xlabel('Week')
+    plt.ylabel('Missing Time Percentage (%)')
+    plt.title('Missing Time Percentage per Week')
+    plt.ylim(0, 100)  # Set y-axis limit from 0 to 100%
+    plt.xticks(rotation=45)
+    plt.grid(axis='y', linestyle='--', alpha=0.7)
+    plt.show()
+
+
+def read_tuple_data_from_txt(file_path: str) -> list[tuple[datetime, datetime, int]]:
+    """读取数据"""
+    tuple_data = []
+    with open(file_path, 'r') as file:
+        for line in file:
+            # Split each line into its components
+            parts = line.strip().split(',')
+            # Convert string representations to datetime objects
+            start_time = datetime.strptime(parts[0], "(%Y, %m, %d, %H, %M, %S, %f)")
+            end_time = datetime.strptime(parts[1], "(%Y, %m, %d, %H, %M, %S, %f)")
+            duration = int(parts[2])
+            # Append the tuple to the list
+            tuple_data.append((start_time, end_time, duration))
+    return tuple_data
+
+
+def calculate_weekly_missing_percentage(
+    start_time: datetime, 
+    end_time: datetime, 
+    missing_intervals: list[tuple[datetime, datetime, int]]
+) -> list[float]:
+    """
+    计算每周缺失百分比。
+
+    参数：
+    - start_time: datetime,起始时间
+    - end_time: datetime,结束时间
+    - missing_intervals: list[tuple[datetime, datetime, int]]，缺失时间段列表
+
+    返回：
+    - list[float]，每周的缺失百分比列表
+    """
+
+    # 计算总周数
+    total_weeks = (end_time - start_time).days // 7 + 1
+
+    # 初始化列表以存储每周的缺失百分比
+    weekly_missing_percentage = []
+
+    # 遍历每一周
+    for week_index in range(total_weeks):
+        # 定义周的起始和结束时间
+        week_start = start_time + timedelta(weeks=week_index)
+        week_end = min(start_time + timedelta(weeks=week_index + 1) - timedelta(microseconds=1), end_time)
+
+        # 计算一周的总秒数
+        seconds_in_week = (week_end - week_start).total_seconds()
+
+        # 计算一周内的缺失秒数
+        missing_seconds_in_week = 0
+        for interval_start, interval_end, missing_seconds in missing_intervals:
+            overlap_start = max(interval_start, week_start)
+            overlap_end = min(interval_end, week_end)
+            overlap_duration_seconds = max(0, (overlap_end - overlap_start).total_seconds())
+            missing_seconds_in_week += overlap_duration_seconds
+
+        # 计算一周的缺失百分比
+        missing_percentage = (missing_seconds_in_week / seconds_in_week) * 100
+        weekly_missing_percentage.append(missing_percentage)
+
+    return weekly_missing_percentage
+
+
+@log_function_call
+def calculate_daily_data_availability(min_time: datetime, max_time: datetime, missing_intervals: list[tuple[datetime, datetime, int]]) -> dict[datetime, float]:
+    """
+    计算每日数据存有率字典
+    
+    参数：
+        min_time (datetime): 数据的最小时间
+        max_time (datetime): 数据的最大时间
+        missing_intervals (List[Tuple[datetime, datetime, int]]): 包含缺失时间段的列表
+        
+    返回：
+        dict[datetime, float]: 包含日期和每日数据存有率的字典
+    """
+    # 初始化每日数据存有率字典
+    daily_data_availability = {}
+
+    # 生成日期范围
+    date_range = pd.date_range(start=min_time.date(), end=max_time.date(), freq='D')
+
+    for date in date_range:
+        # 当天的起始时间和结束时间
+        start_of_day = datetime.combine(date, datetime.min.time())
+        end_of_day = datetime.combine(date, datetime.max.time())
+
+        # 初始化当天缺失数据的秒数
+        missing_seconds = 0
+
+        # 计算当天缺失数据的秒数
+        for interval_start, interval_end, interval_missing_seconds in missing_intervals:
+            # 如果缺失时间段与当天有交集
+            if interval_start <= end_of_day and interval_end >= start_of_day:
+                # 计算交集部分的缺失秒数
+                intersection_start = max(interval_start, start_of_day)
+                intersection_end = min(interval_end, end_of_day)
+                intersection_duration = (intersection_end - intersection_start).total_seconds()
+                missing_seconds += intersection_duration
+
+        # 计算当天的数据存有率
+        total_seconds_in_day = (end_of_day - start_of_day).total_seconds()
+        data_availability_percentage = 100 * (1 - (missing_seconds / total_seconds_in_day))
+
+        # 将结果添加到字典，并精确到小数点后四位
+        daily_data_availability[start_of_day] = round(data_availability_percentage, 4)
+
+    return daily_data_availability
+
+
+@log_function_call
+def export_data_availability_to_file(daily_data_availability: dict[datetime, dict[str, float]]) -> None:
+    """
+    将每日数据存有率字典输出到文件
+    
+    参数：
+        daily_data_availability (dict[datetime, dict[str, float]]): 包含日期和每日数据存有率的字典
+        
+    返回：
+        None
+    """
+    # 将字典转换为 DataFrame
+    df = pd.DataFrame.from_dict(daily_data_availability, orient='index')
+    
+    # 将 NaN 替换为 0
+    df = df.fillna(0)
+
+    # 将 0 的数据存有率标识为 'N/A'
+    df = df.apply(lambda x: x.map(lambda val: 'N/A' if val == 0 else val))
+
+    # 重置索引，使日期成为列
+    df.reset_index(inplace=True)
+    df.rename(columns={'index': 'Date'}, inplace=True)
+
+    # 排序日期
+    df['Date'] = pd.to_datetime(df['Date'])
+    df = df.sort_values('Date')
+
+    # 生成表格
+    table = tabulate(df, headers='keys', tablefmt='fancy_grid', showindex=False)
+
+    # 将表格输出到文件
+    with open('output_table.txt', 'w', encoding='utf-8') as file:
+        file.write(table)
+
+    print("表格已经成功输出到文件 output_table.txt 中。")
+
+
+@log_function_call
+def load_missing_intervals(file_path: str) -> list[tuple[datetime, datetime, int]]:
+    """
+    从文件加载数据到 missing_intervals 列表中
+    
+    参数：
+        file_path (str): 文件路径
+        
+    返回：
+        List[Tuple[datetime, datetime, int]]: 包含缺失时间段的列表
+    """
+    missing_intervals = []
+
+    with open(file_path, "r") as file:
+        for line in file:
+            # 替换字符串中的 "datetime.datetime" 为 "datetime"
+            line = line.replace("datetime.datetime", "datetime")
+
+            # 使用 eval() 函数将字符串转换为元组
+            parts = eval(line)
+
+            # 解析日期时间和缺失秒数
+            start_time = parts[0]
+            end_time = parts[1]
+            missing_seconds = parts[2]
+
+            # 添加到 missing_intervals
+            missing_intervals.append((start_time, end_time, missing_seconds))
+
+    return missing_intervals
+
+
+
+
+def main() -> None:
+    file_path_met = "D:/python_proj2/SQL_Met.txt"
+    file_path_accelerometer = "D:/python_proj2/SQL_accelerometer.txt"
+    file_path_tiltmeter = "D:/python_proj2/SQL_tiltmeter.txt"
+    file_path_arr = "D:/python_proj2/SQL_arr.txt"
+    file_path_ggkx = "D:/python_proj2/SQL_arr.txt"
+
+
+    missing_intervals = load_missing_intervals(file_path_met)
+    missing_intervals_accelerometer = load_missing_intervals(file_path_accelerometer)
+    missing_intervals_tiltmeter = load_missing_intervals(file_path_tiltmeter)
+    missing_intervals_arr = load_missing_intervals(file_path_arr)
+    missing_intervals_ggkx = load_missing_intervals(file_path_ggkx)
+
+    # 最小时间和最大时间
+    min_time = datetime(2023, 4, 13, 16, 4, 40, 985000)
+    max_time = datetime(2024, 4, 11, 13, 5, 16, 701000)
+
+
+    accelerometer_min_time = datetime(2023, 7, 17, 16, 40, 39, 2000)
+    accelerometer_max_time = datetime(2023, 8, 16, 19, 49, 8, 583000)
+
+    tiltmeter_min_time = datetime(2023, 4, 17, 23, 49, 5, 782000)
+    tiltmeter_max_time = datetime(2024, 4, 12, 21, 1, 12, 430000)
+
+    arr_min_time = datetime(2023, 3, 23, 15, 15, 43)
+    arr_max_time = datetime(2024, 4, 13, 18, 36, 40)
+
+    ggkx_min_time = datetime(2023, 3, 23, 15, 15, 43)
+    ggkx_max_time = datetime(2024, 4, 13, 18, 39, 43)
+
+    # 示例用法
+    daily_availability_met = calculate_daily_data_availability(min_time, max_time, missing_intervals)
+
+    # 计算SQL_accelerometer和SQL_tiltmeter的每日数据存有率
+    daily_availability_accelerometer = calculate_daily_data_availability(accelerometer_min_time, accelerometer_max_time, missing_intervals_accelerometer)
+    daily_availability_tiltmeter = calculate_daily_data_availability(tiltmeter_min_time, tiltmeter_max_time, missing_intervals_tiltmeter)
+    daily_availability_arr = calculate_daily_data_availability(arr_min_time, arr_max_time, missing_intervals_arr)
+    daily_availability_ggkx = calculate_daily_data_availability(ggkx_min_time, ggkx_max_time, missing_intervals_ggkx)
+
+
+    # 找出最小和最大日期
+    all_dates: list[datetime] = []
+    all_dates.extend(daily_availability_met.keys())
+    all_dates.extend(daily_availability_accelerometer.keys())
+    all_dates.extend(daily_availability_tiltmeter.keys())
+    all_dates.extend(daily_availability_arr.keys())
+    all_dates.extend(daily_availability_ggkx.keys())
+
+    min_date = min(all_dates)
+    max_date = max(all_dates)
+
+    # 创建新字典并填充
+    combined_dict:dict[datetime, dict[str, float]] = {}  # 类型注解
+    for date in (min_date + timedelta(days=i) for i in range((max_date - min_date).days + 1)):
+        combined_dict[date] = {
+            'daily_arr': daily_availability_arr.get(date, 0),
+            'daily_ggkx': daily_availability_ggkx.get(date, 0),
+            'daily_met': daily_availability_met.get(date, 0),    
+            'daily_tiltmeter': daily_availability_tiltmeter.get(date, 0),
+            'daily_accelerometer': daily_availability_accelerometer.get(date, 0),
+        }
+
+    export_data_availability_to_file(combined_dict)
+
+main()
```

## Comparing `JayttleProcess-0.1.6.dist-info/METADATA` & `JayttleProcess-0.1.7.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.1.6
-Summary: modifty time:2024-04-06 23:00
+Version: 0.1.7
+Summary: modifty time:2024-04-15 23:00
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
@@ -19,11 +19,12 @@
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: wordcloud
 Requires-Dist: tqdm
 Requires-Dist: paddlepaddle
 Requires-Dist: paddlenlp
+Requires-Dist: tabulate
 
 UNKNOWN
```

