# Quality Checklist

## Pre-Check
- [ ] All manifest files available (package.json, Cargo.toml, etc.)
- [ ] Lock file present and up-to-date
- [ ] Package registry accessible
- [ ] Clear version ranges defined (no wildcards)

## During Check
- [ ] Full dependency tree resolved
- [ ] Peer dependencies validated
- [ ] Transitive dependencies checked
- [ ] Breaking changes identified
- [ ] Security vulnerabilities scanned
- [ ] Platform requirements verified

## Post-Check
- [ ] Report generated and stored
- [ ] Critical issues escalated
- [ ] Recommendations documented
- [ ] Check results published to release pipeline
- [ ] Known false positives documented
