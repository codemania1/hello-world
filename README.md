# hello-world
测试用新项目。 New project for test.
- Item 1
- Item 2

```
graph TB
    A(浦发权益领取页面)-->|跳转至权益选择页面|B{基于主机性能的欧飞流控机制}
B-->|超出负载能力|B1((流控提示页面))
B-->|负载能力可以满足|B2{判断是否已达到领取上限}
B2-->|已到权益领取上限|B3(提示权益已领完,请下次尝试领取)
B2-->|未达到权益领取上限|C[欧飞权益选择页面]
C-->|选择并确认领取权益类型|C2{判断是否已达到领取上限}
C2-->|已到权益领取上限|B3((提示权益领取完毕))
C2-->|未达到权益领取上限|D[进入充值]
D-->|发起支付兑换请求|E{是否成功充值}
E-->|成功|F((提示成功))
E-->|失败|E1[冲正]
E1-->|发起退款冲正请求|E2((冲正成功))
```
