# J006 Vue+SpringBoot租房推荐交流可视化系统、带KNN推荐和条件推荐+支付功能+管理端

> 完整项目收费，可联系QQ: 81040295 微信: mmdsj186011 注明从git来的，谢谢！
也可以关注我的B站： 麦麦大数据 https://space.bilibili.com/1583208775
> 

关注B站，有好处！
编号:  J006
KNN推荐+条件推荐
## 视频
https://www.bilibili.com/video/BV17ArpYvEEk/
## 1 系统简介
Vue + Spring Boot 租房推荐互动交流可视化系统"是一个功能完善的租房信息平台，提供用户端的房源浏览、个性化推荐功能（基于用户房屋偏好和房屋特征的协同过滤算法），同时具备强大的后台管理能力，便于管理员维护房源信息和用户数据。特别值得一提的是，系统通过"可视化"模块，将房源信息、用户交互数据、租金趋势等多维度数据以直观、美观的方式呈现，极大地辅助用户分析租房市场动态、理解用户需求及房屋供需趋势。技术栈上采用Vue.js和Spring Boot，典型的前后端分离架构，有利于提升开发效率和系统扩展性。
## 2 功能设计
本租房推荐互动交流可视化系统采用经典的前后端分离架构设计，以提供高效、可扩展且用户体验良好的应用。用户通过浏览器作为客户端访问系统，浏览器负责渲染由Vue前端提供的用户界面（UI）。Vue前端基于HTML、CSS、JavaScript，利用Vuex管理全局状态、Vue Router实现页面路由，Echarts组件则用于构建丰富的可视化数据图表，从而呈现主页、房源推荐、可视化分析等功能。前端通过异步通信（如Ajax）与Spring Boot后端进行数据交互。Spring Boot后端作为业务逻辑层，负责处理前端请求，包括房源推荐算法（基于用户房屋偏好和房屋特征的协同过滤）、数据查询、管理操作等，并通过MyBatis-Plus框架简化ORM操作，高效地对底层MySQL数据库进行数据访问和持久化，存储并管理所有房源信息、用户数据以及互动信息。这种分层设计确保了系统的模块化、高内聚低耦合，便于开发、部署和维护。
### 2.1系统架构图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/7ba661587d694dbeb8a77dc7120d2ee2.png)
### 2.2 功能模块图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/1008934773a34c18a48c95b4ea941e8d.png)
### 2.3 配套文档 2.2万字
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/3ab4ad69a06d41acbb1f99f7c25b17b4.png)

### 2.4 项目目录
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b85039caf0814b6aa6f0eabc3a9dfa5d.png)
## 3 网站 功能展示
### 3.1 登录 & 注册
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/eedf752b7dfd463dabd46142ec8dcf5c.png)
### 3.2 主页 & KNN 推荐算法
提供网站的整体KNN推荐算法，根据原理为用户推荐租房房源信息。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e55ed41283844904933f47c4293930e4.png)
### 3.3 条件推荐算法
这是系统的核心功能之一。利用 物品协同过滤 (ItemCF) 算法为用户推荐租房房源，结合用户给出的条件比如价格、房屋朝向等因素为用户推荐最符合心意的房子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d2db58aebdd54fbf9033d768154357bb.png)
### 3.4 可视化分析
- 小区分析: 以花瓣图、柱状图、折线图图表等可视化方式展示小区等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f9bb0ce7358b46c1813d88d53d46376b.png)
- 价格分析: 以漏斗图、仪表盘、柱状图可视化展示房屋价格度趋势等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/05bfddd770ae472d9f1c94186e9f95d9.png)
### 3.5 词云分析
词云分析: 对房源信息进行文本分析，生成词云图，直观展示中高频出现的关键词，帮助用户快速了解主题或风格。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c68b91fc308b40a1a162c723af4a9f9b.png)
### 3.6 修改密码
提供用户更改密码的功能。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2b90a18474cd4ea9964dd807ddffabc6.png)
### 3.7 数据查询
允许用户根据关键词、等条件查询音乐信息。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e1ba4c8b528b44278b3f55d3c4d22f78.png)
### 3.8 个人中心
### 3.9 详情页面
### 3.9.1 详细信息
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2283b3c7a7ad42eebf072805c86e35db.png)
### 3.9.2 评分
通过评分控件实现对 的评分，评分是0~5分
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/380bfba9b7e5406aad4309cab8b49373.png)
### 3.9.3 收藏
房源支持收藏。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6d052ec1f98e4255a9f2536c17a86bdd.png)
### 3.9.4 支付
可以下单定金预定房源。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/515038bf9e6c428aa9c9a4a023d96730.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4fb068fbb1c64b55ad7366cee843805b.png)
### 3.10 评价房东
租客可以对房东进行评价。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f7dd3ee51905448e97077a0faa60e21e.png)
### 3.11 个人信息修改
支持信息修改。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c418ca8237e44b9da96184f52fe8eb2f.png)
### 3.12 交流平台
支持在网站上直接进行交流，为租客和房东提供一个互相沟通的平台。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e2f7d43659584fcea31c7c0ebdde41de.png)
### 3.13 订单中心
查看自己的租房订单。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5d0fa33615a9469f91f3b0fc9a61e427.png)
## 4 管理系统 功能展示
### 4.1 登录 
该模块主要面向系统管理员，用于对网站内容、用户和数据进行管理和维护。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9fa68d74ddd54ea1b5d81ae8d7a5d440.png)
### 4.2 主页
查看目前系统运行情况的统计，还可以通过图形分析目前用户的来源【饼图】，以及用户性别【柱状图图】
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f0080dcf97f448cab3e9639ae2c3efc5.jpeg)

