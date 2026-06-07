# tavern-helper-ui

SillyTavern 角色卡的前端界面托管仓库（通过 jsdelivr CDN 提供）。

仅包含已编译的前端产物，源码在本地 `tavern_helper_template` 项目中维护。

## 状态栏

- `xiayou/index.html` — 夏柚 角色卡的状态栏界面（Vue3 + MVU，运行于酒馆助手 iframe 内）

jsdelivr 访问地址：
```
https://testingcf.jsdelivr.net/gh/BLBKS/tavern-helper-ui/xiayou/index.html
```

## 更新方式

1. 在 `tavern_helper_template`（本地 `制卡/`）中修改 `src/夏柚/界面/状态栏/` 源码
2. `pnpm build`
3. 把 `dist/夏柚/界面/状态栏/index.html` 复制到本仓库 `xiayou/index.html`
4. `git commit` + `git push`
5. 如 CDN 未刷新，访问 `https://purge.jsdelivr.net/gh/BLBKS/tavern-helper-ui/xiayou/index.html` 刷新缓存
