# XCrawler
A股爬虫项目
- 核心逻辑1:通过财经网址获取全部股票的动态数据，并且经过分析，将日涨，日跌超过x%的股票进行筛选，按照股票的涨跌幅进行排序；通过对股票的大额买入卖出订单进行排序，并预测前10位买入卖出的之后的大概股价，并对买入卖出进行排序；并存储到数据库(DB:Mysql，需要跟进)
- 核心逻辑2:对保留到数据库的数据按照5日，20日进行分析排序，筛选出5，20日上涨，下降的前x位的股票，进行排序，并存储到数据库(DB:Mysql)
- 核心逻辑3:做T，通过股票的涨跌幅，对股票进行T操作
1. 使用技术指标建模交易信号。比如利用布林通道、均线交叉等技术分析指标,建立买入和卖出规则。
2. 加入风险管理作为交易决策依据。比如设置止损价格和动态调整仓位,降低单日风险。
3. 采用复合指标相结合,避免单一依赖某一指标。比如结合MACD、KDJ等多 time frame 的指标信号。
4. 进行回测优化,找出参数组合效果好的交易策略。优化周期、触发点设定等策略变量。
5. 采用平滑移动平均线,避免被短期波动误导。比如用EMA作为买入信号。
6. 重点跟踪行业领跑股票,利用行业势头。同时观察大盘走势变化。
7. 使用量化选股条件排除个股风险,比如营收同比增长、获利能力等。
8. 定期回顾回测结果,调整不好的交易规则。持续优化策略模型。
9. 采取分散投资多个股票池分担风险。