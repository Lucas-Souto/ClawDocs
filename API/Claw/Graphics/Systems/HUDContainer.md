# HUDContainer
```csharp
public class HUDContainer
```
Representa uma lista de [HUDElement](/API/Claw/Graphics/Systems/HUDElement.md#HUDElement) s.<br />
## HUDContainer
```csharp
public HUDContainer() { }
```
## Active
```csharp
public bool Active;
```
## Elements
```csharp
public System.Collections.Generic.List<Claw.Graphics.Systems.HUDElement> Elements;
```
## HUDContainer[int element]
```csharp
public Claw.Graphics.Systems.HUDElement HUDContainer[int element] { get; } 
```
## Step
```csharp
public virtual void Step(Claw.Graphics.Systems.HUD hud) { }
```
## Render
```csharp
public virtual void Render(Claw.Graphics.Systems.HUD hud) { }
```
