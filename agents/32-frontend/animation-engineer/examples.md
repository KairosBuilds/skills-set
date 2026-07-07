# Animation Engineer Examples

## Example 1: Framer Motion Spring Entrance

```tsx
<motion.div
  initial={{ opacity: 0, y: 16 }}
  animate={{ opacity: 1, y: 0 }}
  transition={{ type: 'spring', stiffness: 300, damping: 25 }}
/>
```

## Example 2: Staggered List

```tsx
const container = { hidden: {}, visible: { transition: { staggerChildren: 0.06 } } };
const item = { hidden: { opacity: 0, y: 12 }, visible: { opacity: 1, y: 0 } };

<motion.ul variants={container} initial="hidden" animate="visible">
  {items.map(i => <motion.li key={i.id} variants={item}>{i.name}</motion.li>)}
</motion.ul>
```

## Example 3: R3F Animated Sphere

```tsx
function AnimatedSphere() {
  const ref = useRef<Mesh>(null);
  useFrame((state) => { ref.current!.rotation.x = state.clock.elapsedTime * 0.5; });
  return <mesh ref={ref}><sphereGeometry /><meshStandardMaterial color="hotpink" /></mesh>;
}
```
