# strict-tsconfig
SmartRecruiters’ tsconfig with all strict rules that helps you don't think anymore about which rules should be enabled or disabled and keep your project stable.  

## Installation

There are just two simple steps.

**Step 1**. Install an appropriate version on the package, it's really simple version of the package should be the same as your TS version without patch version

| TS version | Package version |
|------------|:----------------|
| 4.0        | 4.0             |
| 4.1        | 4.1             |
| 4.2        | 4.2             |
| 4.3        | 4.3             |
| 4.4        | 4.4             |
| 4.5        | 4.5             |

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