Cywin
========

这是创业赢的源代码: <http://cywin.cn>

专门用于体验的环境( 随便折腾 ): <http://staging.cywin.cn>, 用户名: admin@cywin.cn, 密码: admin

创业赢是一个股权众筹平台, 通过集合优秀的天使投资人领投, 联合普通投资人来帮助初创企业完成天使轮融资的全流程线上平台. 其国外的对手如: [angellist](https://angel.co), 国内的对手如: [天使汇](http://angelcrunch.com), [创投圈](http://vc.cn/) 等.

其核心流程如下:

1. 创业者

    创建项目 -> 发布项目 -> 发布融资预热 -> 邀请领投人 -> 领投人确认 -> 投资人投资 -> 成功融资

2. 普通投资人

    申请为认证投资人 / 跟投项目

3. 认证投资人

    领投项目 / 制定投资规则


## 为什么把创业赢开源?

在花费 6 个月的时间打磨这个产品后, 我才意识到, 我与合伙人根本无法单凭线上渠道运作起来这个平台, 线下渠道极为有限, 我觉得在中国这个市场, 无法继续存活下去, 它已经耗费了我所有的精力.

与合伙人在下一步产品理念上的冲突, 迟迟未获取的正反馈, 使得我最终决定退出该项目.

几个月之后, 在我得知项目源码已经不再继续开发时, 我决定将其开源. 希望它还能够帮助一些对其感兴趣的朋友.

## 这个项目还会继续维护吗?

我不再打算在毫无前景的情况下继续开发, 虽然项目是一个人开发, 并且一直压力很大, 但这个项目拥有非常良好的架构与可持续开发能力, 它的测试仍然非常完整( 120+ ), UI 非常漂亮( 花费上万的设计费 ), 并且还支持响应式, 更加给力的是, 前端没有丑陋的 jQuery 代码, 而是利用 AngularJS 组织的非常清晰.

整体而言, 这是我目前最为满意的一个作品, 可持续开发能力非常强, 当然对维护者的能力要求也比较高.

## 我能得到你的帮助吗?

如果你在学习甚至打算基于此系统二次开发, 我都非常乐意. 你的问题可以提交到 github 的 issues 中, 我在业余时间可以尝试帮助你解决.

## 最值得参考的点

* 消息机制( 模板与邮件推送 )
* 登录功能( 定制 Devise / 邀请注册 / 注册码 )
* 角色管理( 权限管理 )
* AngularJS 与 Rails 的混合模式最佳实践
* AngularJS 组件化开发
* 响应式开发
* SCSS 代码组织结构
* RESTful Controller 设计
* 分离环境的自动发布系统( staging / demo / production )
* 搜索功能
* 业务逻辑的 TDD 测试开发
* 配置文件的组织结构

## 核心技术栈

* Ruby on Rails( 4.1 )
* AngularJS( 混合模式 )
* Foundation 5

## 安装配置

0. `gem install bundler`
1. `bundle install`
2. 复制 config/xx.example.yml 到 config/xx.yml, 并根据需要调整配置.
3. `rake db:setup`
4. `rails s`

可选配置 sunspot.

根据你 config/application.yml 的配置的 ADMIN_EMAIL 和 ADMIN_PASSWORD 登录 Cywin.

## 发布历史记录

### 2014.10.20

项目宣布退出

### 2014.9.15

发布新 UI

完善功能

### 2014.8.16

重构了分类

完善功能

### 2014.8.6

重构了首页

完善调整功能

### 2014.4.15

重构了所有页面, 适应于手机

基本功能已完成

### 2014.3.26

项目选型

-----------------

## 授权

本系统遵守 [MIT](http://www.opensource.org/licenses/mit-license.php) 和 [GPL](http://www.gnu.org/licenses/gpl.html) 双重授权.

额外地, 系统中 Logo 等图片资源不得用于商业目的.
