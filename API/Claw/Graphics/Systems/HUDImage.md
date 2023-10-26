# HUDImage
```csharp
public sealed class HUDImage : Claw.Graphics.Systems.HUDElement
```
Representa uma imagem na HUD do jogo.<br />
## HUDImage
```csharp
public HUDImage(Claw.Graphics.Sprite sprite, Claw.Rectangle spriteArea, Claw.Vector2 position, Claw.Vector2 scale, Claw.Vector2 origin) { }
```
## HUDImage
```csharp
public HUDImage(Claw.Animator animator, Claw.Vector2 position, Claw.Vector2 scale) { }
```
## Sprite
```csharp
public virtual Claw.Graphics.Sprite Sprite { get; set; } 
```
## SpriteArea
```csharp
public virtual Claw.Rectangle? SpriteArea { get; set; } 
```
## Origin
```csharp
public virtual Claw.Vector2 Origin { get; set; } 
```
## Animator
```csharp
public Claw.Animator Animator { get; set; } 
```
## Step
```csharp
public virtual void Step(Claw.Graphics.Systems.HUD hud) { }
```
## Render
```csharp
public virtual void Render(Claw.Graphics.Systems.HUD hud) { }
```
