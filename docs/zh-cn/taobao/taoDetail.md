## 基本信息
>数据描述：
>
淘宝商品详细信息查询，可应用于商品销售情况分析，电商选品分析，品牌口碑挖掘和竞争对手分析等。 因数据实时性特点，无法反查接口调取时的数据内容，请务必确认满足要求再订购。
>
>请求地址：https://taotaoapi.com/taobao/detail
>
>请求方式：get
>
>请求示例：https://taotaoapi.com/taobao/detail?num_iid=淘宝商品id&appkey=您申请的APPKEY 
>
> [点此获取APPKEY](https://www.omotool.com/)
>
## 请求参数

##### 公共请求参数

名称|类型|必填|示例值|描述
:-|-:|:-:|:-:|:-:
appkey|String  |是|1|您申请的appkey 

##### 业务请求参数

名称|类型|必填|示例值|描述
:-|-:|:-:|:-:|:-:
num_iid|String  |是|17621470828|商品ID 


## 返回参数

##### 公共返回参数

名称|类型|示例值|描述
:-|:-|:-|:-
code|String|10000|更多返回参数示例值请参看错误参照码
charge|	boolean|	false 或 true|	false：不扣费 true：扣费
remain|	long|	1305|	数据剩余次数
msg|	string|	查询成功|	更多返回参数示例值请参看“[错误参照码](zh-cn/common/code.md)”
result|	object|	{...}|	数据查询结果

##### 业务返回参数

result 中的JSON串

```json
{
    "vid":28327,
    "name":"酒红色",
    "image":"//img.alicdn.com/imgextra/i2/132691477/O1CN01FVmFIA1MmVevEk4ww_!!132691477.jpg"
}

```

