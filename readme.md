@wymjs/vite-build-drop-log
===

> 構建模式移除 console

## 安裝

```shell
$ pnpm i -D @wymjs/vite-build-drop-log
```

## 使用

```typescript
import { defineConfig } from 'vite'
import { buildDropLog } from '@wymjs/vite-build-drop-log'

export default () => {
  return defineConfig({
    plugins: [
      // 配置下去就會在 vite build 時移除項目中的 console 與 debugger
      // 恩...就這樣
      buildDropLog(),
    ],
  })
}
```
