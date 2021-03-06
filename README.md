# vuerd-vscode

> [vuerd](https://github.com/vuerd/vuerd) ERD Editor vscode extension

[![npm version](https://img.shields.io/npm/v/vuerd.svg?style=flat-square&color=blue)](https://www.npmjs.com/package/vuerd) [![VS Marketplace version](https://vsmarketplacebadge.apphb.com/version-short/dineug.vuerd-vscode.svg?style=flat-square&color=blue&logo=visual-studio-code)](https://marketplace.visualstudio.com/items?itemName=dineug.vuerd-vscode) [![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square&logo=webcomponents.org)](https://www.webcomponents.org/element/vuerd) [![GitHub](https://img.shields.io/github/license/vuerd/vuerd?style=flat-square&color=blue)](https://github.com/vuerd/vuerd/blob/master/LICENSE) [![Codecov](https://img.shields.io/codecov/c/gh/vuerd/vuerd?logo=codecov&style=flat-square)](https://codecov.io/gh/vuerd/vuerd) [![CI](https://img.shields.io/github/workflow/status/vuerd/vuerd/CI?label=CI&logo=github&style=flat-square)](https://github.com/vuerd/vuerd/actions)

## ERD

![vuerd](https://github.com/vuerd/vuerd/blob/master/img/vuerd-erd.gif?raw=true)

## SQL DDL

![vuerd](https://github.com/vuerd/vuerd/blob/master/img/vuerd-ddl.gif?raw=true)

## Generator Code

![vuerd](https://github.com/vuerd/vuerd/blob/master/img/vuerd-generator-code.gif?raw=true)

## Visualization

![vuerd](https://github.com/vuerd/vuerd/blob/master/img/vuerd-visualization.gif?raw=true)

## SQL DDL Import

![vuerd](https://github.com/vuerd/vuerd/blob/master/img/vuerd-ddl-import.gif?raw=true)

## Usage

### [Webview API](https://code.visualstudio.com/api/extension-guides/webview)

1. ERD data [filename].vuerd.json Save a file as a form
1. Focus on the saved file and click the vuerd icon in the upper right corner of the Editor window  
   ![Image](./img/vuerd-vscode-2.png)  
   ![Image](./img/vuerd-vscode-1.png)

### [Custom Editor API](https://code.visualstudio.com/api/extension-guides/custom-editors)

1. ERD data [filename].vuerd Save a file as a form

## Theme

### settings.json

```json
{
  "dineug.vuerd-vscode.theme": {
    "canvas": "#282828",
    "table": "#191919",
    "tableActive": "#14496d",
    "focus": "#00a9ff",
    "keyPK": "#B4B400",
    "keyFK": "#dda8b1",
    "keyPFK": "#60b9c4",
    "font": "#a2a2a2",
    "fontActive": "white",
    "fontPlaceholder": "#6D6D6D",
    "contextmenu": "#191919",
    "contextmenuActive": "#383d41",
    "edit": "#ffc107",
    "columnSelect": "#232a2f",
    "columnActive": "#372908",
    "minimapShadow": "black",
    "scrollBarThumb": "#6D6D6D",
    "scrollBarThumbActive": "#a2a2a2",
    "menubar": "black",
    "visualization": "#191919"
  }
}
```

## Document

- [Live Demo](https://vuerd.github.io/vuerd/iframe.html?id=editor--load)
- [Import SQL DDL support syntax](https://github.com/vuerd/vuerd/blob/master/data/SQL_DDL_Test_Case.md)

## Editor Keymap(default)

| Name                                                       | Keymap                                                                   |
| ---------------------------------------------------------- | ------------------------------------------------------------------------ |
| Editing - ERD                                              | dblclick, Enter                                                          |
| Editing - Grid                                             | dblclick, Enter                                                          |
| All Stop                                                   | Escape                                                                   |
| Search - find, filter                                      | Ctrl + Alt + F                                                           |
| Undo - ERD                                                 | Ctrl + Z                                                                 |
| Redo - ERD                                                 | Ctrl + Shift + Z                                                         |
| Selection - table, memo                                    | Ctrl + Drag, Click, Ctrl + Click, Ctrl + Alt + A                         |
| Selection - column, filter                                 | Click, Ctrl + Click, Shift + Click, Shift + Arrow key(up, down), Alt + A |
| Movement - table, memo, column, filter                     | Drag, Ctrl + Drag                                                        |
| Copy - column                                              | Ctrl + C                                                                 |
| Paste - column                                             | Ctrl + V                                                                 |
| Contextmenu - ERD, Table, Relationship, SQL, GeneratorCode | Right-click                                                              |
| Table Properties                                           | Ctrl + Space                                                             |
| New Table                                                  | Alt + N                                                                  |
| New Memo                                                   | Alt + M                                                                  |
| New - column, filter                                       | Alt + Enter                                                              |
| Delete - table, memo                                       | Ctrl + Delete                                                            |
| Delete - column, filter                                    | Alt + Delete                                                             |
| Select Hint - dataType, find                               | Arrow key(right), Click                                                  |
| Move Hint - dataType, find                                 | Arrow key(up, down)                                                      |
| Primary Key                                                | Alt + K                                                                  |
| checkbox - Grid, filter                                    | Space, Click                                                             |
| Move checkbox - Grid, filter                               | Arrow key(up, down, left, right)                                         |
| Relationship - Zero One N                                  | Ctrl + Alt + 1                                                           |
| Relationship - Zero One                                    | Ctrl + Alt + 2                                                           |
| Relationship - Zero N                                      | Ctrl + Alt + 3                                                           |
| Relationship - One Only                                    | Ctrl + Alt + 4                                                           |
| Relationship - One N                                       | Ctrl + Alt + 5                                                           |
| Relationship - One                                         | Ctrl + Alt + 6                                                           |
| Relationship - N                                           | Ctrl + Alt + 7                                                           |

## TODO

- [x] Undo, Redo Manager
- [x] Grid filter
- [x] ERD Table finder
- [x] Real-time simultaneous editing api
- [x] SQL index Support [#9](https://github.com/vuerd/vuerd-vscode/issues/9)
- SQL DDL import Support [#7](https://github.com/vuerd/vuerd-vscode/issues/7)
  - [x] Oracle
  - [x] MSSQL
  - [x] PostgreSQL
- [ ] SQL-Query generator [#3](https://github.com/vuerd/vuerd/issues/3)

## License

[MIT](https://github.com/vuerd/vuerd-vscode/blob/master/LICENSE)
