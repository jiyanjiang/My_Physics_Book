杂项/其他罗列
---



甘特图
---

```gantt
    title 项目开发流程
    section 项目确定
        需求分析       :a1, 2016-06-22, 3d
        可行性报告     :after a1, 5d
        概念验证       : 5d
    section 项目实施
        概要设计      :2016-07-05  , 5d
        详细设计      :2016-07-08, 10d
        编码          :2016-07-15, 10d
        测试          :2016-07-22, 5d
    section 发布验收
        发布: 2d
        验收: 3d
```




```mermaid
graph TD
  A[产品需求收集] --> B[需求分析]
  B --> C{是否可行}
  C -->|是| D[产品设计]
  C -->|否| A
  D --> E[开发]
  E --> F[测试]
  F --> G[发布]
```



```mermaid
gantt
  title 项目甘特图
  dateFormat YYYY-MM-DD
  section 阶段1
  任务1 :a1, 2025-07-01, 7d
  任务2 :a2, after a1, 5d
  section 阶段2
  任务3 :a3, 2025-07-15, 10d
```





```mermaid
gantt
    title Igsein AI
    tickInterval 1month
    section 视频
        第一个月    :2025-07-02, 30d
        第二个月    :31d
        第三个月    :30d
    section 产品
        市场调研    :2025-06-23, 35d
        产品说明书  :7d
    section APP DEMO
        概念初版        :2025-06-23, 14d
        概念第1版      :14d
        概念第2版      :14d
        正式DEMO 1       :28d
        正式DEMO 2       :28d
    section 天命之书
        第1-2版       :2025-06-19, 7d
        第3版       :7d
        第4版       :7d
    section 其他运营
        待定任务1    :2025-07-04, 14d
        待定任务2    :28d
        待定任务3    :42d
```
