# Design Pattern

#### 介绍
总结互联网相关的设计模式组合，以及常见业务使用相应的设计模式搭配来实现代码的解耦，如工厂加策略，状态加观察者，责任链，迭代器等实现以及他们的互联网使用场景。

#### 应用
| 设计模式 | 应用场景 | 对应模块 |
| --- | --- | --- |
| 工厂策略 | 支付场景，业务接口有多种方式处理| FactoryStrategy |
| 状态观察 | 订单状态，业务存在状态转化| StateObserver |
| 责任链模式 | 投放、文件处理场景，业务有较长的处理链条且关联性不强，可将处理流程拆封成不同的责任点，并且后续扩展优秀 | ResponsibilityChain |
| 迭代器模式 | ES查询大批量数据分页查询场景，特点是不能进行页面任意跳转，必须依赖前一次查询| |
| 装饰享元| 支付后的营销活动，比如平台积分更新，红包优惠卷发放等。通过对支付接口包装，实现新功能拓展，在相应的支付门面接口上，并且减少包装类的多次创建，通过享元模式，进行单例工厂映射。 | DecoratorFlyweight|
| 模板方法| 核心审计日志记录，如用户操作记录，订单记录等||
|建造原型|开具增值发票，建造者创建个人发票和单位发票，原型模式克隆减少公共部分的创建,还有不同业务类型的多种类别创建也可以采用建造者模式|BuilderPrototype|
|桥接模式|第三方登录||
|组合访问|商品多级分类||