## Syntax Highlighting

![](./assets/Syntax-Highlighting.png)

## Code Completion

![](./assets/Code-Completion.png)

## Hover Information

![](./assets/Hover-Information.png)

## Signature Help

![](./assets/Signature-Help.png)

## Document Symbols

Press `CTRL + SHIFT + o` on Windows or `CMD + SHIFT + o` on macOS.

![](./assets/Document-Symbols.png)

## Go To Definition

`This feature is available in 1.2.4 +`

Press `F12` to trigger `Go To Definition` command Or Click the `Go To Definition` in right click context menu 

![](./assets/GoToDefinition.gif)

## Code Snippets

![](./assets/Snippets.png)

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

#### Format Document

Two ways to format document:

1. Right click the editor area and select __Format Document__ menu in context menu  
2. Open __Command Palette__ and type "Format Document", and then press `ENTER` key on keyborad.

![](./assets/AutoFormat.gif)

#### Format Selection

Two ways to format selection:

1. Right click the editor area and select __Format Selection__ menu in context menu  
2. Open __Command Palette__ and type "Format Selection", and then press `ENTER` key on keyborad

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

### Macros Alignment Modes

In Settings, there is an item under `ShaderlabVScode` section named `Formatting: Style`, change the `Macros alignment modes` to set formatting mode for macros.

#### Indentation with hierachy

```csharp
Subshader 
{
    Pass
    {
        CGPROGRAM
        void MacroTest()
        {
            float c;
            #if 0
                c = 0;
                #if 1
                    c = 1;
                #endif
            #endif
        }
        ENDCG
    }
}
```

### Indentation without hierachy

```csharp
Subshader 
{
    Pass
    {
        CGPROGRAM
        void MacroTest()
        {
            float c;
         #if 0
                c = 0;
         #if 1
                c = 1;
         #endif
         #endif
        }
        ENDCG
    }
}
```

#### No Indentation but with hierachy

```csharp
Subshader 
{
    Pass
    {
        CGPROGRAM
        void MacroTest()
        {
            float c;
#if 0
            c = 0;
    #if 1
            c = 1;
    #endif
#endif
        }
        ENDCG
    }
}
```

### No Indentation and without hierachy

```csharp
Subshader 
{
    Pass
    {
        CGPROGRAM
        void MacroTest()
        {
            float c;
#if 0
            c = 0;
#if 1
            c = 1;
#endif
#endif
        }
        ENDCG
    }
}
```

### Doc Comment

Doc Comments are the comments start with `///`. for eaxmple:

```csharp
/// Return max value of a and b
float Max(float a, float b) 
{

}
```

**Hover Information** and **Signature Help** will display doc comments as documentation.

**NOTE:** Doc comment supports Markdown

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
