# renovate-update-single-module-example [![renovate-app badge][renovate-badge]][renovate-app] [![ci status][ci image]][ci url]
[ci image]: https://github.com/bahmutov/renovate-update-single-module-example/workflows/test/badge.svg?branch=master
[ci url]: https://github.com/bahmutov/renovate-update-single-module-example/actions
> Example repository where only a single dependency is updated using Renovate Bot

The [renovate.json](renovate.json) only allows checking updates for dependency `debug`, all other dependencies (like `chalk`) should be ignored. The configuration follows advice given in [this issue](https://github.com/renovatebot/config-help/issues/210)

[Renovate Dashboard](https://app.renovatebot.com/dashboard)

[renovate-badge]: https://img.shields.io/badge/renovate-app-blue.svg
[renovate-app]: https://renovateapp.com/
