# SpriteFont
```csharp
public sealed class SpriteFont
```
Representa uma fonte, com base numa [Sprite](/API/Claw/Graphics/Sprite.md#Sprite) .<br />
## SpriteFont
```csharp
public SpriteFont(Claw.Graphics.Sprite sprite, Claw.Vector2 spacing, System.Collections.Generic.Dictionary<char,Glyph> glyphs) { }
```
## SpriteFont
```csharp
public SpriteFont(Claw.Graphics.Sprite sprite, Claw.Vector2 spacing, Claw.Vector2 charSize, char[] chars) { }
```
## SpriteFont
```csharp
public SpriteFont(Claw.Graphics.Sprite sprite, Claw.Vector2 spacing, Claw.Vector2 charSize, string chars) { }
```
## Sprite
```csharp
public readonly Claw.Graphics.Sprite Sprite;
```
## Spacing
```csharp
public Claw.Vector2 Spacing;
```
## Glyphs
```csharp
public readonly System.Collections.Generic.Dictionary<char,Glyph> Glyphs;
```
## AddKerning
```csharp
public SpriteFont AddKerning(char first, char second, float value) { }
```
Adiciona um par de kerning para este [SpriteFont](/API/Claw/Graphics/SpriteFont.md#SpriteFont) .<br />
## MeasureString
```csharp
public Claw.Vector2 MeasureString(string text) { }
```
Retorna as dimensões que a [Não encontrado!] teria com este [SpriteFont](/API/Claw/Graphics/SpriteFont.md#SpriteFont) .<br />
## MeasureChar
```csharp
public Claw.Vector2 MeasureChar(char character) { }
```
Retorna as dimensões que o tamanho da área de um [SpriteFont.Glyph](/API/Claw/Graphics/SpriteFont.md#Glyph) .<br />
## ToString
```csharp
public virtual string ToString() { }
```
# Glyph
```csharp
public sealed class Glyph
```
Representa os dados de um único caractere de um [SpriteFont](/API/Claw/Graphics/SpriteFont.md#SpriteFont) .<br />
## Glyph
```csharp
public Glyph(Claw.Rectangle area, System.Collections.Generic.Dictionary<char,float> kerningPair) { }
```
## Area
```csharp
public readonly Claw.Rectangle Area;
```
## KerningPair
```csharp
public readonly System.Collections.Generic.Dictionary<char,float> KerningPair;
```
