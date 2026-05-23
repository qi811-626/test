# Anthropic Office Skills

本仓库仅复制 Anthropic 官方 skills 仓库中的办公四件套：

- `skills/docx`
- `skills/xlsx`
- `skills/pptx`
- `skills/pdf`

安装来源：

- 官方仓库：https://github.com/anthropics/skills/tree/main/skills
- 复制范围：`skills/docx`、`skills/xlsx`、`skills/pptx`、`skills/pdf`
- 复制日期：2026-05-23

## 用途

| Skill | 用途 |
| --- | --- |
| `docx` | 创建、读取、编辑和分析 Word `.docx` 文件，包括模板、批注、修订、目录、页眉页脚和格式化文档。 |
| `xlsx` | 创建、读取、编辑和分析电子表格，包括 `.xlsx`、`.xlsm`、`.csv`、`.tsv`，支持公式、格式、图表和数据清理。 |
| `pptx` | 创建、读取、编辑和检查 PowerPoint `.pptx` 演示文稿，包括模板、幻灯片、备注和视觉 QA。 |
| `pdf` | 读取、拆分、合并、旋转、加水印、创建、OCR、填写表单和处理 PDF 文件。 |

## 文件完整性

每个 skill 目录都保留了官方仓库中的原始文件，包括 `SKILL.md`、脚本、模板、参考文档、资源和许可证文件。已确认以下文件存在：

- `skills/docx/SKILL.md`
- `skills/xlsx/SKILL.md`
- `skills/pptx/SKILL.md`
- `skills/pdf/SKILL.md`

## 依赖要求

以下依赖根据各 skill 的 `SKILL.md`、参考文档和脚本整理。具体任务只需要安装对应场景所需的依赖。

| Skill | 依赖 |
| --- | --- |
| `docx` | `pandoc` 用于文本提取；Node 包 `docx` 用于新建 Word 文档；LibreOffice / `soffice` 用于转换和接受修订；Poppler 的 `pdftoppm` 用于渲染页面图片。 |
| `xlsx` | LibreOffice / `soffice` 用于公式重算；Python 包 `pandas` 用于数据分析；Python 包 `openpyxl` 用于公式、格式和工作簿编辑。 |
| `pptx` | Python 包 `markitdown[pptx]` 用于文本提取；Python 包 `Pillow` 用于缩略图；Node 包 `pptxgenjs` 用于从零创建演示文稿；LibreOffice / `soffice` 用于转 PDF；Poppler 的 `pdftoppm` 用于渲染幻灯片图片；`pptxgenjs.md` 中还提到可选的 `react-icons`、`react`、`react-dom`、`sharp`。 |
| `pdf` | Python 包 `pypdf`、`pdfplumber`、`reportlab` 用于常见 PDF 操作；可选 Python 包 `pypdfium2`、`pdf2image`、`pytesseract` 用于高级渲染和 OCR；JavaScript 包 `pdf-lib` 用于表单和高级 PDF 修改；命令行工具 Poppler (`pdftotext`、`pdftoppm`、`pdfimages`)、`qpdf`，以及可选的 `pdftk`。 |
