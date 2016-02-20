中国城市三级联动菜单 (Redis)
==

开发中经常遇到城市三级联动菜单的问题。我的解决办法是将这些数据存在redis中，然后处理，既不需要前端存储大量数据，又能保障查询速度。

这个Repo负责将该数据初始化到Redis中。

而此Ropo的城市数据来源于京东(jd.com)。


运行
==
```
npm install
```

All data
--
### places
##### [places.json] 中是中国所有城市与地区的Json数据,其中

* name 是城市（地区）名称
* id 是它在文件中的唯一标识
* pid 是它的上级行政机构的名称
详情参见 https://github.com/rickytan/AllCities

##### [places_parser.js] 将 [places.json]

```
```
[places.json]: ./places.json
[places_parser.js]: ./places_parser.js
