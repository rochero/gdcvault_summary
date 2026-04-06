# GDCVault 总结

本仓库包含对 GDCVault 上数千个演讲视频的 AI 总结，方便速览和检索。数据提供 Markdown、CSV 和 SQLite 三种格式。

## 数据来源与处理方式

- **原始视频列表数据**：来自 [https://gdc-search.github.io/](https://gdc-search.github.io/)  
- **原始视频**：来自 [https://gdcvault.com/](https://gdcvault.com/)
- **AI 总结内容**：基于以下资料通过 qwen3.5-flash 批量生成  
  - 视频自带字幕  
  - whisper-large-v3-turbo 转写的字幕  
  - 演讲 PDF 附件里的文本  

## 数据字段说明

每条记录包含以下字段：

| 字段名     | 说明 |
|------------|------|
| year       | 演讲年份 |
| category   | 演讲所属大类 |
| shortcat   | 简化分类标签 |
| title      | 演讲标题 |
| custom_id  | 唯一标识符 |
| vpage      | 视频页面链接 |
| spage      | 幻灯片页面链接 |
| speaker    | 演讲者姓名 |
| company    | 演讲者所在公司 |
| overview   | 官方简介 |
| duration   | 演讲时长（分钟） |
| content    | AI 总结内容 |

## 版权声明

仅用于学习与研究目的。原始视频与幻灯片版权归 GDCVault 及相关演讲者所有。
