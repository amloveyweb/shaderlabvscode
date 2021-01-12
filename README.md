# ShaderlabVSCode 

## Introduction
ShaderlabVSCode is a Visual Studio Code extension for Unity Shaderlab progamming.

 <a href='http://forum.unity3d.com/threads/403471/'>Forum </a> | <a href='mailto:amlovey@qq.com'> Email </a> |<a href='https://assetstore.unity.com/packages/slug/94653?aid=1011lGoJ'> Purchase from Asset Store </a> | <a href='https://mianbaoduo.com/product/show/mbd-Yp2Ylw==>'> Purchase from MianBaoDuo </a>

## Video Preview
<iframe width="640" height="351" src="https://www.youtube.com/embed/d9ZNNEcZOOs" frameborder="0" allowfullscreen></iframe>

## Installation

### Running On Mac

1. Import ShaderlabVSCode unity package into Unity Editor.
2. [Download Visual Studio Code](https://go.microsoft.com/fwlink/?LinkID=534106) for macOS.
3. Double-click on the downloaded archive to expand the contents.
4. Drag `Visual Studio Code.app` to the `Applications` folder, making it available in the Launchpad.
5. Launch VS Code, Open the `Command Palette (⇧⌘P) ` and type 'install from vsix' and then press `Enter` key on keyboard.
6. Select the vsix file under `ShaderlabVSCode/VSCodePlugin/` folder of Unity Project
7. Restart Visual Studio Code


### Running On Windows

1. Import ShaderlabVSCode unity package into Unity Editor.
2. Download the [Visual Studio Code installer](https://go.microsoft.com/fwlink/?LinkID=534107) for Windows. 
3. Once it is downloaded, run the installer (VSCodeSetup-version.exe). This will only take a minute.
4. By default, VS Code is installed under C:\Program Files (x86)\Microsoft VS Code for a 64-bit machine.
5. Launch VS Code, Open the `Command Palette (CTRL+SHIF+P) ` and type 'install from vsix' and then press `Enter` key on keyboard.
6. Select the vsix file under `ShaderlabVSCode/VSCodePlugin/` folder of Unity Project
7. Restart Visual Studio Code

> Note: .NET Framework 4.5.2 is required for VS Code. If you are using Windows 7, please make sure .NET Framework 4.5.2 is installed.

## Features

### Syntax Highlighting

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/highlighting.jpg)

### Code Completion and Basic Intellisense

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/completion.jpg)

### Hover Information

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/hover.jpg)

### Signature Help

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/signature.jpg)

### Document Symbols

Press `CTRL + SHIFT + o` on Windows or `CMD + SHIFT + o` on macOS.

![](https://raw.githubusercontent.com/amloveyweb/amloveyweb.github.io/master/assets/images/shaderlabvscode/symbol-provider.jpg)

### Code Snippets

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

### Auto Format

#### Format Document

Two ways to format document:

1. Right click the editor are and select __Format Document__ menu in context menu  
2. Open __Command Palette__ and type "Format Document", and then press `ENTER` key on keyborad.

### Formatting Options
#### Place Open Brace On New Line

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

### Misc Features

#### 1. Region Mark

There are two ways:

- `//#region` and `//#endregion`
- `//region` and `//#endregion`

### Features in Unity Editor 

####1.  Download Visual Studio Code

Jump to url which can download latest version of Visual Studio Code

> Selection: __Tools__ -> __ShaderlabVSCode__ -> __Download Visual Studio Code__ 

####2.  Update Data of ShaderlabVSCode Extension

Update data of completion, hover information or intelisense from web

> Selection: __Tools__ -> __ShaderlabVSCode__ -> __Update Data of VSCode Extension__

####3. Report an Issue

Two ways to report an issue:

1. Send Email to <amlovey@qq.com>

2. Open a issue on <https://github.com/amloveyweb/amloveyweb.github.io/issues>

## Release Notes

__V1.2.4__

- Fix some methods disappear from code completion bug
- Hover on variables or type member can show their type now
- Add `Go To definition` for method/variable/structs [Experimental]

__V1.2.3__

- Fix code completion for `half2`
- Add formatting option for place open brace on newline or not

__V1.2.2__

- Support more builtin helper functions
- Fix format bug for condition expression

__V1.2.1__

- More Keywords or functions intellisense for URP/HDRP

__V1.2.0__

- SRP supports: Add path intellisense
- Add property drawer attribute keywords

__V1.1.6__

- Fix format bug

__V1.1.5__

- Fix format by when line ends with '\'
- Add Go to definition support for include files

__V1.1.4__  

Support Linux

__V1.1.3__  

- Auto Format
    - use tab or spaces can be configured by `editor.insertSpaces` VSCode settings

__V1.1.2__  

- Add more completions from UnityCG.cginc.
- Fix document symbols show incorrectly in some scenarios.

__V1.1.1__

- Intellisense
    - Add macros code completion support
    - Add more completion items from UnityCG.cginc, there are:
        - UnityWorldSpaceViewDir
        - UnityWorldToClipPos
        - UnityViewToClipPos
        - UnityWorldToViewPos
        - UnityObjectToWorldDir
        - UnityWorldToObjectDir
        - UnityObjectToWorldNormal
        - UnityWorldSpaceLightDir
    - Fix methods intellisense was broken by ':' in parameters

- Format Document
    - Improve format for marcos

- Syntax Highlighting 
    - Add highlight for `#ifdef` and `#ifndef`

- Add document symbols support, press `CTRL + SHIFT + o` on Windows or `CMD + SHIFT + o` on macOS to open it.

__V1.1.0__

- Intellisense
    - Fix intellisense was broken by "," in structs and fileds in some scenario

- Format Document
    - Fix format for [XX]PROGRAM..END[XX] structure
    - Make #define to match levels

- Experiment:
    - Add .hlsl and .cg file support

__V1.0.9__

- Intellisense
    - Fix wrong result when there are duplicate name of variables

- Syntax Highlighting
    - Add highlighing for custom functions


__V1.0.8__
- Format Document
    - Improve format for Operators

__V1.0.7__
- Intellisense
    - Fix Intellisense broken by '+', '-', '*', '/' in some scenarios

- Format Document
    - Improve format for preprocessor directives

- Syntax Highlighting
    - Improve color of preprocessor directives

__V1.0.6__
- Format Document:
   - fix colon formation is incorrect in #pragma line

- Intellisense
   - Fix wrong code completion result in #pragma line which is triggered by colon
   - Update description for `clip` and `cos` cg method in code completion item

__V1.0.5__
- Add region mark support(Required VSCode version 1.17.0 +). ShaderlabVSCode now supports two type markers:
    - //#region and //#endregion, snippet is `region`
    - //region and //endregion, snippet is `region2`

__V1.0.4__
- Intellisense
    - Add Unity defined Values support, like _Time
    - Fix duplicate members when include same cginc files multiple times

__V1.0.3__

- Intellisense
    - Fix bug variable broken by semicolon

- Editor
    - Improve compability

__V1.0.2b3__
- Auto Format:
    - Add format document feature 
- Intellisense:
    - supports builtin types, like half, fixed and float
    - supports completion of fields of types
    - supports completion of method return type
- Bug Fixes:
    - Fix bug structure fields are broken by comments

__V1.0.1b2__
- Add code snippets support
- Update hover infromation for some keywords
- Fix wrong fields data get from struct in some scenarios
- Fix bug that Variable and Properties Info broken by whitespace

__v1.0.0b1__

- First beta release

------
## For more information

Visit site <http://www.amlovey.com>