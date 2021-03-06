# 探索构建数据中心碳交易协议(DCCC)

From [Meson Network](https://meson.network/)

## 摘要

数据中心在现代数字经济活动中具有举足轻重的地位。伴随数字经济的蓬勃发展，数据中心的建设也进入了快车道。在数据中心大量建设并投入使用的过程中，人们发现由于摩尔定律的限制，数据传输的增加需要消耗越来越多的能源。同时全球正受到气候变暖的威胁，每个国家都积极投入到减少碳排放的工作中，但数据中心日渐增长的能源消耗与控碳减排的目标形成了一对根本的矛盾。

我们通过考察和设计，尝试提出 DCCC 作为数据中心碳交易的媒介，Meson 成为第一个支持该积分落地应用的平台。Meson 作为基于通证激励以及去中心化的区块链技术的带宽统筹平台，不仅可以有效的将存量闲置资源通过通证激励利用起来，跨国境，跨区域，跨项目的统筹协调带宽资源，同时还能鼓励更多超大型数据中心的建设。这使得数据中心的建设既能满足现代科技的发展，同时也迎合了各地节能减排的需求，在碳排放的硬约束下为数字经济的发展铺下了坚实高效的地基。

## 碳排放与 IDC 背景

### 数据中心在数字经济的重要性

数据中心可以被认为是互联网的“大脑”。它们的作用是处理、存储和交流我们每天依赖的无数信息服务背后的数据，无论是流媒体视频、电子邮件、社交媒体、在线协作还是科学计算。数字服务是能源使用增加的主要原因。对数字服务的需求一直在稳步增长，随之而来的是其基础设施的发展。随着基础设施的增加，对更多能源的需求也在增加。

### 数据中心耗能情况

数据中心已经估计每年使用 200 太瓦时 (TWh)。这超过了包括伊朗在内的一些国家的国家能源消耗，但占全球运输用电量的一半，占全球电力需求的 1%。数据中心对整体碳排放的贡献约为 0.3%。

ICT 的碳足迹与航空业的燃料排放量持平。未来可能发生的事情很难预测。但最令人担忧的模型之一预测，当今天出生的孩子长到十几岁时，信息通信技术的用电量可能会超过全球总量的 20%，而数据中心使用的电量超过三分之一。

![](./assets/01.png)

![](./assets/02.png)

在过去的几年中，已经发布了许多能源消耗报告。国际能源署 (IEA) 报告称，2021 年工作负载和互联网流量将翻一番，但由于效率提高，数据中心的能源需求将保持平稳。

然而，一些报道驳斥了这一说法。Uptime Institute Intelligence 表示，推动数据中心能源消耗的因素非常强大。有些数据甚至与 IEA 的数据相矛盾。例如，IEA 报告称，2018 年全球数据中心能耗为 197.8 TWh，2021 年略有下降。但欧盟资源效率协调行动（EURECA）项目表示，欧洲数据中心在 2017 年消耗了 130 TWh，而绿色和平组织估计2018年中国数据中心的能耗为160 TWh，这意味着仅中国和欧洲就消耗了290 TWh，远高于IEA提供的数据。（https://journal.uptimeinstitute.com/data-center-energy-use-goes-up-and-up/)。

在美国数据中心，收益递减规律可能开始限制节能的影响。例如，在数据中心层面，热/冷通道封闭、安装盲板和提高设定点温度等最佳实践已经广泛部署；这可以从 2011 年至 2014 年电源使用效率 (PUE) 的大幅下降中看出。 然而，自 2014 年以来，PUE 并没有大幅下降，而在 2019 年，注意到受访者向我们报告的年均 PUE 略有上升全球数据中心调查。同样，对于 IT 硬件，摩尔定律已经放缓，更新的服务器无法保持过去看到的相同效率改进。

Uptime Institute 预计 IT 行业的强劲增长将在未来五年内持续下去，因为人们已经充分了解需求模式，并且现有技术将被大规模采用。IT 能源消耗也将稳步上升，到 2020 年将增加多达 10%。

### 驱动数据中心耗能的因素

这种需求的增加是云、托管和一些企业数据中心中更多基础设施和更多能源消耗的重要驱动因素——尽管不是唯一的驱动因素。但一个新的因素尚未发挥作用：5G。

虽然 5G 的进一步成熟和普及还需要几年时间，但 2020 年 5G 的推出大大加快数据增长趋势，在智慧城市、物联网等领域出现许多新型数字服务和交通，等等。与 4G 相比，带宽增加将导致对更高分辨率内容和更丰富的媒体格式（例如虚拟现实）的需求在 2020 年末增加，此后随着能源消耗的增加而急剧增加。

社交媒体提供了另一个不受控制的能源使用的例子。 Uptime Intelligence 的研究表明，每当葡萄牙足球明星克里斯蒂亚诺·罗纳尔多（Cristiano Ronaldo）（在撰写本文时在该平台上拥有最多的追随者）在 Instagram 上发布图片时，他超过 1.88 亿的追随者都会消耗超过 24 兆瓦时（ MWh) 的能量来查看它。

