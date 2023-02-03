# @smartrecruiters/tsconfig-strict-angular

Usually it's told that for enabling strict mode for TS just `"strict": true` should be added in `tsconfig.json` of your project. Actually it's not fully truth, there are much many additional options and with this package you don't have to check which options should be enabled for absolutely strict mode. Our tsconfig enables all strict rules and keeps your project type-safety.

For typescript projects, please, use [config for TypeScript](https://www.npmjs.com/package/@smartrecruiters/tsconfig-strict)

## Installation

There are just two simple steps for starting using strict mode.

**Step 1**. Install an appropriate version on the package, it's really simple - the version of the package should be the same as your Angular version without patch version

| Package version | Angular version |
| --------------- | :-------------- |
| 15.1.x          | >= 15.1.x       |
| 15.0.x          | 15.0.x          |
| 14.2.x          | 14.2.x          |
| 14.1.x          | 14.1.x          |
| 14.0.x          | 14.0.x          |
| 13.3.x          | 13.3.x          |
| 13.2.x          | 13.2.x          |
| 13.1.x          | 13.1.x          |
| 13.0.x          | 13.0.x          |
| 12.2.x          | 12.2.x          |
| 12.1.x          | 12.1.x          |
| 12.0.x          | 12.0.x          |
| 11.2.x          | 11.2.x          |
| 11.1.x          | 11.1.x          |
| 11.0.x          | 11.0.x          |
| 10.2.x          | 10.2.x          |
| 10.1.x          | 10.1.x          |


```
npm i -D @smartrecruiters/tsconfig-strict-angular@{version}
```

When Angular in your project wil be updated don't forget to update the package as well. But anyway, if the current version of the package is not perfectly matches for the new version, there will be a warning in your terminal.

**Step 2**. Configure typescript in your project:

Just add `"extends": "@smartrecruiters/tsconfig-strict-angular/tsconfig.json",` in your main `tsconfig` file. It's also possible to override any rule that the package provides by default, for example

```json
{
  "extends": "@smartrecruiters/tsconfig-strict-angular/tsconfig.json",
  "compilerOptions": {
    "allowUnusedLabels": false
  }
}
```

## License

[MIT](LICENSE)
