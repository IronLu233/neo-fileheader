# Fileheader Pro

Fileheader VSCode extension with out-of-box and full customizable

## Features

### Full customizable. Write your own template **with javascript logic**

![CustomFileheader](https://user-images.githubusercontent.com/20639676/175778910-6d761e2e-e956-48d6-90ef-fe9193d481cd.gif)

### Auto add file header when create new file. **No need to add file header manually**

![AutoInsert](https://user-images.githubusercontent.com/20639676/175778891-90796099-26e7-42a7-b501-77b5d6b03b50.gif)

### Auto update file header when save file

![AutoUpdate](https://user-images.githubusercontent.com/20639676/175778916-0a2734d2-21a3-4e93-833c-377261912652.gif)

## Usage

### Manually add file header

Open your file and press Ctrl+Shift+P(`Command+Shift+P` on Mac).

Then type `"Fileheader Pro: Add Fileheader"`
a default file header will insert into your file.

### Customize fileheader with template

Press Ctrl+Shift+P(`Command+Shift+P` on Mac) for open your command palette.

Then type `"Fileheader Pro: Generate Custom Fileheader Template"`
A new [template file](https://github.com/IronLu233/fileheader-pro/blob/main/src/FileheaderLanguageProviders/provider.template.js) will be generated in your `${workspaceRoot}/.vscode/fileheader.template.js`

## Extension Settings

| Setting                              | Default Value         | Description                                                        |
| ------------------------------------ | --------------------- | ------------------------------------------------------------------ |
| FileheaderPro.currentUserName        |                       | The fixed current user. The default is from your VCS               |
| FileheaderPro.currentUserEmail       |                       | The fixed current user email. The default is from your VCS         |
| FileheaderPro.companyName            | YourCompanyName       | Company name, please replace to your owns                          |
| FileheaderPro.dateFormat             | 'YYYY-MM-DD HH:mm:ss' | The date format, see https://momentjs.com/docs/#/displaying/format |
| FileheaderPro.autoInsertOnCreateFile | true                  | Auto insert file header when create new file                       |
| FileheaderPro.autoUpdateOnSave       | true                  | Auto update file header when save file                             |

## Known Issues

Due to API limit, modify the source code and then manually edit to original in VCS will change the modified time.

`mtime` of template variable may have some issues.
If you find any issue, please report to [GitHub Issue](https://github.com/IronLu233/fileheader-pro/issues)

## TODOS
- [ ] Add support for other languages
- [ ] Add support for other VCS
- [ ] Integration test and unit test

## Release Notes

### 0.0.1
