## 1.接口规范介绍
本接口规范对xxx接口操作、相关参数、响应和错误码进行定义，所有提交及返回接受的变量均使用小写。目前支持REST APP,并提供接口操作请求和响应规范

## 2.REST错误响应
所有访问当出现错误时，HTTP响应包含以下header信息：
> * content-type:application/json
> * http响应码：1xx,2xx,3xx,4xx,5xx
> * http body包含具体错误描述信息，列：
```
{"error":{"code":404,"message":"NOT FIND"}}
```
## 3.接口分类
#### * 接口说明:
> 用户登录
#### * URL:
> `api/user/login`
#### * HTTP请求方式：
> post
#### * 请求headers:
> data
| 参数名称 | 类型 | 参数描述 |
|:---|:---|:---|
| username | string | 用户名 |
| password | string | 密码 |
#### * 示例：
> * 请求：
`url:`
> * 响应：
```
{}
```
## 4.其他
## 5.修订历史
#### 
| 版本号 | 作者 | 时间 | 内容 |
|:-------|:----|:-----|:-----|
| 0.1 | lsq | 2018.04.23 | 创建：接口定义规范 |
