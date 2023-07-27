# Metabase Buildpack

Forked from https://github.com/metabase/metabase-buildpack as metabase does not officially support the Heroku buildback.

Add the following to your app.json:

```
"buildpacks": [
  {
    "url": "https://github.com/kaizan-ai/metabase-buildpack"
  }
]
```

The metabase version is statically set in the `bin/version` file. To bump the version, update this file.

## Pushing to staging

Staging currently has the buildpack manually added in the Heroku UI (see screenshot)

![image](https://github.com/kaizan-ai/metabase-buildpack/assets/12790/70a6d0a9-ea85-4bd8-8c13-17f4be899fe4)

We shouldn't need to do this, but I'm not changing it now.

Pushing to staging should be a case of running the commands under **QuickStart** in the https://github.com/kaizan-ai/metabase-deploy repository.

## Pushing to prod
Just use the Heroku UI to **Promote to Production**.
