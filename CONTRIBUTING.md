# 贡献指南

欢迎补充 Gemini 4 Carbon 的公开、可核验使用案例。

## 提交要求

1. 必须与 **Gemini 4 Carbon** 直接相关。来源要清楚写明是 Carbon 做的工作。不要把只属于 Gemini 4 Argon，或只在 Arena / 第三方目录里被猜测成 Carbon 的结果送来。
2. 附上原始来源链接（官方博文、公司公告、作者原帖、GitHub 仓库或可核验的新闻，且该新闻应能追溯到一手来源）。
3. 保留作者或机构署名；说明 Carbon 参与了哪一部分（生成、协调、审计、评测等）。
4. 一条 Pull Request 对应一个独立项目、演示或公开结果，不要把能力介绍复述成多条。
5. 时长、成本、基准分数、点赞数等数字请按来源原文抄录，不要改写成「已独立验证」。
6. 网络安全案例只写公开结论。不要提交利用步骤、PoC、payload 或复现流程。
7. 请同步修改：
   - `README.md`（中文默认）
   - `README.en.md`
   - `cases.json`（字段：`id`, `title_zh`, `title_en`, `category`, `summary`, `source_url`, `author`, `date`, `source_type`；可用 `notes` 写收录说明）

## 分类

现有分类：`official-demo`、`cybersecurity`、`science`、`engineering`、`knowledge-work`、`community`。新案例请尽量归入已有类；只有明显对不上时再提议新类。

## 修改方式

事实勘误、失效链接、错误署名和版权问题可以直接开 Issue 或 Pull Request。小修正也可直接提交 PR。
