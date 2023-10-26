# TextConfig
```csharp
public sealed class TextConfig
```
Define as configurações para a renderização do [TextRenderer](/API/Claw/Graphics/Systems/TextRenderer.md#TextRenderer) .<br />
## TextConfig
```csharp
public TextConfig() { }
```
## TextConfig
```csharp
public TextConfig(float? rotation, Color? color, Vector2? scale, TextOrigin? origin, TextEffect? effect, Claw.Graphics.SpriteFont font, Flip? flip) { }
```
## Rotation
```csharp
public float? Rotation;
```
## Color
```csharp
public Color? Color;
```
## Scale
```csharp
public Vector2? Scale;
```
## Origin
```csharp
public TextOrigin? Origin;
```
## Effect
```csharp
public TextEffect? Effect;
```
## Font
```csharp
public Claw.Graphics.SpriteFont Font;
```
## Flip
```csharp
public Flip? Flip;
```
## Copy
```csharp
public void Copy(TextConfig other) { }
```
Copia os valores de um outro [TextConfig](/API/Claw/Graphics/Systems/TextConfig.md#TextConfig) .<br />
