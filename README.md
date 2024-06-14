# LiteMES（免费开源小型生产制造系统）

当前最新版本：v1.5.0 (发布时间：2024-06-14)



[![输入图片说明](https://img.shields.io/static/v1?label=licents&message=Apache%20License%202.0&color=green)](https://gitee.com/leepm/mini-contract/blob/master/LICENSE)

[![输入图片说明](https://img.shields.io/static/v1?label=Author&message=shawn&color=blue)](https://www.yi-types.com)

[![输入图片说明](https://img.shields.io/static/v1?label=version&message=1.5.0&color=green)](https://www.yi-types.com)



## LiteMES 什么是 ？



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-13T16%3A18%3A26-zrnt.png)


LiteMES，一款专为广大中小型企业量身打造的生产制造全链路执行系统，以其卓越的性价比和低投入成本，成为市场上备受青睐的选择。系统基于行业标准开源项目开发，融合了企业现实业务需求，旨在提供一套全面、高效且易于使用的生产管理工具，同时我们也支持物联网设备的接入，如监控摄像、火灾报警等



LiteMES 的六大核心功能模块——计划排程、仓储管理、制造执行、质量管理、物联网IoT管理、看板报表管理——均经过精心设计，以实现功能最大化与操作简化的完美平衡。这些模块的协同工作，不仅优化了生产流程，还大幅提升了企业的运营效率和产品质量。



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-13T16%3A21%3A20-aqpe.png)


## 我们的优势是什么？



对于资源有限的小型企业而言，LiteMES 的**低成本投入和高性价比**是其最大的福利。系统采用模块化设计，企业可以根据自身需求和预算灵活选择所需的模块，避免了不必要的功能堆砌和成本浪费。此外，LiteMES 的轻量化设计减少了系统对硬件的高要求，进一步降低了企业的IT投资成本。



在易用性方面，LiteMES 提供了直观的图形用户界面和简化的操作流程，即使是技术背景较弱的员工也能迅速掌握使用方法。系统的快速部署和便捷维护，让企业能够以最小的IT支持需求，实现生产管理的数字化转型。



## 适用业务场景

#### 行业 

- 电子行业
- 食品加工行业
- 其它中小微型生产与制造行业企业

#### 功能

- 无纸化生产过程控制

  - 无纸化制程执行，流程跟踪
  - 数据收集\分析，对SMT、手工
  - 插件、微组装加工过程监控管理

  

- 全程质量追溯与分析

  - 基于产品的全生产周期的追溯
  - 分析，监控并及时发现缺陷，提高产品质量；



- 设备状态监控与数据采集
  - 底层工业控制网络实现设备联网和状态监控、数据采集；



- 数字化看板与分析
  - 报表、报警、实时看板以及运作看板。



## 支持业务端

- MES 后台管理端（业务管理）
- MES 生产端（报工）
- MES 移动端（巡检、出入库、库存盘点、售后服务）



## 技术架构

### 开发架构

- 语言：Java 8+ (小于17)，Vue2.0
- IDE(JAVA)： IDEA (必须安装lombok插件 )
- IDE(前端)： Vscode、HBuilder
- 依赖管理：Maven（后端）、npm（前端）
- 缓存：Redis
- 数据库脚本：MySQL

###   **后端**

- 基础框架：Spring Boot

- 持久层框架：Mybatis

- 安全框架：Apache Shiro 1.10.0，Jwt 3.11.0
- 其他：fastjson，poi，Swagger-ui，quartz, lombok（简化代码）等。

```
项目结构

├─ ktg-admim            系统管理模块
├─ ktg-common           公共模块
├─ kgt-flowable         工作流模块
├─ ktg-framework        框架核心模块
├─ ktg-generator        代码生成模块
├─ ktg-mes              系统核心模块
├─ ktg-quartz           定时任务模块
```


### 前端

#### 前端框架

| 说明       | 框架       | 说明     | 框架 |
| ---------- | ---------- | -------- | ---- |
| 基础框架   | element-ui | JS版本   | ES6  |
| 基础JS框架 | Vue.js     | 状态管理 | Vuex |
| css预处理  | scss       |          |      |

```
│  .editorconfig                    // 代码格式配置
│  .env.development	                // 本地环境配置
│  .env.production                  // 生产环境配置
│  .env.test                        // 测试环境配置
│  .eslintignore	                  // ESlint忽略文件配置
│  .eslintrc.js			                // ESlint 检查配置
│  .gitignore			                  // git忽略文件配置
│  package.json	                    // 配置项目版本依赖等信息
│  README.md		                    // 帮助文档
│  vue.config.js	                  // 开发设置
├─build		                          // 打包配置
├─public	                          // html基础配置
└─src						                    // 组件区域
  ├─api						                  // 接口封装
  │
  ├─assetsn						              // 静态资源
  │
  ├─components					            // 公共组件
  │
  ├─config				                  // 配置
  │
  ├─directive					              // 自定义指令
  │
  ├─layout					                // 基础主题组件
  │
  ├─plugins						              // 基础方法及缓存
  │
  ├─router						              // 路由配置
  │
  ├─store    					              // vuex 管理store
  │
  ├─styles							            // 公共样式
  │
  ├─utils						                // 工具
  │
  └─views							              // 页面组件
```


## 项目效果

## MES 后台管理端（业务管理）

> 支持多租户的方式使用，标准的SaaS模式，高性价比，免维护。


![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A25%3A56-tsya.png)


### 组织管理

#### 部门管理

> 标准化的组织架构，让职责划分更加明确，管理职责更加清晰



![2024-06-01T21:28:08-urir.png](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A28%3A08-urir.png)



#### 角色管理

> 功能权限与业务职责可由管理人员随便定义和定制，让管理管理更方便



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A33%3A54-xojn.png)

#### 用户管理

> 企业内部可以管理自己的员工和员工的基本信息，包括权限职责的授权等



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A35%3A10-kyrh.png)

### 工厂管理

#### 编码规则

> 为了满足不同业务场景的需求，我们专门设计了一套由用户和使用人员定制的编号生成规则



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A36%3A20-fmea.png)

#### 物料产品管理

产品、物料、原料、包装、辅料可由使用者自己上传，同时可以设置成品半成品库房，包括上传产品照片和设置产品的过期时间等

![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A43%3A27-lyrf.png)





![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A47%3A00-lqlv.png)



#### 物料产品分类

> 管理人员可以结合自身业务需求情况设置，成品，半成品等分类


![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A48%3A14-jpjt.png)


#### 计量单位

> 同时我们还支持多单位的转换与，主单位，辅单位，主单位与辅单位自动计算等



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A54%3A44-occf.png)