流媒体占全球流量的比例最大，并且在全球范围内稳步上升，已成为互联网的耗能大户。流式传输 2.5 小时的高清 (HD) 电影会消耗 1 千瓦时 (kWh) 的能量。但对于 4K（超高清）流媒体——在 2020 年开始成为主流——这将接近 3 千瓦时，增加了三倍。

## 协议提出及设计

我们尝试去思考数据中心本身对全球碳排放造成的影响，穿透到底层是两方面。第一是数据中心的建设过程会产生碳排放，第二是对数据中心的日常使用会产生碳排放。

建设过程会涉及到原材料（如钢材、水泥等）的生产、消耗人力、对当地土地植被自然资源的破环等方面，可以抽象成建筑建设的碳排放，遵从各国各地标准。这边着重讨论对于数据中心的日常使用所产生的碳排放。

我们先来看下对于一个数据中心，其日常使用所消耗的资源构成。大体分成几个部分，包括 IT 设备，冷却系统，照明及其他附属部分。

![](./assets/03.png)

服务器的运行需要保持在一定温度限制里，做计算时会消耗大量的能量并释放热量，所以需要冷却系统持续把热量给排出。对于数据中心能效指标，有统一参数叫 PUE:


> PUE 是 Power Usage Effectiveness的简写，是评价数据中心能源效率的指标，是数据中心消耗的所有能源与IT负载使用的能源之比，是DCIE(data center infrastructure efficiency)的反比。

> PUE = 数据中心总设备能耗/IT设备能耗，PUE是一个比值，基准是2，越接近1表明能效水平越好

> PUE(PowerUsageEffectiveness，电源使用效率)值已经成为国际上比较通行的数据中心电力使用效率的衡量指标。PUE值是指数据中心消耗的所有能源与IT负载消耗的能源之比。PUE值越接近于1，表示一个数据中心的绿色化程度越高。


对于冷却系统，现在主流的大致有三种方案:


> **关于数据中心不同冷却系统的概览**

> 基于空气的冷却系统会向服务器机房供应冷空气。服务器机架通常布置在所谓的“冷”和“热”通道中，以控制气流并消除冷热空气混合。由于热容量和传热系数低，空气不是一种很好的传热介质，导致能耗高，服务器的紧凑程度受到限制，废热温度相对较低。

> 基于液体的冷却系统使用诸如水之类的液体来散热。这可以通过在微通道中循环水并在与服务器组件直接接触的冷板式热交换器中交换热量来实现。与空气相比，水和液体通常具有明显更好的传热性能。基于液体的冷却系统使得更紧凑的数据中心成为可能，并减少用于冷却的能源使用和获得更高的废热温度。

