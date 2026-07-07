# Accessibility Engineer Examples

## Example 1: Accessible Modal Dialog

```tsx
<div role="dialog" aria-modal="true" aria-labelledby="modal-title">
  <h2 id="modal-title">Confirm Delete</h2>
  <p>Are you sure you want to delete this item?</p>
  <button onClick={closeModal}>Cancel</button>
  <button onClick={confirmDelete}>Delete</button>
</div>
```

## Example 2: Accessible Form with Error Association

```tsx
<div>
  <label htmlFor="email">Email</label>
  <input id="email" type="email" aria-describedby="email-error" aria-invalid={!!error} />
  {error && <p id="email-error" role="alert">{error}</p>}
</div>
```

## Example 3: Skip Navigation Link

```tsx
<a href="#main-content" className="sr-only focus:not-sr-only focus:absolute focus:p-4">
  Skip to main content
</a>
<main id="main-content">{children}</main>
```
