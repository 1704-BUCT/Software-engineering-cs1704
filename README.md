### api接口文档

#### 1.前言

1. 服务器地址：39.97.241.101
2. 用户名：Administrator
3. 密码：
4. （如果密码被和谐了来私聊我）
5. 目前服务器上已配置apach-tomcat、mysql。已有部分数据。
6. 以http://+ip+port+url的格式访问，如：http://39.97.241.101:8080/museum/{id}
7. 用url里用大括号{}括起来的表示直接写数据，如：http://39.97.241.101:8080/museum/1
8. 这里序号都从1开始，没有0号！
9. 返回数据里删除线表示还未实现的数据.

#### 2.目前可用接口表
api快捷查找表

Museum

| 功能                     | url                           | 返回类型 |
| ------------------------ | ----------------------------- | -------- |
| 根据博物馆id获得博物馆信息 | /museum/findByMid/{id}    | List     |
| 返回所有博物馆信息         | /museum/findAll           | List     |
| 根据藏品名字查找         | /museum/findByName/{name} | List     |

Collection

| 功能                     | url                           | 返回类型 |
| ------------------------ | ----------------------------- | -------- |
| 根据博物馆id获取藏品信息 | /collection/findByMid/{id}    | List     |
| 返回所有藏品列表         | /collection/findAll           | List     |
| 根据藏品名字查找         | /collection/findByName/{name} | List     |


Comment

| 功能                         | url                         | 返回类型 |
| ---------------------------- | --------------------------- | -------- |
| 根据博物馆id查找评论         | /comment/findByMid/{mid}    | List     |
| 用户是否已经给某博物馆评论过 | /coment/already/{uid}/{mid} | 1/0      |
| 上传评论                     | /comment/update             |          |

Education

| 功能                     | url                          | 返回类型 |
| ------------------------ | ---------------------------- | -------- |
| 根据博物馆id返回教育活动 | /education/findByMid/{id}    | List     |
| 返回所有教育活动         | /education/findAll           | List     |
| 根据名字搜索             | /education/findByName/{name} | List     |

Exhibition
| 功能                     | url                          | 返回类型 |
| ------------------------ | ---------------------------- | -------- |
| 根据博物馆id返回展览 | /exhibition/findByMid/{id}    | List     |
| 返回所有展览        | /exhibition/findAll           | List     |
| 根据名字搜索             | /exhibition/findByName/{name} | List     |

News
| 功能                     | url                          | 返回类型 |
| ------------------------ | ---------------------------- | -------- |
| 根据博物馆id返回新闻 | /news/findByMid/{id}    | List     |
| 返回所有新闻        | /news/findAll           | List     |
| 根据名字搜索             | /news/findByName/{name} | List     |

CollectionExplanation

| 功能                     | url                                    | 返回类型 |
| ------------------------ | -------------------------------------- | -------- |
| 根据博物馆id查找藏品讲解 | /collectionExplanation/findByMid/{mid} | List     |

ExhibitionExplanation

| 功能                     | url                                    | 返回类型 |
| ------------------------ | -------------------------------------- | -------- |
| 根据博物馆id查找展览讲解 | /exhibitionExplanation/findByMid/{mid} | List     |
