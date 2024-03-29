# CHANGE LOGS

### Version 1.5.1

**NEW:**
- Add support for methods in structs for Signature Help and hover information
- Add support for methods of Shader Model 5 Objects [Expiremental]
- Add keyword `globallycoherent`

**IMPROVE:**
- Unsigned integer will highlight as same as other number type now
- Fix method definition highlight is not correct when the return type is struct

**FIX:**
- Fix Code completion items will duplicated or missing when structs have overloaded methods
- Fix auto fill result for document commment is not correct when break line by `Enter` key

### Version 1.5.0

**IMPROVE**: Fix possible memory leak issue, **RECOMMEND EVERYONE TO UPDATE TO THIS VERSION**

### Version 1.4.7

**NEW:**
- BetterShaders Supports [Expiremental]
    - Add Syntax Highlighting support
    - Add Outline support
- More keywords for Stencil operation values

**IMPROVE:**
- Improve performance via caching system

### Version 1.4.6

**IMPROVE**
- Improve property drawer completions
- Add more keywords in Code Completion

**FIXED**
- Fix include files in HLSLINCLUDE/CGINCLUDE block are ignored

### Version 1.4.5

**IMPROVE**
- Turn off time cost features when openning generated or compiled shader from Unity Editor. The features can be turn on/off in settings

**FIXED**
- Fix fields of types are not correct in some case
- Fix `?:` format is not correct in some case
- Fix completion for `RequireOptions` tag

### Version 1.4.3

**IMPROVE:**
- Improve accuracy and speed of Go To Definition
- Improve accuracy of Code Completion
- Improve accuracy of Document Symbol

**FIXED:**
- Fix typo of 'multi_compile' in completion list
- Fix nested included shader library is not working 

### Version 1.4.2

- **HOT FIX**: Fix Code completion are not works on windows sometimes 

### Version 1.4.1

**IMPROVE:**
- Suppports Local packages which are binplaced under project root path

**FIXED:**
- Fix hover on variables from parameter will show methods doc comment
- Fix Go To Definition cann not find location of symbols when mulitple files included in some cases
- Fix double click shader file in packages may open blank file

### Version 1.4.0

**NEW:**
- Add **Doc Comment** feature. Doc comments are the comments start with `///`. **Hover Information** and **Signature Help** will display doc comments as documentation
- Add methods of structs suppport in Code Completions

**IMPROVED:**
- Signature Help will display current signature with same parameters number 
- Document Symbol supports static methods

**FIXED**
- Fix signature help is broken for custom methods in same shader file
- Fix variables is missing from completion list when its type defined in active document
- Fix document symbol is not working when there are invalid path in include files line

### Version 1.3.5

**FIXED:**
- Fix signature help broken for some unity built-in methods
- Fix indent level are not correct for some macros
- Fix confused description for method `UnityWorldSpaceViewDir`

### Version1.3.4

**NEW:**
- Add method overload supports (Experimental)

**IMPROVED:**
- Improve Signature Help that supports call out in mutiple lines code

**FIXED:**
- Fix formatter will add new spaces after document formattion in block comments
- Fix EditorConfig not works for new version of EditorConfig for VSCode Extension

### Version1.3.3

**NEW:**
- Add local packages support
- Add vfxshader support (Experimental)

**IMPROVED:**
- Improve shader script template workflow

**FIXED:**
- Fix Go To Definition does not work for struct in generic
- Fix some formatter bugs
- Fix double click shader cannot open VSCode sometimes in Unity 2020+

### Version1.3.2

**NEW:**
- Add `shader_feature` and `multiple_compile` keywords
- Add `UnityPBSLighting.cginc` as default linked library
- Add ability to create HLSL shader via `Create->Shader->HLSL Shader` menu in Unity Editor (Restart Unity Editor is required)

**IMPROVED:**
- Optimize VSCode finding algorithm to support doulble click shader file will open VSCode even it installed non default path on Windows

**FIXED:**
- Fix `- -1` will format as `-- 1` bug

### Version1.3.1

**IMPROVED:**
- Improve supports for shaders inside Packages folders
- Improve formatting for marcos methods

### Version1.3.0

**NEW:**
- Add supports for shader inside Packages folder
- Auto format supports switch..case now
- Auto format supports config tags style now

**IMPROVED:**
- Improve syntax highlighting

**FIXED:**
- Fix bug that fields of struct are missing in code completion when struct has macros

### Version1.2.9

**NEW:**
- Auto Format supports Editor Config now

**IMPROVED:**
- Improve syntax highlighting for operators

**FIXED:**
- Fix Code Completion is not correct for fields of struct with methods
- Fix some minor bugs

### Version1.2.8

**IMPROVED:**
- Improve Code Completion that supports multiple level included libraries.

