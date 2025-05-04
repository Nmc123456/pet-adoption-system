# 🐾 宠物领养系统

[![GitHub license](https://img.shields.io/github/license/Nmc123456/pet-adoption-system)](https://github.com/Nmc123456/pet-adoption-system/blob/main/LICENSE)
[![Java CI](https://github.com/Nmc123456/pet-adoption-system/actions/workflows/build.yml/badge.svg)](https://github.com/Nmc123456/pet-adoption-system/actions)

## 🚀 功能特性
### 用户端
- 宠物信息浏览（品种/年龄/健康状态）
- 在线领养申请（表单验证+邮件通知）
- 领养进度追踪（状态机可视化）

### 管理端
- 宠物信息 CRUD 管理
- 领养申请审核工作流
- 数据看板（领养率统计）

## 🛠️ 技术架构
```mermaid
graph TD
    A[前端] -->|Vue3| B(宠物展示模块)
    A -->|Element Plus| C(领养申请表单)
    D[后端] -->|Spring Boot| E(JWT认证)
    D -->|MyBatis| F(数据持久化)
    G[数据库] -->|MySQL 8.0| H(关系模型设计)
