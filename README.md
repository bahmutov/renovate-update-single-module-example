# renovate-update-single-module-example [![renovate-app badge][renovate-badge]][renovate-app] [![ci status][ci image]][ci url]
[ci image]: https://github.com/bahmutov/renovate-update-single-module-example/workflows/test/badge.svg?branch=master
[ci url]: https://github.com/bahmutov/renovate-update-single-module-example/actions
> Example repository where only a single dependency is updated using Renovate Bot

The [renovate.json](renovate.json) only allows checking updates for dependency `debug`, all other dependencies (like `chalk`) should be ignored. Here is the relevant portion of the file, we disable all updates, except for package `debug` using [excludePackagePatterns](https://docs.renovatebot.com/configuration-options/#excludepackagepatterns) option:

```json
"packageRules": [
  {
    "packagePatterns": ["*"],
    "excludePackagePatterns": ["debug"],
    "enabled": false
  }
]
```

Renovate Bot documentation at [https://docs.renovatebot.com/](https://docs.renovatebot.com/)

You can see what Renovate does using the [Renovate Dashboard](https://app.renovatebot.com/dashboard).

![Renovate Dashboard](images/dashboard.png)

Click on any build, and in the DEBUG logs you can search for a module and see if it was disabled.

![Disabled chalk module](images/disabled.png)

## More info

- [Zeit Now GitHub app + Renovate app + Cypress tests = 💝](https://glebbahmutov.com/blog/zeit-now-renovate-and-app/)
- [Painless Dependency Upgrades with Renovate App](https://glebbahmutov.com/blog/renovate-app/)

[renovate-badge]: https://img.shields.io/badge/renovate-app-blue.svg
[renovate-app]: https://renovateapp.com/
