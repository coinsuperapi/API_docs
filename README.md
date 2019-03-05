# REST API

简介

```
Exchange API 是交易所面向外部开发者提供的开发接口。
```

------

更新历史

| 版本        | 时间       | 说明           | 作者     |
| --------- | -------- | ------------ | ------ |
| v1.0.1(R) | 20180626 | 增加接口：可用交易对列表 | liyong |
| v1.0.2(R) | 20190215 | 接口分类调整       | liyong |

------

## [一、全局规则](https://github.com/coinsuperapi/API_docs/wiki#%E4%B8%80%E5%85%A8%E5%B1%80%E8%A7%84%E5%88%99)

#### [接口访问前缀](https://github.com/coinsuperapi/API_docs/wiki#%E6%8E%A5%E5%8F%A3%E8%AE%BF%E9%97%AE%E5%89%8D%E7%BC%80)

#### [接口规则](https://github.com/coinsuperapi/API_docs/wiki#%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99)

##### [全局数据格式定义](https://github.com/coinsuperapi/API_docs/wiki#%E5%85%A8%E5%B1%80%E6%95%B0%E6%8D%AE%E6%A0%BC%E5%BC%8F%E5%AE%9A%E4%B9%89)

##### [签名描述](https://github.com/coinsuperapi/API_docs/wiki#%E7%AD%BE%E5%90%8D%E6%8F%8F%E8%BF%B0) 

#####  [签名生成方法示例](https://github.com/coinsuperapi/API_docs/wiki#%E7%AD%BE%E5%90%8D%E7%94%9F%E6%88%90%E6%96%B9%E6%B3%95%E7%A4%BA%E4%BE%8B) 

####  [全局通用状态码](https://github.com/coinsuperapi/API_docs/wiki#%E5%85%A8%E5%B1%80%E9%80%9A%E7%94%A8%E7%8A%B6%E6%80%81%E7%A0%81) 

## [二、详细接口定义](https://github.com/coinsuperapi/API_docs/wiki#%E4%BA%8C%E8%AF%A6%E7%BB%86%E6%8E%A5%E5%8F%A3%E5%AE%9A%E4%B9%89)

### [接口分组及限流](https://github.com/coinsuperapi/API_docs/wiki#%E6%8E%A5%E5%8F%A3%E5%88%86%E7%BB%84%E5%8F%8A%E9%99%90%E6%B5%81)

### [API 接口定义](https://github.com/coinsuperapi/API_docs/wiki#api-%E6%8E%A5%E5%8F%A3%E5%AE%9A%E4%B9%89)

#### [1.行情](https://github.com/coinsuperapi/API_docs/wiki#1%E8%A1%8C%E6%83%85)

##### [1.1 深度行情(最新深度图数据)](https://github.com/coinsuperapi/API_docs/wiki#11-%E6%B7%B1%E5%BA%A6%E8%A1%8C%E6%83%85%E6%9C%80%E6%96%B0%E6%B7%B1%E5%BA%A6%E5%9B%BE%E6%95%B0%E6%8D%AE)

##### [1.2 价格行情(最新订单簿数据)](https://github.com/coinsuperapi/API_docs/wiki#12-%E4%BB%B7%E6%A0%BC%E8%A1%8C%E6%83%85%E6%9C%80%E6%96%B0%E8%AE%A2%E5%8D%95%E7%B0%BF%E6%95%B0%E6%8D%AE)

##### [1.3 分时行情(最新K线数据)](https://github.com/coinsuperapi/API_docs/wiki#13-%E5%88%86%E6%97%B6%E8%A1%8C%E6%83%85%E6%9C%80%E6%96%B0k%E7%BA%BF%E6%95%B0%E6%8D%AE)

##### [1.4 实时成交行情（最新成交行情数据）](https://github.com/coinsuperapi/API_docs/wiki#14-%E5%AE%9E%E6%97%B6%E6%88%90%E4%BA%A4%E8%A1%8C%E6%83%85%E6%9C%80%E6%96%B0%E6%88%90%E4%BA%A4%E8%A1%8C%E6%83%85%E6%95%B0%E6%8D%AE)

