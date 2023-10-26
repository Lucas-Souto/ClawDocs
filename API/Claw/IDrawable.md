# IDrawable
```csharp
public interface IDrawable
```
Interface para componentes que fazem parte do Draw.<br />
## Visible
```csharp
public bool Visible { get; } 
```
## DrawOrder
```csharp
public int DrawOrder { get; } 
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
public void Render() { }
```
