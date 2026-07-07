# Quality Checklist — Rust Engineer

- [ ] No unwrap() in production code
- [ ] Clippy warnings resolved
- [ ] Proper error types (thiserror/anyhow)
- [ ] Tests passing (cargo test)
- [ ] Documentation written (cargo doc)
- [ ] No unsafe code without justification
- [ ] Send + Sync implemented for shared types
- [ ] Async cancellation handled