**FIXED:**
- Fix `Go To Definition` don't works in for loop
- Fix some minor bugs

### Version1.2.7

[Thanks to Jaosn Ma and Nixon]

**NEW:**
- Add `Format Selection` feature

**IMPROVED:**
- Better HLSL Supports that add more keywords and builtin methods
- Better folding strategy that base on syntax instead of base on indentation
- Better macros formatting. We can change different styles in `Macros Alignment Modes` settings
- Improve syntax highlighting for Monokai pro

**FIXED:**
- Fix bugs that StructuredBuffer show as Buffer type in hover information

### Version1.2.6

**NEW:**
- Add new version notification

**IMPROVED:**
- Improve syntax highlighting for types and methods

**FIXED:**
- Fix bug that code completion for operation `?:` is not correctly
- Fix bug that F12 cannot jump in included library of SRP

### Version1.2.5

**NEW:**
- Add more code snippets:
  - `hlp`: HLSLPROGRAM...ENDHLSL block
  - `glp`: GLSLPROGRAM...ENCGLSL block
  - `inc`: #include ""
  - `incpkg`: #include "Pakcages"

### Version1.2.4

**NEW:**
- Add `Go To definition` for method/variable/structs [Experimental]
- Hover on variables or type member can show their type now

**FIXED:**
- Fix some methods disappear from code completion bug

### Version1.2.3

**NEW:**
- Add formatting option for place open brace on newline or not

**FIXED:**
- Fix code completion for `half2`

### Version1.2.2

**NEW:**
- Support more builtin helper functions

**FIXED:**
- Fix format bug for condition expression

### Version1.2.1

**NEW:**
- More Keywords or functions intellisense for URP/HDRP

### Version1.2.0

**NEW:**
- SRP supports: Add path intellisense
- Add property drawer attribute keywords

### Version1.1.6

**FIXED:**
- Fix format bug

### Version1.1.5
**NEW:**
- Add Go to definition support for include files

**FIXED:**
- Fix format by when line ends with '\'

### Version1.1.4

**NEW:**
- Support Linux

### Version1.1.3

**NEW:**
- Auto Format: use tab or spaces can be configured by `editor.insertSpaces` VSCode settings

### Version1.1.2

**NEW:**
- Add more completions from UnityCG.cginc.

**FIXED:**
- Fix document symbols show incorrectly in some scenarios.

### Version1.1.1

**NEW:**
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

- Syntax Highlighting
    - Add highlight for `#ifdef` and `#ifndef`

- Add document symbols support, press `CTRL + SHIFT + o` on Windows or `CMD + SHIFT + o` on macOS to open it.

**IMPROVED:**
- Format Document
    - Improve format for marcos

### Version1.1.0

**NEW:**
- Add .hlsl and .cg file support

**FIXED:**
- Fix intellisense was broken by "," in structs and fileds in some scenario
- Fix format for [XX]PROGRAM..END[XX] structure
- Fix Make #define to match levels

### Version1.0.9

**NEW:**
- Add highlighing for custom functions

**FIXED:**
- Intellisense: Fix wrong result when there are duplicate name of variables

### Version1.0.8

**IMPROVED:**
- Format Document: Improve format for Operators

### Version1.0.7

**IMPROVED:**
- Format Document: Improve format for preprocessor directives
- Syntax Highlighting: Improve color of preprocessor directives

**FIXED:**
- Fix Intellisense broken by '+', '-', '*', '/' in some scenarios

### Version1.0.6

**IMPROVED:**
- Update description for `clip` and `cos` cg method in code completion item

**FIXED:**
- fix colon formation is incorrect in #pragma line
- Fix wrong code completion result in #pragma line which is triggered by colon

### Version1.0.5

**NEW:**
- Add region mark support(Required VSCode version 1.17.0 +). ShaderlabVSCode now supports two type markers:
    - //#region and //#endregion, snippet is `region`
    - //region and //endregion, snippet is `region2`

### Version1.0.4

**NEW:**
- Add Unity defined Values support, like _Time

**FIXED:**
- Fix duplicate members when include same cginc files multiple times


### Version1.0.3

**FIXED:**
- Fix bug variable broken by semicolon

**IMPROVED:**
- Improve compability

### Version1.0.2b3

**NEW:**
- Add format document feature
- Intellisense:
    - supports builtin types, like half, fixed and float
    - supports completion of fields of types
    - supports completion of method return type

**FIXED:**
- Fix bug structure fields are broken by comments

### Version1.0.1b2

**NEW:**
- Add code snippets support

**IMPROVED:**
- Update hover infromation for some keywords

**FIXED:**
- Fix wrong fields data get from struct in some scenarios
- Fix bug that Variable and Properties Info broken by whitespace

### Version1.0.0b1
- First beta release
