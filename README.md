A simple project to refactor a personal site using new static site concepts like Hugo and modern deployment concepts like Github Actions.

The content is built using Hugo and deployed to S3 using Github actions. The site is hosted using AWS S3 and fronted by Cloudflare.

### Local Testing
Loose notes of local testing and initial build steps

    hugo new site .
    git clone <theme URL> themes/<theme name>
    # git submodule add https://github.com/EmielH/hallo-hugo.git themes/hallo
    hugo server -t <theme name>


### Deployment
Normal deploy to S3 using latest.

    hugo deploy

Force if caching is preventing Hugo from pushing to S3.

    hugo deploy --verbose --force
    

### Useful Reading
https://capgemini.github.io/development/Using-S3-and-Hugo-to-Create-Hosting-Static-Website/
https://www.a-h.io/blog/github-actions-hugo-deploy-and-amazon-s3/
https://github.com/virtualjj/aws-s3-backed-cloudflare-static-website