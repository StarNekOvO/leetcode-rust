# LeetCode Rust

用 Rust 刷 LeetCode 的个人项目

## 项目结构

每个题目放在 `examples/` 目录下，可以独立运行。

```
examples/
├── p0001_two_sum.rs    # 题目 1：两数之和
├── p0002_add_two_numbers.rs  # 题目 2
└── ...
```

## 使用方法

### 运行题目

根据你把测试用例写在哪，选择不同的命令：

```bash
# 如果测试用例写在 main() 函数里 → 用 run
cargo run --example p0001_two_sum

# 如果测试用例写在 #[test] 标记的函数里 → 用 test
cargo test --example p0001_two_sum
```

**区别：**
- `cargo run` → 执行 `main()` 函数里的手动调试代码
- `cargo test` → 执行所有 `#[test]` 标记的自动化测试

### 添加新题目

1. 在 `examples/` 目录创建新文件 `p0XXX_xxx.rs`
2. 复制模板，按格式填写题目描述
3. 实现解题函数和测试用例
4. 可直接运行 `cargo run --example p0XXX_xxx`

## 解题模板

```rust
/// # 题目编号. 题目名称
/// 
/// 题目描述...
///
/// ## 示例 1：
/// ```
/// 输入：...
/// 输出：...
/// ```

// 实现函数
pub fn solution(/* 参数 */) {
    // TODO: 你的实现
}

#[cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn test_case_1() {
        // TODO: 测试用例 1
    }
}

fn main() {
    // TODO: 测试用例
    println!("结果: ");
}
```
