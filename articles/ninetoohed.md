NineToothed 是一个轻量级 AI 编译器工具链，支持跨平台部署。

## IR 设计
基于 MLIR 构建中间表示，实现语言与硬件解耦。
MLIR 提供了模块化设计，使得 IR 可以灵活扩展。

```rust
fn build_ir() -> Module {
    let module = Module::new();
    module.add_func("main", vec![Arg::new("input", TensorType::F32)];
}