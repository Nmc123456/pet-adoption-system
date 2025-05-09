# 🐾 宠物领养系统

[![GitHub license](https://github.com/Nmc123456/pet-adoption-system/blob/main/a1.png)

欢迎使用 **宠物领养系统**，这是一个开源项目，旨在为宠物爱好者提供便捷的领养体验，并为管理员提供高效的管理工具。项目基于现代技术栈开发，支持用户端和管理端功能，仅仅适用于个人学习或实际部署。

- **仓库地址**: [https://github.com/Nmc123456/pet-adoption-system](https://github.com/Nmc123456/pet-adoption-system)
---

## 🚀 功能特性

### 用户端
- **宠物信息浏览**  
  - 查看宠物详细信息，包括品种、年龄、健康状态等。  
  - 支持筛选和搜索功能（例如按品种或年龄排序）。    
    ![宠物列表页](https://github.com/Nmc123456/pet-adoption-system/blob/main/a1.png)

- **在线领养申请**  
  - 提供带表单验证的领养申请页面。  
  - 提交后通过邮件通知管理员和申请者。  
    ![领养申请表单](https://github.com/Nmc123456/pet-adoption-system/blob/main/a2.png)

- **领养进度追踪**  
  - 使用状态机可视化显示领养进度（例如“待审核”→“审核通过”→“领养完成”）。    
    ![领养进度追踪](https://github.com/Nmc123456/pet-adoption-system/blob/main/b1.png)

- **用户端功能模块图**
  - 用户权限操作的功能包括申请领养宠物，申请认领宠物，查看申请的宠物领养或申请的宠物认领的审核状态，发布感谢信，查看或对教学视频进行收藏以及留言。
  - ![用户端功能模块图](https://github.com/Nmc123456/pet-adoption-system/blob/main/d2.png)


### 管理端
- **宠物信息 CRUD 管理**  
  - 支持新增、编辑、删除和查看宠物信息。  
  - 提供批量操作功能（例如批量删除）。  
    ![宠物管理界面](https://github.com/Nmc123456/pet-adoption-system/blob/main/b2.png)

- **领养申请审核工作流**  
  - 管理员可查看申请列表，审核通过或拒绝。  
  - 支持备注和通知功能。   
    ![申请审核](https://github.com/Nmc123456/pet-adoption-system/blob/main/b3.png)

- **数据看板**  
  - 展示领养率统计、热门宠物种类等可视化数据。  
  - 使用图表（如柱状图或饼图）呈现。  
    ![数据看板](https://github.com/Nmc123456/pet-adoption-system/blob/main/c1.png)

 - **管理端功能模块图**
  - 管理员权限操作的功能包括对注册用户信息的管理，对宠物领养，宠物认领，教学视频，感谢信以及公告进行管理，审核宠物领养以及认领的信息。
  - ![管理端功能模块图](https://github.com/Nmc123456/pet-adoption-system/blob/main/d1.png)


---

## 🛠️ 技术架构

```mermaid
graph TD
    A[前端] -->|Vue 3| B(宠物展示模块)
    A -->|Element Plus| C(领养申请表单)
    A -->|Sass| D(样式管理)
    E[后端] -->|Spring Boot 2.2.2| F(JWT 认证 & Shiro)
    E -->|MyBatis-Plus| G(数据持久化)
    H[数据库] -->|MySQL 8.0| I(关系模型设计)
    J[构建工具] -->|Maven| K(后端依赖管理)
    J -->|npm| L(前端依赖管理)
    M[部署] -->|Tomcat 9.0.29| N(嵌入式服务器)
