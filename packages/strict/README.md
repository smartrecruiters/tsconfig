# tsconfig/strict
Usually it's told that for enabling strict mode for TS just `"strict": true` should be added in `tsconfig.json` of your project. Actually it's not fully truth, there are much many additional options and with this package you don't have to check which options should be enabled for absolutely strict mode. SmartRecruiters’ tsconfig enables all strict rules and keeps your project type-safety.

## Installation

There are just two simple steps for starting using strict mode.

**Step 1**. Install an appropriate version on the package, it's really simple version of the package should be the same as your TS version without patch version

| Package version | TS version |
|-----------------|:-----------|
| 4.0             | 4.0        |
| 4.1             | 4.1        |
| 4.2             | 4.2        |
| 4.3             | 4.3        |
| 4.4             | \>=4.4     |

```
npm i -D git+https://github.com/smartrecruiters/strict-tsconfig.git
```
When typescript in your project wil be updated don't forget to update the package as well, but anyway if there is more suitable the package version for the new version of TS there will be a warning in your terminal.

**Step 2**. Configure typescript in your project:

Just add `"extends": "@tsconfig/strict/tsconfig.json",` in your main `tsconfig` file. It's also possible to override any rule that the package provides by default, for example
```json
{
  "extends": "@tsconfig/strict/tsconfig.json",
  "compilerOptions": {
    "allowUnusedLabels": false
  }
}
```

## License

[MIT](LICENSE)