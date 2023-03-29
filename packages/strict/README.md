# @smartrecruiters/tsconfig-strict

Usually it's told that for enabling strict mode for TS just `"strict": true` should be added in `tsconfig.json` of your project. Actually it's not fully truth, there are much many additional options and with this package you don't have to check which options should be enabled for absolutely strict mode. Our tsconfig enables all strict rules and keeps your project type-safety.

For Angular projects, please, use [config for Angular](https://www.npmjs.com/package/@smartrecruiters/tsconfig-strict-angular)

## Installation

There are just two simple steps for starting using strict mode.

**Step 1**. Install an appropriate version of the package, it's really simple - the version of the package should be the same as your TS version without patch version

| Package version | TS version |
| --------------- | :--------- |
| 5.0.x           | 5.0.x      |
| 4.9.x           | 4.9.x      |
| 4.8.x           | 4.8.x      |
| 4.7.x           | 4.7.x      |
| 4.6.x           | 4.6.x      |
| 4.5.x           | 4.5.x      |
| 4.4.x           | 4.4.x      |
| 4.3.x           | 4.3.x      |
| 4.2.x           | 4.2.x      |
| 4.1.x           | 4.1.x      |
| 4.0.x           | 4.0.x      |


```
npm i -D @smartrecruiters/tsconfig-strict@{version}
```

When TypeScript in your project wil be updated don't forget to update the package as well. But anyway, if the current version of the package is not perfectly matches for the new version of TS, there will be a warning in your terminal.

**Step 2**. Configure typescript in your project:

Just add `"extends": "@smartrecruiters/tsconfig-strict/tsconfig.json",` in your main `tsconfig` file. It's also possible to override any rule that the package provides by default, for example

```json
{
  "extends": "@smartrecruiters/tsconfig-strict/tsconfig.json",
  "compilerOptions": {
    "allowUnusedLabels": false
  }
}
```

## License

[MIT](LICENSE)
