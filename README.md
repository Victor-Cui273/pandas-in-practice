# pandas-in-practice
我的 Pandas 学习笔记与实践代码，涵盖 Series 和 DataFrame 的创建、操作、统计分析及多个实战案例。
# Pandas 学习笔记与实践 🐼

本仓库是我学习 Pandas 的实践记录，包含 **Series** 和 **DataFrame** 的详细用法、常用方法、统计分析以及多个贴近实际的案例。所有内容均以 Jupyter Notebook 形式呈现，适合初学者巩固基础，也方便进阶用户查阅。

## 📂 内容概览

### 1. Series 基础
- 创建：从列表、字典创建，自定义索引与名称
- 属性：`.index`, `.values`, `.shape`, `.dtype`, `.name`
- 索引：`.loc[]`, `.iloc[]`, `.at[]`, `.iat[]`，布尔索引
- 常用方法：`head()`, `tail()`, `describe()`, `count()`, `isna()`, `isin()`, `value_counts()`, `unique()`, `nunique()`, `drop_duplicates()`
- 统计：`mean()`, `std()`, `median()`, `min()`, `max()`, `sum()`, `var()`, `quantile()`, `mode()`
- 排序：`sort_values()`, `sort_index()`
- 时间序列：`pd.date_range()`, `diff()`, `pct_change()`, `resample()`, `rolling()`, `between_time()`

### 2. DataFrame 基础
- 创建：通过字典、Series 列表创建，指定 `index` 和 `columns`
- 属性：`.index`, `.columns`, `.values`, `.dtypes`, `.shape`, `.size`, `.T`
- 数据获取：
  - 单列/多列：`df['列名']`, `df[['列1','列2']]`, `df.列名`
  - 行选择：`.loc[]`（显式索引），`.iloc[]`（隐式索引）
  - 单个元素：`.at[]`, `.iat[]`
  - 头部/尾部：`head()`, `tail()`
  - 随机抽样：`sample()`
  - 布尔索引：`df[条件]`
- 常用方法：
  - 信息查看：`info()`, `describe()`, `value_counts()`
  - 缺失值：`isna()`, `isnull()`
  - 元素检查：`isin()`
  - 去重：`drop_duplicates()`, `duplicated()`
  - 替换：`replace()`
  - 累积计算：`cumsum()`, `cummin()`, `cummax()`
  - 排序：`sort_index()`, `sort_values()`, `nlargest()`, `nsmallest()`
- 列操作：新增列、删除列、基于现有列计算新列

### 3. 实战案例
- **学生成绩分析**：计算平均分、最高/低分、筛选高于平均分的学生
- **温度数据分析**：找出超过30度的天数、平均温度、温度变化最大的日期
- **商品销售统计**：计算销售额、总销售额、最高销售额产品
- **电商用户行为**：每位用户消费金额、消费金额最高用户、各类别购买数量
- **股票收益率分析**：每日收益率、波动率、收益率最高/最低日期
- **月度销售分析**：销量最高月份、月环比增长率、季度平均销量、连续增长月份
- **小时级销售分析**：按天汇总、营业/非营业时段销售额占比、滑动窗口求和

## 🚀 如何使用

1. 克隆仓库：
   ```bash
   git clone https://github.com/Victor-Cui273/pandas-in-practice.git

2. 安装依赖（推荐使用虚拟环境）：
   pip install pandas numpy jupyter

## 📌 环境要求
Python 3.x

Pandas

NumPy

Jupyter Notebook（可选）

## 🤝 贡献
如果您发现任何错误或有改进建议，欢迎提交 Issue 或 Pull Request。

## 📄 许可证
本项目采用 MIT 许可证，详情请参阅 LICENSE 文件。
