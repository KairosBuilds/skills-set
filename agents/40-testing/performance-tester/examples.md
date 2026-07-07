# Examples

## k6 Script
```javascript
import http from 'k6/http';
import { check, sleep } from 'k6';

export const options = {
  stages: [
    { duration: '2m', target: 100 },
    { duration: '5m', target: 100 },
    { duration: '2m', target: 0 },
  ],
  thresholds: {
    http_req_duration: ['p(95)<500'],
  },
};

export default function () {
  const res = http.get('https://api.example.com/users');
  check(res, { 'status is 200': (r) => r.status === 200 });
  sleep(1);
}
```

## Artillery YAML
```yaml
config:
  target: 'https://api.example.com'
  phases:
    - duration: 60
      arrivalRate: 10
      rampTo: 50
scenarios:
  - flow:
      - get:
          url: '/users'
```
