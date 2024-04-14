# vite-ssr-react
https://deploy-preview-16089--vite-docs-main.netlify.app/guide/

# Vite OSS Repo

```bash
git clone https://github.com/vitejs/vite.git
cd vite
pnpm install
cd packages/vite
pnpm run build
pnpm link --global # globally link the vite package you built
```

# Vite Project Using Vite OSS Repo

- in another window 
```bash
pnpm create vite # choose others react ssr
cd vite-project
pnpm link --global vite # link the app project to your global vite
```
- in the newly created project, add the local vite to dev deps
```json
"devDependencies": {
    "vite": "file:/Users/bronifty/codes/oss/vite"
  }
```