### 4.3 管理个人信息
用户可以自行管理和修改个人资料，如昵称、头像、密码等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b0edc29af3f24f6baddc6d2d1c4d2e89.png)
### 4.4 权限
 对系统用的权限进行管理
 ![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9258ad27792c484d91602188909c1375.png)
### 4.5 用户管理
对系统用户进行管理。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e228da0fc111480c9d35cbd355c9ec32.png)

### 4.6 房源管理
 对专辑信息进行管理，包括专辑名称、发行日期、简介、封面等。
 
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2ae457c4a8a249c48ecc47a59c6c203f.png)
## 5 程序代码
### 5.1 代码说明
代码介绍：类定义：HouseRecommender 类用于处理推荐逻辑，包含房源数据和用户偏好。House 类表示房源信息，包括ID、租金、朝向和装修情况。
初始化：在构造函数中，初始化房源数据和用户偏好，并设置各推荐因素的权重。
相似度计算：calculate_similarity 方法计算房源与用户偏好的综合得分，基于租金、朝向和装修的匹配程度。
单因素评分计算：
_calculate_rent_score：根据房源租金是否在用户预算范围内，计算租金得分。
_calculate_orientation_score：检查房源朝向是否在用户偏好的朝向列表中。
_calculate_decoration_score：检查房源装修是否在用户偏好的装修列表中。
推荐生成：get_recommendations 方法对房源进行评分、排序，并返回前N个推荐房源。
示例使用：展示如何创建房源数据和用户偏好对象，使用推荐算法生成推荐房源，并输出结果。
### 5.2 流程图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2b361c710a0b4a7d9eebca5bed998c58.png)

### 5.3 代码实例
```java

class HouseRecommender:
    def __init__(self, houses, userPreferences):
        self.houses = houses
        self.userPreferences = userPreferences
        # 定义各个因素的权重
        self.weight_rent = 0.5
        self.weight_orientation = 0.3
        self.weight-decoration = 0.2

    def calculate_similarity(self, house):
        # 计算租金相似度
        rent_score = self._calculate_rent_score(house['rent'])
        # 计算朝向相似度
        orientation_score = self._calculate_orientation_score(house['orientation'])
        # 计算装修相似度
        decoration_score = self._calculate_decoration_score(house['decoration'])
        # 加权求和
        total_score = (self.weight_rent * rent_score +
                      self.weight_orientation * orientation_score +
                      self.weight-decoration * decoration_score)
        return total_score

    def _calculate_rent_score(self, house_rent):
        # 假设用户偏好租金范围为 [min_rent, max_rent]
        user_min = self.userPreferences['min_rent']
        user_max = self.userPreferences['max_rent']
        if house_rent < user_min:
            return 0.0
        elif house_rent > user_max:
            return 0.0
        else:
            # 按照线性归一化计算得分
            return (house_rent - user_min) / (user_max - user_min)

    def _calculate_orientation_score(self, house_orientation):
        # 假设用户偏好朝向为一个列表
        preferred_orientations = self.userPreferences['preferred_orientations']
        if house_orientation in preferred_orientations:
            return 1.0
        else:
            return 0.0

    def _calculate_decoration_score(self, house_decoration):
        # 假设用户偏好装修情况为一个列表
        preferred_decorations = self.userPreferences['preferred_decorations']
        if house_decoration in preferred_decorations:
            return 1.0
        else:
            return 0.0

    def get_recommendations(self, num_recommendations=5):
        scored_houses = []
        for house in self.houses:
            score = self.calculate_similarity(house)
            scored_houses.append((house, score))
        # 按照得分排序，降序
        scored_houses.sort(key=lambda x: x[1], reverse=True)
        # 返回前num_recommendations的房源
        return [house for house, score in scored_houses[:num_recommendations]]

class House:
    def __init__(self, id, rent, orientation, decoration):
        self.id = id
        self.rent = rent
        self.orientation = orientation
        self.decoration = decoration

# 示例使用
if __name__ == "__main__":
    # 示例房源数据
    houses = [
        House("H1", 2000, "南", "豪华"),
        House("H2", 2500, "北", "简单"),
        House("H3", 1800, "西", "中等"),
        House("H4", 2200, "南", "中等"),
        House("H5", 3000, "东", "豪华"),
    ]
    
    # 示例用户偏好
    user_preferences = {
        'min_rent': 1800,
        'max_rent': 2500,
        'preferred_orientations': ['南', '东'],
        'preferred_decorations': ['中等', '豪华']
    }
    
    recommender = HouseRecommender(houses, user_preferences)
    recommended_houses = recommender.get_recommendations(3)
    
    print("推荐的房源：")
    for house in recommended_houses:
        print(f"ID: {house.id}, 租金: {house.rent}, 朝向: {house.orientation}, 装修: {house.decoration}")

```
