Code for my personal website. Built using [Hugo](https://gohugo.io/) and [Papermod](https://github.com/adityatelange/hugo-PaperMod/)

Deployment workflow:
1. Deploy to S3. hugo --> hugo deploy. If this fails check environment variables in ~/.zshenv
2. Check that S3 bucket updated. Once confirmed
3. Go to Cloudfront --> Distributions --> Invalidations and invalidate the cache. Choose `/*` to invalidate all