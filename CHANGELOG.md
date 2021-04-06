## V1.2.7 

[Thanks to Jaosn Ma and Nixon]

- Better HLSL Supports that add more keywords and builtin methods
- Better folding strategy that base on syntax instead of base on indentation
- Better macros formatting. We can change different styles in `Macros Alignment Modes` settings
- Add `Format Selection` feature
- Improve syntax highlighting for Monokai pro
- Fix bugs that StructuredBuffer show as Buffer type in hover information

## V1.2.6

- Improve syntax highlighting for types and methods
- Add new version notification
- Fix bug that code completion for operation `?:` is not correctly
- Fix bug that F12 cannot jump in included library of SRP

## V1.2.5

- Add more code snippets:
  - `hlp`: HLSLPROGRAM...ENDHLSL block
  - `glp`: GLSLPROGRAM...ENCGLSL block
  - `inc`: #include ""
  - `incpkg`: #include "Pakcages"

## V1.2.4

- Fix some methods disappear from code completion bug
- Hover on variables or type member can show their type now
- Add `Go To definition` for method/variable/structs [Experimental]

## V1.2.3

- Fix code completion for `half2`
- Add formatting option for place open brace on newline or not

## V1.2.2

- Support more builtin helper functions
- Fix format bug for condition expression

## V1.2.1

- More Keywords or functions intellisense for URP/HDRP

## V1.2.0

- SRP supports: Add path intellisense
- Add property drawer attribute keywords

## V1.1.6
- Fix format bug

## V1.1.5

- Fix format by when line ends with '\'
- Add Go to definition support for include files

## V1.1.4
Support Linux

## V1.1.3
- Auto Format
    - use tab or spaces can be configured by `editor.insertSpaces` VSCode settings

## V1.1.2
- Add more completions from UnityCG.cginc.
- Fix document symbols show incorrectly in some scenarios.

## V1.1.1
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

## V1.1.0

- Intellisense
    - Fix intellisense was broken by "," in structs and fileds in some scenario

- Format Document
    - Fix format for [XX]PROGRAM..END[XX] structure
    - Make #define to match levels

- Experiment:
    - Add .hlsl and .cg file support

## V1.0.9
- Intellisense
    - Fix wrong result when there are duplicate name of variables

- Syntax Highlighting
    - Add highlighing for custom functions

## V1.0.8
- Format Document
    - Improve format for Operators

## V1.0.7
- Intellisense
    - Fix Intellisense broken by '+', '-', '*', '/' in some scenarios

- Format Document
    - Improve format for preprocessor directives

- Syntax Highlighting
    - Improve color of preprocessor directives

## V1.0.6
- Format Document:
    - fix colon formation is incorrect in #pragma line

- Intellisense
    - Fix wrong code completion result in #pragma line which is triggered by colon
    - Update description for `clip` and `cos` cg method in code completion item

## V1.0.5
- Add region mark support(Required VSCode version 1.17.0 +). ShaderlabVSCode now supports two type markers:
    - //#region and //#endregion, snippet is `region`
    - //region and //endregion, snippet is `region2`

## V1.0.4
- Intellisense
    - Add Unity defined Values support, like _Time
    - Fix duplicate members when include same cginc files multiple times


## V1.0.3
- Intellisense
    - Fix bug variable broken by semicolon
    
- Editor
    - Improve compability

## V1.0.2b3
- Auto Format:
    - Add format document feature 
- Intellisense:
    - supports builtin types, like half, fixed and float
    - supports completion of fields of types
    - supports completion of method return type
- Bug Fixes:
    - Fix bug structure fields are broken by comments

## V1.0.1b2
- Add code snippets support
- Update hover infromation for some keywords
- Fix wrong fields data get from struct in some scenarios
- Fix bug that Variable and Properties Info broken by whitespace

## v1.0.0b1
- First beta release
