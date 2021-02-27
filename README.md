A simple project to refactor a personal static site using new concepts like Hugo and Github Actions.

Site is hosted using AWS S3 and front ended by Cloudflare.

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
    