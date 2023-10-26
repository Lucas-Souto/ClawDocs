# HUDText
```csharp
public sealed class HUDText : HUDElement
```
Representa um texto na HUD do jogo.<br />
## HUDText
```csharp
public HUDText(string text, Claw.Graphics.SpriteFont font, Claw.Vector2 position, Claw.Vector2 scale, Claw.Vector2 origin) { }
```
## Text
```csharp
public string Text;
```
## Font
```csharp
public Claw.Graphics.SpriteFont Font;
```
## Render
```csharp
public virtual void Render(Claw.Graphics.Systems.HUD hud) { }
```
