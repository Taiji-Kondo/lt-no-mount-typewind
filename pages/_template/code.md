---
layout: center
---

```ts {1|2|4,5|all}
const a = 1
const b = 2

// 3
console.log(a + b)
```

[//]: # (TODO: Setup Monaco)
```tsx {monaco}
import { FC } from 'react'

type TemplatePropsType = {
  subtitle: string
  title: string
}

const Template: FC<TemplatePropsType> = ({ subtitle, title }) => {
    return (
        <div>
          <h1>{title}</h1>
          <p>{subtitle}</p>
        </div>
    )
}
```