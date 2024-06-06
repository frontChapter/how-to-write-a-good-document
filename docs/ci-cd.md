## CI/CD

We use GitHub Actions for continuous integration and deployment. The configuration file is located in `.github/workflows/deploy.yml`.

### GitHub Actions Configuration

```yaml
name: Deploy

on:
  push:
    branches:
      - main

jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Install dependencies
        run: npm install
      - name: Build project
        run: npm run build
      - name: Deploy to Vercel
        run: vercel deploy --prod
        env:
          VERCEL_TOKEN: ${{ secrets.VERCEL_TOKEN }}
```

---

[Go back to Readme](../README.md)
