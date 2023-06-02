# Deploy Vite app to GitHub Pages using GitHub Actions + custom domain

This is just an example setup with a custom domain for my other repo:
https://github.com/sitek94/vite-deploy-demo

## Steps

### CNAME record
Add CNAME record in your DNS settings (in my case it's Netlify):

![Screenshot 2023-06-02 at 19 33 18](https://github.com/sitek94/vite-deploy-demo-custom-domain/assets/58401630/0e9a1a2d-d178-4606-8b15-4259c315abea)

### Vite config
Update Vite config:

```diff
export default defineConfig({
  plugins: [react()],
-  base: '/vite-deploy-demo/',
+  base: '/'
})
```

### GitHub Pages
Update Pages settings in repository settings:

![image](https://github.com/sitek94/vite-deploy-demo-custom-domain/assets/58401630/7818c13e-b257-4286-b74b-b74326ca136d)
