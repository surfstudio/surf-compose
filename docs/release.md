# Release

Each component has its own release github action, which deploys a new artifact version to [SurfArtifactory](https://artifactory.surfstudio.ru/artifactory/webapp/#/artifacts/browse/tree/General/libs-release-local/ru/surfstudio/compose).

Release is launched manually from GithubActions list, [example](https://github.com/surfstudio/surf-accompanist/actions/workflows/release.yml).

A new version must be provided as input parameter for release job. A current lib version could be found at gradle.properties. By default a new lib version increments the previous (major, minor or patch version part, which could be defined by developer for each case).

A new version will be comitted to gradle.properties after successfull release.

![manual-release](https://github.com/surfstudio/surf-compose/blob/main/docs/data/manual-run.png?raw=true)
