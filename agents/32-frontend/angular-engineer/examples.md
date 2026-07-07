# Angular Engineer Examples

## Example 1: Standalone Component with Signals

```typescript
@Component({
  selector: 'app-counter',
  standalone: true,
  changeDetection: ChangeDetectionStrategy.OnPush,
  template: `<button (click)="increment()">Count: {{ count() }}</button>`
})
export class CounterComponent {
  count = signal(0);
  private logger = inject(LoggerService);
  increment() { this.count.update(c => c + 1); this.logger.log('incremented'); }
}
```

## Example 2: Reactive Form with Validation

```typescript
@Component({ standalone: true, ... })
export class LoginFormComponent {
  form = new FormGroup({
    email: new FormControl('', [Validators.required, Validators.email]),
    password: new FormControl('', [Validators.required, Validators.minLength(8)])
  });
  onSubmit() { if (this.form.valid) /* submit */ }
}
```

## Example 3: Lazy-Loaded Route Configuration

```typescript
export const routes: Routes = [{
  path: 'dashboard',
  loadComponent: () => import('./dashboard/dashboard.component').then(m => m.DashboardComponent),
  canActivate: [authGuard]
}];
```
