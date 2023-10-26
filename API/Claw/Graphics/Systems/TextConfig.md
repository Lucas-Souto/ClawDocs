# TextConfig
```csharp
public sealed class TextConfig
```
Define as configurações para a renderização do [TextRenderer](/API/Claw/Graphics/Systems/TextRenderer#TextRenderer) .<br />
## TextConfig
```csharp
public TextConfig() { }
```
## TextConfig
```csharp
public TextConfig(float? rotation, Claw.Color? color, Claw.Vector2? scale, Claw.Graphics.Systems.TextOrigin? origin, Claw.Graphics.Systems.TextEffect? effect, Claw.Graphics.SpriteFont font, Claw.Graphics.Flip? flip) { }
```
## Rotation
```csharp
public float? Rotation;
```
## Color
```csharp
public Claw.Color? Color;
```
## Scale
```csharp
public Claw.Vector2? Scale;
```
## Origin
```csharp
public Claw.Graphics.Systems.TextOrigin? Origin;
```
## Effect
```csharp
public Claw.Graphics.Systems.TextEffect? Effect;
```
## Font
```csharp
public Claw.Graphics.SpriteFont Font;
```
## Flip
```csharp
public Claw.Graphics.Flip? Flip;
```
## Copy
```csharp
public void Copy(TextConfig other) { }
```
Copia os valores de um outro [TextConfig](/API/Claw/Graphics/Systems/TextConfig#TextConfig) .<br />