#### [2.交易](https://github.com/coinsuperapi/API_docs/wiki#2%E4%BA%A4%E6%98%93)

##### [2.1 买入委托](https://github.com/coinsuperapi/API_docs/wiki#21-%E4%B9%B0%E5%85%A5%E5%A7%94%E6%89%98)

##### [2.2 卖出委托](https://github.com/coinsuperapi/API_docs/wiki#22-%E5%8D%96%E5%87%BA%E5%A7%94%E6%89%98)

##### [2.3 取消委托](https://github.com/coinsuperapi/API_docs/wiki#23-%E5%8F%96%E6%B6%88%E5%A7%94%E6%89%98)

##### [2.4 批量取消委托](https://github.com/coinsuperapi/API_docs/wiki#24-%E6%89%B9%E9%87%8F%E5%8F%96%E6%B6%88%E5%A7%94%E6%89%98)

#### [3.查询](https://github.com/coinsuperapi/API_docs/wiki#3%E6%9F%A5%E8%AF%A2)

##### [3.1 获取个人资产信息](https://github.com/coinsuperapi/API_docs/wiki#31-%E8%8E%B7%E5%8F%96%E4%B8%AA%E4%BA%BA%E8%B5%84%E4%BA%A7%E4%BF%A1%E6%81%AF)

##### [3.2 查询委托单状态(根据委托单号)](https://github.com/coinsuperapi/API_docs/wiki#32-%E6%9F%A5%E8%AF%A2%E5%A7%94%E6%89%98%E5%8D%95%E7%8A%B6%E6%80%81%E6%A0%B9%E6%8D%AE%E5%A7%94%E6%89%98%E5%8D%95%E5%8F%B7)

##### [3.3 查询订单交易详情(根据委托单号)](https://github.com/coinsuperapi/API_docs/wiki#33-%E6%9F%A5%E8%AF%A2%E8%AE%A2%E5%8D%95%E4%BA%A4%E6%98%93%E8%AF%A6%E6%83%85%E6%A0%B9%E6%8D%AE%E5%A7%94%E6%89%98%E5%8D%95%E5%8F%B7)

##### [3.4 挂单单号列表(个人未完全成交委托单列表)](https://github.com/coinsuperapi/API_docs/wiki#34-%E6%8C%82%E5%8D%95%E5%8D%95%E5%8F%B7%E5%88%97%E8%A1%A8%E4%B8%AA%E4%BA%BA%E6%9C%AA%E5%AE%8C%E5%85%A8%E6%88%90%E4%BA%A4%E5%A7%94%E6%89%98%E5%8D%95%E5%88%)

##### [3.5 查询个人历史委托单列表](https://github.com/coinsuperapi/API_docs/wiki#35-%E6%9F%A5%E8%AF%A2%E4%B8%AA%E4%BA%BA%E5%8E%86%E5%8F%B2%E5%A7%94%E6%89%98%E5%8D%95%E5%88%97%E8%A1%A8)

##### [3.6 查询个人历史成交列表](https://github.com/coinsuperapi/API_docs/wiki#36-%E6%9F%A5%E8%AF%A2%E4%B8%AA%E4%BA%BA%E5%8E%86%E5%8F%B2%E6%88%90%E4%BA%A4%E5%88%97%E8%A1%A8)

##### [3.7 可交易的交易对列表](https://github.com/coinsuperapi/API_docs/wiki#37-%E5%8F%AF%E4%BA%A4%E6%98%93%E7%9A%84%E4%BA%A4%E6%98%93%E5%AF%B9%E5%88%97%E8%A1%A8)

------

## 联系我们

```
如需帮助请加入以下API问题交流群（加入申请备注：API+coinsuper账号）：
1.QQ群：472488338 
2.Telegram电报群：https://t.me/joinchat/HEgiSxBKVx6nwQ33otJ3Zg
```