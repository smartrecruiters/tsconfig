# strict-tsconfig
Usually it's told that for enabling strict mode for TS just `"strict": true` should be added in `tsconfig.json` of your project. Actually it's not fully truth, there are much many additional options and with this package you don't have to check which options should be enabled for absolutely strict mode. SmartRecruiters’ tsconfig enables all strict rules and keeps your project type-safety.

## How to use

Choose a needed project:

- [TypeScript](packages/strict/README.md)
- [Angular](packages/angular-strict/README.md)

## How to update

1. create a branch with a proper name or checkout on existing one with the proper name
   - TypeScript: `strict-{major version of TS}.{minor version of TS}.x`
   - Angular: `angular-{major version of Angular}.{minor version of Angular}.x`
2. update `peerDependencies`
3. set proper version for a package. The same version as `TS`/`Angular` apart from patch version. Patch version should be `0` or increased from previous version 
4. push updates
5. create and push a tag with the same name as the branch or update an existing tag 
6. publish the new version on `nmp`
   - TypeScript: `npm run publish:ts`
   - Angular: `npm run publish:angular`

## License

[MIT](LICENSE)
