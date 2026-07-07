# Performance Regression Detector — Examples

## Example 1: Lighthouse Score Drop
**Baseline:** Performance 92, LCP 1.8s, TBT 150ms
**Current:** Performance 68, LCP 4.2s, TBT 450ms
**Analysis:** New analytics script added blocking render
**Root Cause:** `analytics.js` loaded synchronously in `<head>`

## Example 2: API Latency Regression
**Baseline:** p50 45ms, p99 120ms
**Current:** p50 120ms, p99 450ms
**Analysis:** New N+1 query pattern in order listing
**Root Cause:** Missing eager loading for related entities

## Example 3: Bundle Size Increase
**Baseline:** 245KB gzipped
**Current:** 412KB gzipped
**Analysis:** Tree-shaking failure after library update
**Root Cause:** Import style changed from named to default import
