# OpenMAIC 课堂存档

由 [OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) 生成的 AI 互动课堂数据存档。

## 课堂列表

### 01 · AI 与 Agent 全解析
- **课堂 ID**: `T-0DmI0CRD`
- **在线地址**: https://open.maic.chat/classroom/T-0DmI0CRD
- **数据文件**: [T-0DmI0CRD.json](./T-0DmI0CRD.json)
- **场景数**: 12
- **简介**: 面向零技术背景用户，讲解 AI 与 Agent 的本质区别、主流模型、各职业应用场景及上手路径。

**场景目录**
1. 课程导入
2. 什么是AI：从"复读机"到"创作家"
3. AI 基础认知小测验
4. 什么是 AI Agent：给 AI 装上"身体"
5. Agent 工作原理全拆解
6. 主流 Agent 框架与产品大赏
7. 提效实战 1：电商运营与传统行业
8. 提效实战 2：教育从业者与自由职业者
9. 场景应用实战测试
10. 普通人上手 Agent 的最简路径
11. 警惕！AI 和 Agent 的局限性
12. 总结：拥抱智能时代，成为"指挥官"

---

### 02 · 桃花源记 · 时空调查
- **课堂 ID**: `YAynHhhM2S`
- **在线地址**: https://open.maic.chat/classroom/YAynHhhM2S
- **数据文件**: [YAynHhhM2S.json](./YAynHhhM2S.json)
- **场景数**: 15
- **原始课件**: https://lydia2214.github.io/slides/taoyuanji/v1/
- **简介**: 初中语文《桃花源记》游戏化教学，采用"时空调查"框架，8个任务扩展为15个场景。

**场景目录**
1. 任务导入：时空调查启动
2. 解锁线索：4张线索卡
3. 通读全文
4. 调查记录：环境/生活/路径/叹惋
5. 读文测验
6. 古今异义：6个陷阱词
7. 一词多义：志·寻
8. 社会档案：小组分析
9. 最大谜题：4条证据链
10. 存在之辩：投票辩论
11. 揭秘：陶渊明的精神世界
12. 虚实相生的写法
13. 调查报告：总结
14. 结项综合测验
15. 延伸：你的桃花源

---

## 数据格式说明

每个 `.json` 文件包含完整的课堂结构：

```json
{
  "id": "课堂ID",
  "stage": { "name": "课堂名称", "language": "zh-CN", ... },
  "scenes": [ { "type": "slide|quiz|interactive|pbl", "title": "...", "content": {...} } ],
  "createdAt": "生成时间"
}
```

可通过 OpenMAIC API 重新导入：
```bash
curl -X POST https://open.maic.chat/api/classroom \
  -H "Content-Type: application/json" \
  -d @T-0DmI0CRD.json
```

## 生成工具

- 平台：[OpenMAIC](https://open.maic.chat) · 清华大学开源
- 生成时间：2026-03-23
