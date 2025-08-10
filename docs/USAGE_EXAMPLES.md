# Usage Examples

This guide shows how consumers should import and use your public APIs. Replace placeholders when APIs are added.

JavaScript / TypeScript
```ts
// Installation (example)
// npm install @your-scope/your-pkg

// Importing a function
import { doThing } from "@your-scope/your-pkg";

async function run() {
  const result = await doThing({ flag: true });
  console.log(result.value);
}

run();
```

React Components
```tsx
import { PrimaryButton } from "@your-scope/your-pkg";

export default function Page() {
  return <PrimaryButton label="Save" onClick={() => console.log("clicked")} />;
}
```

Python
```python
# pip install your-package
from your_package import do_thing

print(do_thing(True))
```

Go
```go
import (
    "github.com/your-org/your-pkg"
)

func main() {
    out, err := yourpkg.DoThing(yourpkg.Options{Flag: true})
    if err != nil { panic(err) }
    println(out.Value)
}
```

Rust
```rust
use your_crate::do_thing;

fn main() {
    let out = do_thing(true).unwrap();
    println!("{}", out.value);
}
```

Notes
- Replace package names with actual module names when available.
- Include error-handling examples where relevant.