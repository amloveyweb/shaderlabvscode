## Syntax Highlighting

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/highlighting.jpg)

## Code Completion and Basic Intellisense

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/completion.jpg)

## Hover Information

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/hover.jpg)

## Signature Help

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/signature.jpg)

## Document Symbols

Press `CTRL + SHIFT + o` on Windows or `CMD + SHIFT + o` on macOS.

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/symbol-provider.jpg)

## Go To Definition

`This feature is available in 1.2.4 +`

Press `F12` to trigger `Go To Definition` command Or Click the `Go To Definition` in right click context menu 

![](https://www.amloveycom/shaderlabvscode/assets/Go_To_Definition.gif)

## Code Snippets

Below are the snippets:

| Snippets     | Description                              |
| ------------ | :--------------------------------------- |
| blend1_1     | Blend One One                            |
| blendsa_1-sa | Blend SrcAlpha OneMinusSrcAlpha          |
| blend1_1-sa  | Blend One OneMinusSrcAlpha               |
| blend1-dc_1  | Blend OneMinusDstColor One               |
| blenddc_0    | Blend DstColor Zero                      |
| blenddc_sc   | Blend DstColor SrcColor                  |
| cgp          | CGPROGRAM...ENCG                         |
| for          | for loop                                 |
| fallback     | Fallback                                 |
| glp          | GLSLPROGRAM...ENCGLSL                    |
| if           | if { ... }                               |
| ifelse       | if {...} else {...}                      |
| incucg       | #include "UnityCG.cginc"                 |
| inclight     | #include "Lighting.cginc"                |
| incautolight | #include "AutoLight.cginc"               |
| props        | Properties                               |
| prop2d       | `2D` type property                       |
| propcube     | `Cube` type property                     |
| propc        | `Color` type property                    |
| propv        | `Vector` type property                   |
| propf        | `Float` type property                    |
| proprange    | `Range` type proprety                    |
| region       | //#region ... //#endregion               |
| region2      | //region ... //endregion                 |
| shader       | Shader { ... }                           |
| subshader    | SubShader { ... }                        |
| struct       | structure                                |
| tags         | Tags { ... }                             |
| tagstt       | Tags with both of RenderType and Queue is Transparent |

## Auto Format

### Format Document

Two ways to format document:

1. Right click the editor are and select __Format Document__ menu in context menu  
2. Open __Command Palette__ and type "Format Document", and then press `ENTER` key on keyborad.

## Formatting Options
### Place Open Brace On New Line

In Settings, there is an item under `ShaderlabVScode` section named `Formatting: Style`, check or uncheck the `Place open brace on new line` will toggle differnt format style.

Below is not place open brace on new line

```csharp
float test() {

}
```

Below is place open brace on new line

```csharp
float test()
{
    
}
```

## Misc Features

### 1. Region Mark

There are two ways:

- `//#region` and `//#endregion`
- `//region` and `//#endregion`

## Features in Unity Editor 

### 1.  Download Visual Studio Code

Jump to url which can download latest version of Visual Studio Code

> Selection: __Tools__ -> __ShaderlabVSCode__ -> __Download Visual Studio Code__ 

### 2.  Update Data of ShaderlabVSCode Extension

Update data of completion, hover information or intelisense from web

> Selection: __Tools__ -> __ShaderlabVSCode__ -> __Update Data of VSCode Extension__

### 3. Report an Issue

Two ways to report an issue:

1. Send Email to <amlovey@qq.com>
2. Open a issue on <https://github.com/amloveyweb/amloveyweb.github.io/issues>
