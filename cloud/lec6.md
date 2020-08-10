class: middle, center

### AI技术和云技术在视频监控中的应用

# 流式计算模型

陈一帅

[yschen@bjtu.edu.cn](mailto:yschen@bjtu.edu.cn)

北京交通大学电子信息工程学院

.footnote[铁路综合视频监控维护管理培训班]

---
# 内容

- .red[定义]
- 原理
- 系统
---

# 流式计算模型

- 实时或近实时分析变得越来越关键
  - 视频流
  - 物联网
- 分析来自无限制流的数据的活动，即数据流分析
- 可追溯到 1990 年代在斯坦福，加州理工学院和剑桥等地进行的复杂事件处理的基础研究

???

[87] K. M. Chandy, O. Etzion, and R. von Ammon. Event processing. Dagstuhl Seminar Proceedings 10201, Schloss Dagstuhl - Leibniz-Zentrum fuer Informatik, Germany, 2011.

is becoming increasingly critical

sensors onboard an autonomous vehicle or an energy power grid

trending topics and hashtags

activity of analyzing data coming from unbounded streams as data stream analytics.

dates back to basic research on complex event processing in the 1990s at places including Stanford, Caltech, and Cambridge [87].

---
# 内容

- 定义
- .red[原理]
- 系统

---

# 节点预分析

- 数据流的分析有时需要靠近源
- 正在出现执行预分析的工具，其目的是确定应发送到云以进行更深入分析的数据子集
- 如 Apache Edgent 边缘分析工具，能够在 Raspberry Pi 等小型系统中运行

???

analysis of instrument data streams sometimes needs to move closer to the source. Tools are emerging to perform preanalysis, with the goal of identifying the data subsets that should be sent to the cloud for deeper analysis. For example, the Apache Edgent edge-analytics tools edgent.apache.org are designed to run in small systems such as the Raspberry Pi. Kamburugamuve and Fox [165] survey many of these stream-processing technologies,

S. Kamburugamuve and G. Fox. Survey of distributed stream processing, Feb 2016. https://www.researchgate.net/publication/299411481.

---

# 时间窗口

- 固定时间窗口：将输入流分为逻辑段，每段对应于一个指定的处理时间间隔。间隔不重叠
- 滑动窗口：允许窗口重叠。例如，窗口大小为 10 秒，每 5 秒启动一次
- 以会话为单位的窗口：将流划分为与数据的某些键相关的活动的会话（Session）。例如，某位用户的一连串鼠标点击可以捆绑到一起，作为一个时间上临近的系列点击会话
- 全局窗口：封装整个有界流

---

# 触发

- 与窗口相关联
- 触发对窗口内容的分析，并发布结果

???

Fixed time windows divide the incoming stream into logical segments, each corresponding to a specified interval of processing time. The intervals do not overlap.

Sliding windows allow for the
windows to overlap: for example, windows of size 10 seconds that start every five seconds.

Per session windows divide the stream into sessions of activity related to some key in the data. For example, mouse clicks from a particular user may be bundled into a sequence of sessions of clicks nearby in time.

Global windows can encapsulate an entire bounded stream.

Trigger

Associated with windows there must be a mechanism to trigger an analysis of the content of the window and publish the summary.

---
# 内容

- 定义
- 原理
- .red[系统]

---

# 系统

- Spark Streaming
- Apache Storm, 来自 Twitter 的 Heron
- Apache Flink，来自德国 Stratosphere 项目
- Apache Beam，来自 Google 的 Cloud Dataflow，可以在 Flink, Spark, Google 云上运行
- Amazon Kinesis
- Azure Event Hubs
- IBM Stream Analytics

???

Spark Streaming spark.apache.org/streaming , derived from the Spark parallel data analysis system described in the next chapter;

Twitter’s Storm system storm.apache.org , redesigned by Twitter as Heron [173];

S. Kulkarni, N. Bhagat, M. Fu, V. Kedigehalli, C. Kellogg, S. Mittal, J. M. Patel, K. Ramasamy, and S. Taneja. Twitter Heron: Stream processing at scale. In ACM SIGMOD International Conference on Management of Data, pages 239–250, 2015.

Apache Flink flink.apache.org from the German Stratosphere project;

Google’s Cloud Dataflow [58], becoming Apache Beam beam.apache.org , which runs on top of Flink, Spark, and Google’s Cloud.

T. Akidau, R. Bradshaw, C. Chambers, S. Chernyak, R. J. Fernández-Moctezuma, R. Lax, S. McVeety, D. Mills, F. Perry, E. Schmidt, and S. Whittle. The dataflow model: A practical approach to balancing correctness, latency, and cost in massive- scale, unbounded, out-of-order data processing. Proceedings of the VLDB Endow- ment, 8(12):1792–1803, Aug. 2015.

commercially developed systems include Amazon Kinesis aws.amazon.com/kinesis

Azure Event Hubs [31], and IBM Stream Analytics [25].

Microsoft Azure Event Hubs. https://azure.microsoft.com/en-us/services/ event-hubs/.

IBM Analytics Stream Computing. http://www.ibm.com/analytics/us/en/ technology/stream-computing/.

---

# 系统

- 亚马逊的事件流软件堆栈 Kinesis，包括三个服务
  - Kinesis Streams：提供有序的、可重播的实时流数据
  - Kinesis Firehose：支持极高规模的事件处理，可以将数据直接加载到 S3 或其他 Amazon 服务中
  - Kinesis Analytics：提供了基于 SQL 的分析工具，实时分析 Kinesis Streams 或 Firehose 中的流数据

???

Amazon Kinesis and Firehose
Amazon provides an impressive event-streaming software stack called Kinesis, comprising the following three services:

1. Kinesis Streams provides ordered, replayable real-time streaming data.

2. Kinesis Firehose, designed for extreme scale, can load data directly into S3 or other Amazon services.

3. Kinesis Analytics provides SQL-based tools for real-time analysis of stream- ing data from Kinesis Streams or Firehose.

---
# 小结

- 定义
- 原理
- 系统
