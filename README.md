# nuxt-scss-sample
開發環境為 https 
## 設置

```bash
# 安裝
$ yarn install

# localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

### 製作本機 https 憑證

1. 安裝 Homebrew
2. 安裝 [mkcert](https://github.com/FiloSottile/mkcert)
```bash
brew install mkcert
mkcert -install
# 切換到要放憑證的檔案目錄，製作憑證
mkcert localhost 
```
3. 新增 `.env`
```bash
HTTPS_KEY=../localhost-key.pem
HTTPS_CERT=../localhost.pem
```
## 目錄

assets 目錄包含未編譯的資產，例如 Stylus 或 Sass 文件、圖像或字體。
[documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

components 包含你的 Vue.js 組件。組件構成頁面的不同部分，可以重複使用並導入到頁面、佈局甚至其他組件中。
[documentation](https://nuxtjs.org/docs/2.x/directory-structure/components)

layouts 當您想要更改 Nuxt 應用程序的外觀和感覺時，無論您想要包含側邊欄還是為移動設備和桌面提供不同的佈局
[documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts)

pages 此目錄包含您的應用程序視圖和路由。 Nuxt 將讀取此目錄中的所有 `*.vue` 文件並自動設置 Vue Router。
[documentation](https://nuxtjs.org/docs/2.x/get-started/routing)

plugins 包含您希望在實例化根 Vue.js 應用程序之前運行的 JavaScript 插件。 這是添加 Vue 插件和注入函數或常量的地方。 每次需要使用 `Vue.use()` 時，都應該在 `plugins/` 中創建一個文件，並將其路徑添加到 `nuxt.config.js` 中的插件中。
[documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins)

static 此目錄包含您的靜態文件。 此目錄中的每個文件都映射到`/`。
Example: `/static/robots.txt` is mapped as `/robots.txt`.
[documentation](https://nuxtjs.org/docs/2.x/directory-structure/static)

store 此目錄包含您的 Vuex 存儲文件
[documentation](https://nuxtjs.org/docs/2.x/directory-structure/store)
