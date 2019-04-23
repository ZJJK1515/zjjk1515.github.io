读取类路径下 properties 文件的方式：

```java
ResourceBundle bundle = ResourceBundle.getBundle("文件名");
bundle.getString(key);
```

> 1. 只能用于读取 properties 文件
> 2. 只能用于读取，不能写入
> 3. 只能读取类路径下
> 4. 命名方式是包名.类名，所以不需要后缀名



Inverse of control

控制反转，把创建对象的权利交给 Spring，降低依赖关系，实现解耦。



BeanFactory: 延迟加载，获取对象时生成对象

ApplicationContext:立即加载，读取完配置文件后生成对象