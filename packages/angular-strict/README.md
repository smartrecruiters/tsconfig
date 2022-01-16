# tsconfig/strict-angular
Usually it's told that for enabling strict mode for TS just `"strict": true` should be added in `tsconfig.json` of your project. Actually it's not fully truth, there are much many additional options and with this package you don't have to check which options should be enabled for absolutely strict mode. SmartRecruiters’ tsconfig enables all strict rules and keeps your project type-safety.

## Installation

There are just two simple steps for starting using strict mode.

**Step 1**. Install an appropriate version on the package, it's really simple version of the package should be the same as your TS version without patch version

| Package version | Angular version |
|-----------------|:----------------|
| 11.0             | 11.0           |
| 12.0             | 12.0           |
| 13.0             | 13.0           |

```
npm i -D git+https://github.com/smartrecruiters/tsconfig.git
```
When typescript in your project wil be updated don't forget to update the package as well, but anyway if there is more suitable the package version for the new version of TS there will be a warning in your terminal.

**Step 2**. Configure typescript in your project:

Just add `"extends": "@tsconfig/strict-angular/tsconfig.json",` in your main `tsconfig` file. It's also possible to override any rule that the package provides by default, for example
```json
{
  "extends": "@tsconfig/strict-angular/tsconfig.json",
  "compilerOptions": {
    "allowUnusedLabels": false
  }
}
```

## License

[MIT](LICENSE)