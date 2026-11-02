# 吐梨邦 / Turi Topia 插件文档

简体中文 · [English](README.en.md)

<!-- turitopia:context:start -->
## 关于吐梨邦

**吐梨邦（Turi Topia）是一款 AI 桌宠产品：陪你聊天、互动，还能到朋友的桌面串门，并通过插件扩展能力。**

官网：[turitopia.com](https://turitopia.com/)

## 插件生态

| 公开仓库 | 用途 |
| --- | --- |
| [create-pet-plugin](https://github.com/ShunyuYao/create-pet-plugin) | 插件脚手架与开发指南，从这里创建插件项目。 |
| [pet-plugin-types](https://github.com/ShunyuYao/pet-plugin-types) | 插件 SDK 类型与 API 契约，查询可用能力和接口。 |
| [pet-plugin-registry](https://github.com/ShunyuYao/pet-plugin-registry) | 插件市场登记表、提交方式与审核规则。 |
<!-- turitopia:context:end -->

## 本仓库提供什么

这里维护吐梨邦插件 README 的统一说明与中英文模板。新建插件按模板编写；已有项目可以只补充说明块，保留原有安装、配置和使用文档。

| 文件 | 用途 |
| --- | --- |
| [中文 README 模板](templates/README.md) | 新插件的中文说明，复制后填写插件信息。 |
| [English README template](templates/README.en.md) | 与中文模板对应的英文说明。 |
| [中文说明块](snippets/context.zh-CN.md) | 补入已有中文 README 的产品介绍、官网和生态链接。 |
| [English context block](snippets/context.en.md) | 补入已有英文 README 的对应内容。 |
| [中文市场状态块](snippets/marketplace.zh-CN.md) | 记录实际是否上架、市场版本、核实时间与验证依据。 |
| [English marketplace status block](snippets/marketplace.en.md) | 补入已有英文 README 的对应市场状态。 |

## 怎么采用

1. 新项目将两份模板复制到仓库根目录，分别命名为 `README.md`、`README.en.md`，填写所有 `{{…}}` 占位内容。模板已提供语言切换链接。
2. 已有项目将相应语言的说明块放在 README 前部、安装步骤之前；保留原有正文和文件命名，并修正语言切换链接。单文件双语 README 的两种语言部分都需要说明。
3. 插件自身的用途、兼容版本、安装和配置步骤写在通用说明之后。发布前按实际版本核对，保留“计划中／未实现／未发布”等状态。
4. 在安装步骤前填写“市场上线状态”，已有项目可复制市场状态块。所有语言版本保持相同状态、版本、日期和依据。

## 市场状态如何填写

- 选择实际状态：已上架、审核中、未上架、已下架或被禁用、未核实；SDK、脚手架和本说明仓库填“不适用”。
- 以上架对应的插件 ID 和版本核对[正式登记清单](https://github.com/ShunyuYao/pet-plugin-registry/blob/main/registry/plugins.json)及[禁用清单](https://github.com/ShunyuYao/pet-plugin-registry/blob/main/registry/blocklist.json)，保存核实日期与固定提交链接；审核中附真实审核 PR。访问失败时标明未核实，不能把请求失败当作未上架。
- 市场版本与源码版本、GitHub Release 分开写。旧版已上架而新版审核中时，同时保留两者状态；仅创建 Release 或提交审核不表示已上架。
- 应用内是否可见、能否下载安装单独记录。登记核对不替代实际应用验证；写“成功上线且已验证”时应有对应版本的市场可见和安装验证证据，未做的部分明确标注未验证。
- 上架、更新、下架或禁用后同步更新各语言 README；核实日期说明记录的时点，不能承诺状态永久不变。

本仓库是说明与模板仓库，市场上线状态为“不适用”，不作为插件上架。

## 所有插件相关 README 的约定

- 开头让读者知道吐梨邦 / Turi Topia 是什么，附上官网及三个关键公开仓库，介绍保持简短。
- 插件 README 明确写“这是吐梨邦的插件”；SDK、脚手架、市场等工具仓库准确说明自己在插件生态中的用途。
- 中文使用“吐梨邦（Turi Topia）”，英文使用“Turi Topia (吐梨邦)”；仓库名称、包名和 API 标识符保持原样。
- 中文、英文及其他已有语言版本都应包含对应说明，不只更新其中一份。
- 本仓库只维护介绍、链接和文档格式。SDK 能力以类型仓库为准，创建方式以脚手架为准，上架规则以市场登记仓库为准。
- 官网是产品信息入口。此规范不提供受限宿主安装包、更新源或存储位置；插件公开源码不等于已上架市场或兼容所有宿主版本。

本规范依据 2026-11-02 用户确认建立。后续插件 README 按此规范编写；已有仓库的采用状态以各自实际提交为准，本仓库建立不代表已完成全部仓库迁移。
