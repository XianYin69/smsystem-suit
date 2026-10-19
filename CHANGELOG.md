# CHANGELOG

## [2026-10-19]
### Changed
- 切换正式版分支：伞仓 smsystem-suit 保持在 main 并推送远程 main。
- 撤销误入库的运行产物（db.sqlite3 / runtime/ / task_detail|error|output|result.txt），改由 `.gitignore` 排除；提交 102d52e（承接 192c98c）。
- 改动范围：仓库分支与 .gitignore，未触碰 skill 本体逻辑。
- 涉及文件：.gitignore
- 违反后果：SMS 运行时数据入库 → 泄露本机任务/链数据，且违反红线「SMS 运行时数据不进 skill 本体目录」。

## 规范
- 每次修改/新增/删除操作完成后，必须在本文件记录变更（日期、改动范围、涉及文件、违反后果）；不可缺失、不可跳过、不可事后补录（漏记视为违规）。
