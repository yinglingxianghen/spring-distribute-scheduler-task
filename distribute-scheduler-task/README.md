## 001-distribute-scheduler-task

### 项目说明

分布式定时任务演示实例，单机版mock方案，控制单机的多个定时任务，只允许一个执行

- AOP方案： 
    - 使用之前，需要将 ScheduleDemo 的private方法，修改为public或者protected或删掉
    - 启动类 Application 中开启`@EnableScheduling` 注释 `@EnableDistributeScheduling`
- ScheduledAnnotationBeanPostProcessor 扩展方案
    - 当前默认的是这种方式，可以直接进行测试
