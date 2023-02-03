# strict-tsconfig
Usually it's told that for enabling strict mode for TS just `"strict": true` should be added in `tsconfig.json` of your project. Actually it's not fully truth, there are much many additional options and with this package you don't have to check which options should be enabled for absolutely strict mode. SmartRecruiters’ tsconfig enables all strict rules and keeps your project type-safety.

## How to use

Choose a needed project:

- [TypeScript](packages/strict/README.md)
- [Angular](packages/angular-strict/README.md)

## Contribution

### Updating major/minor versions
1. update `peerDependencies`
1. add new verson in the readme
1. make other necesary changes
1. set proper version for a package. The same version as `TS`/`Angular` apart from patch version. Patch version should be `0`
1. create PR
1. after getting aprouval you can merge it
1. all tags will be created automatically

### Patching
1. make necesary change
1. create PR
1. after getting aprouval you can merge it
1. patch version will be bumped automatically
1. all tags will be created automatically

## License

[MIT](LICENSE)
