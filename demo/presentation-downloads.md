# 静态原型单证样例

六个 `presentation-*` 文件为固定演示资产。页面直接下载文件，不在浏览器调用业务生成器。

- `presentation-jlr-china.xls`、`presentation-jlr-ningbo.xls`：2026-10-21 一次性使用仓库 `customer-invoice-template.js` 的已有模板输出，保留对应原 17 列和三张工作表，文件为真正的 Excel 97–2003 格式。
- `presentation-invoice-en.xlsx`、`presentation-invoice-zh.xlsx`、`presentation-packing.xlsx`、`presentation-guarantee.xlsx`：同日一次性使用仓库 `self-made-document-templates.js` 和 `self-made-document-layouts.json` 输出，保留既有四类原件版式、合并区域、打印设置及模板固定文字。

全部业务数据为预设合成样例，单据范围固定为 `DEMO-BL-20261001` 下 `SALKA9BW1NA100001` 和 `SALKA9BW1NA100002` 两辆车。客户、供应商、地址、联系人等均采用“示例／DEMO”内容，无签章、原件图片或私有业务主体数据。文件仅用于原型展示，不作为业务凭证。

专项验证 `tests/presentation-special.test.mjs` 检查实际文件格式、17 列及四类单据主体布局。生成器与业务引擎不属于默认展示入口的依赖。
