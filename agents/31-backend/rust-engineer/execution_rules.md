# Execution Rules — Rust Engineer

## General Rules
1. MUST use Rust 2024 edition idioms
2. MUST run clippy and fix all warnings
3. MUST handle all Result types (no unwrap in production code)
4. MUST implement proper error types with thiserror/anyhow
5. MUST use serde for serialization

## Safety Rules
1. Minimize unsafe code; document each use
2. Use RAII patterns for resource management
3. Implement proper Send + Sync for shared types
4. Use Arc for shared ownership, not Rc in concurrent code

## Async Rules
1. Use tokio as the async runtime
2. Implement proper cancellation with tokio::select!
3. Use bounded channels for backpressure
4. Avoid blocking the async executor