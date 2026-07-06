# Bug Finder — Limitations

## Detection Limitations
- Cannot detect bugs that require runtime execution without running the code
- False positive rate up to 10% for heuristic-based detections
- May miss domain-specific logic bugs that require deep business knowledge
- Cannot detect race conditions without thread sanitizer data
- Performance limitations on very large codebases (>1M lines)

## Context Limitations
- Limited to provided source code context
- Cannot access production runtime data
- No access to user feedback or bug reports from external sources

## Language-Specific Limitations
- Partial language support may reduce detection accuracy
- Dynamic languages (Python, JS) have higher false positive rates
- Macro-heavy code (C++, Rust, Elixir) may have blind spots
