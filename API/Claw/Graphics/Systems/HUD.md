# HUD
```csharp
public sealed class HUD
```
Representa a HUD do jogo.<br />
## HUD
```csharp
public HUD() { }
```
## Offset
```csharp
public Claw.Vector2 Offset;
```
## Scale
```csharp
public Claw.Vector2 Scale;
```
## Containers
```csharp
public System.Collections.Generic.Dictionary<string,Claw.Graphics.Systems.HUDContainer> Containers;
```
## HUD[string container]
```csharp
public Claw.Graphics.Systems.HUDContainer HUD[string container] { get; } 
```
## HUD[string container, int element]
```csharp
public Claw.Graphics.Systems.HUDElement HUD[string container, int element] { get; } 
```
## Step
```csharp
public void Step() { }
```
## Render
```csharp
public void Render() { }
```
