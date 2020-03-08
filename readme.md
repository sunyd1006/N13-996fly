# 区块链共享员工管理系统（EMS）
github 地址: https://github.com/sunyd1006/N13-996fly

demo视频下载地址（github不支持在线观看）：https://github.com/sunyd1006/N13-996fly/blob/master/demo_ppt/demo.mp4

demo视频在线观看地址（b站等待审核通过中）：
- 地址1：http://114.55.144.141:6789/file.mp4
- B站地址2：审核成功后更改
	
移动前端 Demo地址： http://123.56.86.151:8085/


## 区块链共享员工管理系统是什么？

	  区块链员工共享系统是一套摆脱中心化机构进行员工信息管理与验证的分布式系统解决方案，
	整个系统是基于开源联盟链框架Fisco Bcos设计而成。它与传统的信息系统最大的区别在于，
	其摆脱了多对点对多的拓扑网络结构，变成了点对点对点的星状网络结构，任意业务参与方只
	需要在其服务器集群内部署好一套集成的区块链共享员工管理服务，即可通过P2P网络与其它
	业务参与方构建一个共享员工管理系统。任一事务写入该系统都不会受到任意中心化系统的控
	制，各业务参与方会各自验证事务的合法性，并按照既定的可形式化验证的智能合约代码执行
	该请求，并通过BFT算法对该事务达成共识，维护分布式系统的强一致性。简单来说，这样的
	系统将实现业务闭环内的去信任化，而对于业务参与方而言，区块链共享员工管理系统其实就
	像一个开箱即用的盒子，他们只需要将其打开，并结合自己原有的核心系统配置好，就可以直
	接使用这套服务了。

## 我们希望解决什么问题？
	  疫情期间，许多企业无法正常开工，大多数人都待在家里，人们对O2O以及电商、物流行业
	的需求变得非常旺盛，不同领域的企业对于员工数量的需求开始产生了不平衡现象。因此，一
	种共享员工的模式开始流行了起来。事实上，这个共享员工并不是什么新鲜事了，企业间对于
	员工的劳务派遣早在很久以前就有了。人力资源与社会保障局也迅速对这种模式给予了认可，
	并提示了相关的法律风险。而相应的企业共享平台也开始出现，但出现的这些平台都只服务于
	帮助企业更快的匹配意向共享企业，而并没有为企业之间提供如何解决员工派遣流程数字化问
	题的SaaS服务。而在员工的派遣过程中，其实是会有许多需要多方交叉验证的流程的。比方说
	员工的五险一金应当如何缴纳，员工在派遣过程中的企业福利可否享受，员工的工资应当如何
	发放等等问题。一趟派遣流程，可能需要员工在新老公司与政府部门之间来回跑几趟才能保证
	手续齐全。这显然是与疫情期间的“尽量少出门”的宗旨相违背。因此，一个需要多方参与的信
	息化系统就成了一个刚性需求，我们希望通过区块链共享员工管理系统，可以帮助员工在不需
	要出一趟门的情况下把所有派遣手续办完，并通过引入官方机构参与，以保证流程中不会存在
	任何的法律风险，保障员工和企业在派遣期间的一切合法权益。

## 我们是如何设计这个系统的？
我们希望整个系统就像是一个开奖即用的盒子，那么让我们一起来看看盒子里有什么吧？
### 运行框架
![Image text](.//photo/operation.png)
### 系统架构
![Image text](.//photo/photo1.png)
### DID设计准则
![Image text](.//photo/DID.png)
### 模块介绍
#### Weidentity
	  WeIdentity是一套分布式多中心的技术解决方案，可承载实体对象（人或者物）的现实身份与
	链上身份的可信映射、以及实现实体对象之间安全的访问授权与数据交换。WeIdentity由微众银
	行自主研发并完全开源，秉承公众联盟链整合资源、交换价值、服务公众的理念，致力于成为链接
	多个垂直行业领域的分布式商业基础设施，促进泛行业、跨机构、跨地域间的身份认证和数据合作。
	其目前主要包含两大模块：WeIdentity DID以及WeIdentity Credential。

#### BaaS服务
	  通过这个BaaS服务可视化的管理自己的节点和用户交易，并可以查阅共识状态和区块详情，甚至
	可以通过BaaS服务编译、更新和部署新的智能合约，完成应用层的横向扩展。那么逻辑上其实BaaS
	服务就是基于核心接入层接口的SDK开发的可视化区块链运维工具，方便机构可以轻松上手运维。

#### 企业协作管理服务
      企业协作管理服务，这也是我们系统的核心服务，主要分为数据层和管理层，数据层主要是进行
    外部数据的审核、处理和上链，以及链上信息的聚合与可视化。管理层主要是维护好员工其链上DID
    身份与本地关系型数据库的一个关联性，并对员工的状态，线上合同的签订以及系统设定进行管理。

#### Demo流程展示

github 地址: https://github.com/sunyd1006/N13-996fly

demo视频下载地址（github不支持在线观看）：https://github.com/sunyd1006/N13-996fly/blob/master/demo_ppt/demo.mp4

demo视频在线观看地址（b站等待审核通过中）：
- 地址1：http://114.55.144.141:6789/file.mp4
- B站地址2：审核成功后更改
	
移动前端 Demo地址： http://123.56.86.151:8085/

![Image text](.//photo/demo.png)
