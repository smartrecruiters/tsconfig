# strict-tsconfig
It is said that to enable strict mode for TypeScript, only `"strict": true` should be added in your project's `tsconfig.json` file. Actually it is not the full truth, there are many more useful additional options and this package enables all of them for an absolute strict mode. SmartRecruiters’ tsconfig contains all strict rules and improves your project type-safety.

## How to use

Choose Readme for your project:

- [TypeScript](packages/strict/README.md)
- [Angular](packages/angular-strict/README.md)

## Guide for Migration
[strict TypeScript: guide](https://docs.google.com/document/d/1mHXk3GMv54rUilGApKXQblyJGMZ9MGNvYUlK3YvuNsw/edit?usp=sharing)

## Contribution

### Updating major/minor versions
1. Update `peerDependencies`.
1. Add new version to the readme.
1. Make other necessary changes.
1. Set proper version for a package. The same version as `TS`/`Angular` apart from patch version. Patch version should be `0`
1. Create PR
1. After the PR is approved, feel free to merge it.
1. All tags will be created automatically.

### Patching
1. Make necessary change.
1. Create PR
1. After the PR is approved, feel free to merge it.
1. Patch version will be bumped automatically.
1. All tags will be created automatically

## License

[MIT](LICENSE)
