# Parallax
```csharp
public sealed class Parallax
```
Representa uma sequência de backgrounds para efeito de parallax.<br />
## Parallax
```csharp
public Parallax() { }
```
## UseDeltaTime
```csharp
public bool UseDeltaTime;
```
## UseScaledDeltaTime
```csharp
public bool UseScaledDeltaTime;
```
## Color
```csharp
public Claw.Color Color;
```
## Position
```csharp
public Claw.Vector2 Position;
```
## Backgrounds
```csharp
public System.Collections.Generic.List<Claw.Graphics.Systems.Background> Backgrounds;
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
## Initialize
```csharp
public virtual void Initialize() { }
```
## ChangeAllSpeed
```csharp
public void ChangeAllSpeed(float value) { }
```
Muda a velocidade de todos os backgrounds.<br />
## ChangeAllZoom
```csharp
public void ChangeAllZoom(float value) { }
```
Muda o zoom de todos os backgrounds.<br />
## ChangeAllDirection
```csharp
public void ChangeAllDirection(Claw.Vector2 value) { }
```
Muda a direção de todos os backgrounds.<br />
## Render
```csharp
public virtual void Render() { }
```
# Axis
```csharp
public enum Axis
```
Define os eixos em que o background poderá se repetir durante o parallax.<br />
|Nome|Valor|Descrição|
|---|---|---|
|Horizontal|0||
|Vertical|1||
