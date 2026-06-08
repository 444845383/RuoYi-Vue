# RuoYi-Vue-skill 更新任务

## 计划清单

- [x] 核对当前仓库后端框架、模块结构与接口协议
- [x] 核对当前仓库前端框架、目录结构、权限与动态路由机制
- [x] 澄清本次目标是更新 Trae 全局 `RuoYi-Vue-skill`，而非新增仓库业务模块
- [x] 重写全局 skill 文档，使其与当前 `RuoYi-Vue + RuoYi-Vue3` 真实基线一致
- [x] 复核 skill 文档中的路径、权限、路由、接口、技术栈描述是否与项目源码一致
- [x] 执行后端编译与前端构建验证，确认 skill 所依据的框架基线可正常工作
- [x] 补充审查结论与验证结果

## 审查记录

- 已将全局 `RuoYi-Vue-skill` 从“默认 Vue2 / ruoyi-ui 基线”更新为“后端 `RuoYi-Vue` + 前端 `RuoYi-Vue3` 基线”。
- 已补充动态路由、权限指令、`/login`、`/getInfo`、`/getRouters`、`RouterVo`、`RuoYi-Vue3/src/views` 组件路径等底层约束。
- 已执行 `mvn -pl ruoyi-admin -am -DskipTests compile`，结果 `BUILD SUCCESS`。
- 已执行 `RuoYi-Vue3` 目录下 `npm run build:prod`，结果构建成功。
- 当前仓库仍存在用户原有的大量未提交改动：旧 `ruoyi-ui` 删除、`RuoYi-Vue3` 与 `tasks` 为未纳管内容，本次未回滚这些改动。