#### 客户管理

![2024-06-01T21:56:01-niil.png](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T21%3A56%3A01-niil.png)


#### 供应商管理



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T22%3A03%3A54-ypqn.png)



#### 车间管理



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T22%3A04%3A33-ocnn.png)



#### 工作站管理



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T22%3A05%3A13-omls.png)


### 生产管理

#### 生产计划管理



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-01T22%3A05%3A53-qvrj.png)


#### 工序设置



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A42%3A32-epki.png)


#### 工艺流程



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A43%3A05-vcnc.png)


#### 生产排产



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A43%3A44-akjo.png)


#### 生产报工



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A45%3A26-rxeo.png)


### 质量管理

#### 常见缺陷



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A46%3A22-nniy.png)



#### 检测项管理



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A53%3A28-whku.png)



#### 检测模板



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A53%3A59-rboo.png)



#### 来料检测



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A54%3A28-dqqk.png)



#### 过程检验



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A54%3A55-hvmn.png)



#### 出货检验



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A55%3A26-kqlg.png)



### 考勤管理

#### 考勤记录



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A56%3A04-ioww.png)



#### 工作日历



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A56%3A29-mzmf.png)



#### 打卡地址

![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A56%3A57-nvbo.png)



####  考情统计

![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-02T17%3A57%3A23-yzby.png)





## MES 生产端（报工）

### 工作台

> 登录之后，生产人员根据自己所在的工序或者环节，选择相应的操作台。



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-13T16%3A36%3A20-ziip.png)



### 生产任务

> 生产人员可通过工作台查看到所有的待生产或者未生产的工作任务，生产人员可对生产情况进行数据的上报



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-13T16%3A39%3A02-ydjp.png)



### 生产报工

> 生产人员可在生产终端上面做相应的任务上报，上报后生产经理能及时在数据看板上面查看到相应的数据信息，使其能实时的掌握生产进度。



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-13T16%3A40%3A45-fmiq.png)



### 切换工作台

> 生产终端支持一个岗位完成多个环节的工作上报，从而使其更加的灵活方便



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-13T16%3A44%3A09-jepv.png)





## MES 移动端(巡检、出入库、库存盘点、售后服务)

### 售后工单

> 用户可以使用小程序返回产品问题，进行产品售后申请，同时也可以实时查看到产品目前的售后流程情况



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-14T14%3A52%3A31-zlrh.png)



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-14T14%3A56%3A29-mrid.png)



### 产品信息

> 用户还可以通过产品二维码进行产品信息的查询，可查看到产品的生产日期、产品过程、产品质量过程，同时还能查询产品的质保情况



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-14T14%3A55%3A16-yjoc.png)



### 产品出入库

> 管理端用户可以通过移动端方便的对产品进行入库、出库、领料等等操作。



![img](https://leepm.oss-cn-beijing.aliyuncs.com/leepm_images/halo/2024-06-14T14%3A56%3A36-eamg.png)





综上所述，LiteMES不仅以其高效的生产管理功能助力企业提升竞争力，更以其高性价比和低投入成本，成为小型企业实现智能制造梦想的理想选择。通过LiteMES，小型企业能够以最小的成本，享受到先进的生产管理技术，实现生产过程的优化和业务增长。



如果你有任何对 LiteMES 产品上的想法、意见或建议，或商务上的合作需求，请扫码添加 LiteMES 项目团队进一步沟通： 

![输入图片说明](https://leepm.oss-cn-beijing.aliyuncs.com/public-images/shawn_huangxing_qrcode.png)

##  给个鼓励

如果觉得还不错，请 Watching，Starred，Fork 吧 ☺
