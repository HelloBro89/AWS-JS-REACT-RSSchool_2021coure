# Online Store

## This repository contains only a frontend part for an online store built on AWS. This app is in the process of being finalized, so some features have not yet been implemented.

### All actual requests for the backend part are located in the file along the relative path:
```bash
cd src\constants\apiPaths.ts
```

## User guide

1. **npm install**
2. **npm run start** 
3. **npm run build** 
4. **npm run build:deploy** - build and deploy in S3 bucket
5. **npm run cloudfront:update:build:deploy** - build, deploy, creat cloudfront and invalidation (with confirm)


