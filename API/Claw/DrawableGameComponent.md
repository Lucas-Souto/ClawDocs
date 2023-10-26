# DrawableGameComponent
```csharp
public class DrawableGameComponent : GameComponent
```
Classe pronta de um [IGameComponent](/API/Claw/IGameComponent.md#IGameComponent) do tipo [IUpdateable](/API/Claw/IUpdateable.md#IUpdateable) e [IDrawable](/API/Claw/IDrawable.md#IDrawable) .<br />
## DrawableGameComponent
```csharp
public DrawableGameComponent() { }
```
## DrawOrder
```csharp
public virtual int DrawOrder { get; set; } 
```
## Visible
```csharp
public virtual bool Visible { get; set; } 
```
## VisibleChanged
```csharp
public event System.EventHandler<System.EventArgs> VisibleChanged;
```
## DrawOrderChanged
```csharp
public event System.EventHandler<System.EventArgs> DrawOrderChanged;
```
## Render
```csharp
public virtual void Render() { }
```
