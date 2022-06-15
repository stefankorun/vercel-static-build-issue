## Description

This repo replicates a Vercel issue when trying to serve a static site (e.g. Storybook static site) as a separate Vercel project, 
using the same repository as an existing Next.js project, _only when using custom `vercel.json` configuration_.

### ✅ Next.js Project - builds successfully with default Next cofig:

<img width="480" alt="image" src="https://user-images.githubusercontent.com/2415410/173811259-2e4aca1a-6276-46ca-9153-c10411e037ed.png">

### ❌ Static hosting Project - build fails with error:

<img width="480" alt="image" src="https://user-images.githubusercontent.com/2415410/173810311-a629fbb1-0d65-4df5-a845-0461bcc5bf3a.png">

**Build error**
```
Error: The pattern "pages/api/**/*" defined in `functions` doesn't match any Serverless Functions inside the `api` directory. Learn More: https://vercel.link/unmatched-function-pattern
```

