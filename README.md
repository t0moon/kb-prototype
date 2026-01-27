# 知识库管理系统原型图

基于 Dify 的企业级知识库管理平台 UI 原型设计。

## 在线预览

🔗 **GitHub Pages**: https://YOUR_USERNAME.github.io/kb-prototype/

## 页面列表

| 页面 | 功能 | 文件 |
|------|------|------|
| 首页 | 导航入口 | [index.html](index.html) |
| 页面1 | 知识库创建 | [create-kb.html](create-kb.html) |
| 页面2 | 文件上传与配置 | [file-upload.html](file-upload.html) |
| 页面4 | 知识图谱与SOP | [knowledge-graph.html](knowledge-graph.html) |
| 页面5 | 知识库检索 | [retrieval.html](retrieval.html) |
| 页面6 | 知识库评估 | [hit-testing.html](hit-testing.html) |
| 页面7 | 用户权限管理 | [user-management.html](user-management.html) |
| 页面8 | API管理 | [api-management.html](api-management.html) |

## 功能特性

### 页面1: 知识库创建
- 支持分领域创建知识库
- 两级业务标签（业务 → 场景）
- 版本管理与回滚

### 页面2: 文件上传
- 多格式文档支持（PDF、Word、Markdown、Excel）
- 专有名词/术语表管理
- Embedding 模型配置
- 向量库配置（Milvus、PGVector、FAISS）
- 向量索引状态监控

### 页面4: 知识图谱
- 图谱可视化
- 节点手动编辑
- SOP 流程管理
- Mermaid 格式导出
- 全量/局部更新模式

### 页面5: 知识库检索
- 语义检索 / 关键词检索 / 混合检索
- TopK 参数配置
- 相似度阈值配置
- 业务标签/场景过滤
- 结构化检索结果返回

### 页面6: 知识库评估
- 单条/批量 Query 命中测试
- 查看命中内容对应的 Chunk 与原始文档
- 命中率 / TopK 命中率统计
- 人工标注与结果对比
- 评测历史回溯

### 页面7: 用户管理
- 管理员 / 编辑 / 只读角色
- 知识库级权限控制
- 文档级数据权限控制

### 页面8: API 管理
- 统一知识库检索 API
- API Key 管理
- 在线调试
- 调用统计

## 技术栈

- 纯 HTML + CSS + JavaScript
- 无需构建，开箱即用
- 响应式布局
- Dark 主题

## 本地运行

```bash
cd kb-prototype
python3 -m http.server 8080
```

然后访问 http://localhost:8080

## License

MIT
