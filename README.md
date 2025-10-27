# leetcode-rust

用 Rust 刷 LeetCode 的个人项目

## 项目结构

每个题目一个 rs 文件，直接在主函数中写测试用例。

```
src/
├── main.rs              # 入口文件（可选）
├── two_sum.rs          # 题目示例：两数之和
├── problem_xxx.rs      # 你的题目...
└── ...
```

## 运行方式

### 运行主函数测试

```bash
# 运行示例题目
cargo run --bin two_sum

# 或者直接运行某个文件的主函数
rustc --edition 2021 src/two_sum.rs && ./two_sum
```

### 运行单元测试

如果你想运行项目中的单元测试：

```bash
cargo test
```

## 解题规范

每个题目的文件应包含：
1. 题目描述（注释）
2. 解题函数
3. 主函数包含测试用例
4. （可选）单元测试

示例：
```rust
/// LeetCode #X: 题目名称

pub fn solution(/* ... */) {
    // your solution
}

fn main() {
    // 测试用例 1
    println!("测试用例 1:");
    // ...
    
    // 测试用例 2
    println!("测试用例 2:");
    // ...
}
```
