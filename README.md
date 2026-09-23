# secondhand · 校园二手交易平台

JAVA 实训课程的课程设计项目，基于 Spring Boot。规划了商品、订单、收藏、评论、求购、购物车、站内搜索、公告等业务模块。

> **项目状态：课程骨架（未完成）**
>
> 当前仓库是实训期间搭建的工程骨架——11 个 Controller 已按业务域命名并建立文件结构，但方法体尚未实现。以此记录当时的模块划分设计，不包含可运行的业务逻辑。

## 技术栈

- **Java 21**
- **Spring Boot 3.3.1**（`spring-boot-starter-web`）
- Maven（含 Maven Wrapper，无需预装 Maven）

## 目录结构

```
src/main/java/org/sixhamster/secondhand/
├── SecondhandApplication.java     # 启动类
└── controller/                    # 各业务模块的控制器（骨架）
    ├── GoodsController.java         # 商品信息
    ├── OrderController.java         # 订单
    ├── CollectController.java       # 收藏
    ├── CommentController.java       # 评论
    ├── AsktoBuyController.java      # 求购
    ├── ShoppingCartController.java  # 购物车
    ├── SiteSearchController.java    # 站内搜索
    ├── NoticeController.java        # 公告
    ├── UsersController.java         # 用户
    ├── LoginController.java         # 登录
    └── HelloController.java         # 连通性测试
```

## 如何运行

需要 JDK 21。

```bash
# Windows
mvnw.cmd spring-boot:run

# Linux / macOS
./mvnw spring-boot:run
```

## 分支说明

| 分支 | 内容 |
|---|---|
| `v2`（默认） | 包含全部 11 个 Controller 骨架，业务模块划分最完整 |
| `master` | 最初的空工程，仅启动类与测试类 |

## 后续计划

按规划的业务模块逐个补齐：先做用户与登录，再做商品发布与检索，最后是订单与购物车流程。
