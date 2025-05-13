InfiniLM 是如何做到千亿参数模型高效推理的。

## 技术要点
- 模型蒸馏
- 缓存机制优化
- 异步计算与流水线执行

## 推理加速示例
```javascript
const model = new InfiniLM({
  size: "large",
  cache: true,
  async: true,
});
```

