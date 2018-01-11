
# machine-learing-pace
# the accumulate for the machine learing
# project for part static
# word文件stroop_test_analysis_version_20180111.doc中详细公式 excel为相关计算过程和有效图表（这两个文件是重点呦）。
# background information
在一个 Stroop （斯特鲁普）任务中，参与者得到了一列文字，每个文字都用一种油墨颜色展示。参与者的任务是将文字的打印颜色大声说出来。这项任务有两个条件：一致文字条件，和不一致文字条件。在一致文字条件中，显示的文字是与它们的打印颜色匹配的颜色词，如“红色”、“蓝色”。在不一致文字条件中，显示的文字是与它们的打印颜色不匹配的颜色词，如“紫色”、“橙色”。在每个情况中，我们将计量说出同等大小的列表中的墨色名称的时间。每位参与者必须全部完成并记录每种条件下使用的时间。
# quiz for the servey
作为一般说明，请确保记录你在创建项目时使用或参考的任何资源。作为项目提交的一部分，你将需要报告信息来源。

# 1.	我们的自变量是什么？因变量是什么？
自变量为表达颜色的单词于其本身颜色的一致与否（Congruent/Incongruent），因变量为受其影响的测试人正确说出该单词的屏幕显示颜色的名称。

# 2.此任务的适当假设集是什么？你需要以文字和数学符号方式对假设集中的零假设和对立假设加以说明，并对数学符号进行定义。你想执行什么类型的统计检验？为你的选择提供正当理由（比如，为何该实验满足你所选统计检验的前置条件）。

2.1 Stroop （斯特鲁普）任务的适当假设：单词字面意思和字体显色完全一致时正确说出单词字体颜色名称的时间（Congruent），& 为单词字面意思和字体显色一致时正确说出单词字体颜色名称的时间（Incongruent）。

2.2此任务的适当假设集是什么？你想执行什么类型的统计测试？为你的选择提供正当理由。  单词字面颜色与在单词显色的颜色一致的时间的总体平均值和单词字面颜色与在单词显色的颜色不一致的时间的总体平均值。零假设未时间相同，对立假设为不一致的情况下时间不同。  
执行相依样本t检测双尾检测
#详见新上传的stroop_test_analysis_version_20180111.doc蓝色字体Jan18.
# 3.	报告关于此数据集的一些描述性统计。包含至少一个集中趋势测量和至少一个变异测量。

3.1集中趋势测量：mean  和 median ：一致时的mean = 14.051125 中位数 median  14.3565；不一致时的mean = 22.015917 中位数median = 21.0175(n=24 是升序排列取第12和13位平均值)

#3.2 以下两个数表示方式为（一致时数值，不一致时数值）

#3.2.1变异测量的值域Range （13.698，19.568）

#3.2.2变异测量的四分位差Q3-Q1 （4.686, 5.5165）

#3.2.3变异测量的样本标准差 (3.559357958, 4.797057122)

#3.2.4异常值见stroopdata 红色加粗

#3.2.5箱线图正常值max外加两点（每组各有两个异常值）

#==>详见Stroop Test.mmap文件及stroopdata.xls Excel文件

# 4.	提供显示样本数据分布的一个或两个可视化。用一两句话说明你从图中观察到的结果

可视化图见stroopdata.xls Excel文件

观察到的结果为：本样本中的单词字面意思和单词显色一致时正确读出单词的时间全都比不一致时所花费的时间短。

# 5.	现在，执行统计测试并报告你的结果。你的置信水平和关键统计值是多少？你是否成功拒绝零假设？对试验任务得出一个结论。结果是否与你的期望一致？
#5.0 t检测计算

#5.1计算 t-static = 8.020706944

#5.2计算 t-cratical = 2.069

#5.3 比较 t-static>t-cratical

#5.4查看t表p<0.05

#5.5计算Cohen's d =1.637219949 计算过程见excel表公式

#5.6从样本数据分析结果可以看出应该拒绝零假设，单词显色和字面意思不一致时会与一致时读出的时间有所差异

参考 https://www.zhengweiyu.com/2017/01/25/data-analytics-101-c9-to-c11.html
以及教程截图
