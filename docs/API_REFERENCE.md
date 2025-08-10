# API Reference

This document lists all publicly exposed APIs, functions, classes, and components.

Current inventory
- No public APIs detected in the repository yet.

How to add new API entries
- Prefer documenting directly alongside code using language-native doc comments. See examples below.
- Each public item should include: purpose, parameters, return values, possible errors, and at least one runnable example.

Templates by language

JavaScript / TypeScript
```ts
/**
 * Concise one-line summary.
 *
 * Longer description with context and behavior.
 *
 * @example
 * import { doThing } from "@your-scope/your-pkg";
 * const result = await doThing({ flag: true });
 * console.log(result.value);
 *
 * @param options - Description of options
 * @returns Useful result description
 * @throws ErrorType when ...
 */
export async function doThing(options: { flag: boolean }): Promise<{ value: number }> {
  // ...
}
```

React component (TSX)
```tsx
/** Button that triggers an action. */
export function PrimaryButton(props: { label: string; onClick: () => void }) {
  return <button onClick={props.onClick}>{props.label}</button>;
}

/**
 * @example
 * <PrimaryButton label="Save" onClick={() => save()} />
 */
```

Python
```python
def do_thing(flag: bool) -> int:
    """Concise one-line summary.

    Longer description with context and behavior.

    Args:
        flag: Description
    Returns:
        int: Useful result description
    Raises:
        ValueError: when ...

    Examples:
        >>> do_thing(True)
        42
    """
    pass
```

Go
```go
// DoThing performs the operation.
//
// Example:
//  out, err := DoThing(Options{Flag: true})
//  if err != nil { log.Fatal(err) }
//  fmt.Println(out.Value)
func DoThing(opts Options) (Result, error) {
    // ...
}
```

Rust
```rust
/// Performs the operation.
///
/// # Examples
/// ```
/// let out = crate::do_thing(true);
/// assert!(out.value > 0);
/// ```
pub fn do_thing(flag: bool) -> Result<i32, Error> {
    // ...
}
```

Documentation checklist per item
- Name and short summary
- Detailed description and assumptions
- Parameters and types
- Return type and shape
- Errors and edge cases
- Examples (happy-path and failure)
- Version introduced / breaking changes