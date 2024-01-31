# Aynı anda iki farklı içeri aktarma (require ve import) sistemi kullanma

Öncelikle bir dosya açıp şunu yazın:

```js
// Örnek amaçlı dosya yolu ./src/utils/require.js olsun

import { createRequire } from "module";
export const require = createRequire(import.meta.url);
```

Başka bir dosyada bu şekilde kullanabilirsiniz.

```js
// Örnek amaçlı dosya yolu ./src/index.js olsun

import { require } from "./utils/require.js";

const Discord = require("discord.js");
```
