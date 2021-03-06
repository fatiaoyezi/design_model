设计模式

### 工厂模式

#### &emsp;&emsp;简单工厂模式

&emsp;&emsp;&emsp;&emsp;**定义**：定义一个用于创建对象的接口。 

&emsp;&emsp;&emsp;&emsp;**组成**：

* **工厂类角色**：这是本模式的核心，含有一定的商业逻辑和判断逻辑，用来创建产品；

* **抽象产品角色**：它一般是具体产品继承的父类或者实现的接口；         
* **具体产品角色**：工厂类所创建的对象就是此角色的实例，在java中由一个具体类实现。

[Java Example](https://github.com/fatiaoyezi/design_model/tree/master/src/factory/simple_factory )  

&nbsp;

#### &emsp;&emsp;工厂方法模式

&emsp;&emsp;&emsp;&emsp;**定义**：工厂可以被子类工厂继承，创建实例交给不同的子工厂 。

&emsp;&emsp;&emsp;&emsp;**组成**：

- **抽象工厂角色**： 是具体工厂角色必须实现的接口或者必须继承的父类，在Java中它由抽象类或者接口来实现；

- **具体工厂角色**：它含有和具体业务逻辑有关的代码，由应用程序调用以创建对应的具体产品的对象；         
- **抽象产品角色**：它是具体产品继承的父类或者是实现的接口，在Java中一般由抽象类或者接口来实现；
- **具体产品角色**：具体工厂角色所创建的对象就是此角色的实例，在Java中由具体的类来实现。 

[Java Example](https://github.com/fatiaoyezi/design_model/tree/master/src/factory/factory_mothed )

&nbsp;

#### &emsp;抽象工厂模式

&emsp;&emsp;&emsp;&emsp;**定义**：

&emsp;&emsp;当每个抽象产品都有多于一个的具体子类的时候，工厂角色怎么知道实例化哪一个子类呢？比如每个抽象产品角色都有两个具体产品。抽象工厂模式提供两个具体工厂角色，分别对应于这两个具体产品角色，每一个具体工厂角色只负责某一个产品角色的实例化。每一个具体工厂类只负责创建抽象产品的某一个具体子类的实例。

[Java Example](https://github.com/fatiaoyezi/design_model/tree/master/src/factory/abstract_factory )