> 两相冷却是一种新兴的数据中心冷却技术形式。液体冷却剂在冷板式换热器中蒸发，耗散的能量作为以热能方式储存。这使得更大的热通量和冷却剂进行温度调整，并使具有更高计算密度的系统成为可能。


围绕 PUE 这个核心能耗参数，我们希望可以鼓励世界建造、使用和升级对环境更友好的数据中心，并限制能耗较差的节点。

由此，我们提出一套世界数据中心碳排放积分（DCCC）。对于 PUE 指标不达标的数据中心，需要购买一定数量 DCCC 来抵消其碳足迹，而对于 PUE 较优秀的节点，则可以向市场销售其 DCCC。

第二个比较重要的参数是使用率。世界各地建完的数据中心，使用率差异较大。对于 PUE 较好而使用率不高的数据中心，可以把闲置资源接入一些资源共享的市场（如 MESON）来获取 DCCC，通过出售 DCCC 获取额外收益。对于 PUE 较差的数据中心，需要向市场购买 DCCC，也可以把闲置的资源拿去分享来抵扣 DCCC 差值。

![](./assets/04.png)

除了上部分提到的两个PUE和使用率，还有一个重要参数是供给数据中心的能源结构。在协议未来的发展过程中，我们也考虑把供电的能源结构引入作为 DCCC 的参数。

## DCCC 使用场景

MESON 会成为第一个支持 DCCC 使用的市场。MESON 尝试解决带宽资源闲置的问题，并自下而上构建了一个带宽聚合和交易的市场。

PUE 达标的节点可以贡献资源在 MESON 网络来获取一定数量的 DCCC，PUE 未达标的节点通过贡献资源到 MESON 网络来获取 DCCC 差额。

DCCC 会成为在 MESON 里交易资源的一个重要参数，对于 DCCC 缺少的节点，其在 MESON 里交易的收益和排名会收到一定限制。而对于 DCCC 较好的节点，其在资源置换的市场可以获得更大的优先权。我们希望给世界创造一个平台，更希望这个平台能给人类的可持续性做出贡献，通过 DCCC 尝试实现市场调节资源的供给结构。

![](./assets/05.png)

[https://www.instagram.com/p/BpPovnsFcO9/](https://www.instagram.com/p/BpPovnsFcO9/) 

## 需求侧还是供给侧买单

从资源这个维度来看碳排放，到底应该由资源的供给侧来买单还是由资源的需求、使用侧来买单。举几个例子：坐飞机，应该是由每位乘客为产生的碳足迹买单，还是由提供该航线的航司来买单；电力，应该由发电厂为碳排放买单还是由该电力的使用者买单；区块链挖矿，应该是由运行 BTC 矿机的人买单还是由使用 BTC 网络的人买单（Bitmex 购买碳积分）。我们认为，两端都要抓。对于需求侧，以鼓励自愿为主，对于供给侧，需要一定强制约束。

## 总结

我们提出在数据中心维度建立碳排放交易的协议，引入 PUE、使用率、供电结构等指标并尝试使用 DCCC 来做具体的衡量。协议本身还在早期，我们希望抛砖引玉能引入更多有志之士一起参与该协议的讨论和治理。

加入讨论：[https://github.com/daqnext/DCCC](https://github.com/daqnext/DCCC) 

## 参考资料

- [Tesla Impact Report 2020](https://www.tesla.com/ns_videos/2020-tesla-impact-report.pdf)
- [Bitcoin’s Carbon Footprint](https://blog.bitmex.com/bitcoins-carbon-footprint)
- [Bill Gates:《How to Avoid a Climate Disaster》](https://blog.sintef.com/sintefenergy/this-is-how-we-reduce-data-centers-carbon-footprint/)
- [Trends in Data Centre Energy Consumption under the European Code of Conduct for Data Centre Energy Efficiency](https://www.mdpi.com/1996-1073/10/10/1470)
- [How to stop data centres from gobbling up the world’s electricity](https://www.nature.com/articles/d41586-018-06610-y)