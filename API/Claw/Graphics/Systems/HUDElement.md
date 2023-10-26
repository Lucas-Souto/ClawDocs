# HUDElement
```csharp
public class HUDElement
```
Base de um elemento da HUD do jogo.<br />
## HUDElement
```csharp
public HUDElement() { }
```
## Opacity
```csharp
public float Opacity;
```
## Rotation
```csharp
public float Rotation;
```
## Color
```csharp
public Claw.Color Color;
```
## Flip
```csharp
public Claw.Graphics.Flip Flip;
```
## Position
```csharp
public Claw.Vector2 Position;
```
## Scale
```csharp
public Claw.Vector2 Scale;
```
## Origin
```csharp
public Claw.Vector2 Origin;
```
## GetPosition
```csharp
public Claw.Vector2 GetPosition(Claw.Graphics.Systems.HUD hud) { }
```
Retorna a posição ajustada no hud.<br />
## GetScale
```csharp
public Claw.Vector2 GetScale(Claw.Graphics.Systems.HUD hud) { }
```
Retorna a escala ajustada no hud.<br />
## Step
```csharp
public virtual void Step(Claw.Graphics.Systems.HUD hud) { }
```
## Render
```csharp
public virtual void Render(Claw.Graphics.Systems.HUD hud) { }
```
