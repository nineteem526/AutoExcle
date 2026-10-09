# Excel 出货计划自动化

> **当前项目归档更新至 V21（2026-10-09）。** V21 指用户持有的专用 `.xlsm` 工作簿功能版本，并不表示仓库早期 VBA 源码已同步为 V21。

本仓库中的文档记录 Excel VBA 出货计划工作簿的业务流程、使用方法、验证边界和维护交接。实际工作簿由授权持有人单独保管；文档归档不是发布生产工作簿或 VBA 源码。

## V21 阅读入口

- [V21 项目状态、业务规则、功能、验证和维护边界](docs/V21_PROJECT_STATUS.md)
- [V21 简易操作手册（Markdown）](docs/V21_QUICK_GUIDE.md)
- [V21 简易操作手册（Word）](docs/V21_User_Guide.docx)

V21 的日常收尾顺序：**完成安装日期和 Planned 调整后，最后执行“按批次排序并生成小计”，核查结果，再保存 `.xlsm`。** 普通“刷新总表”不重建明细小计。详细行为和注意事项见 V21 归档与简易手册。

## 历史文档与源码

- [V13 完整项目流程（历史记录）](docs/PROJECT_REPORT.md)
- [早期项目状态（历史记录）](docs/CURRENT_STATUS.md)
- [早期安装说明](docs/INSTALLATION.md)
- [早期验证记录](docs/VALIDATION.md)
- `src/ShippingTools.bas`、`src/SummarySheetEvent.txt`：早期脱敏源码参考。

**重要：** `docs/PROJECT_REPORT.md`、`docs/CURRENT_STATUS.md`、`docs/INSTALLATION.md`、`docs/VALIDATION.md` 和 `src/` 保留了较早阶段的说明。早期源码不能用来重建、完整实现或验证当前 V21 工作簿。请以专用工作簿及 V21 文档为当前行为依据。

## 安全与适用范围

这是依赖固定表结构的项目专用 Excel VBA 工作簿，不是任意 Excel 通用插件。已记录的 V21 文档更新不修改工作簿、不发布 V21 完整宏源码，也不代表仓库历史文件已进行完整安全认证。

该工作簿含业务数据和内部快照。隐藏不等于加密或脱敏。任何外发、共享或源码归档均须遵循项目授权和组织的数据保护要求。运行 VBA 应遵守组织的 Office 宏安全策略；不要为运行按钮降低系统安全设置。

适用环境以 Windows 桌面版 Excel 为目标。WPS、Mac、浏览器版 Excel 和其他版本未承诺完整兼容。
