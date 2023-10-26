# GameComponent
```csharp
public class GameComponent
```
Classe pronta de um [IGameComponent](/API/Claw/IGameComponent#IGameComponent) do tipo [IUpdateable](/API/Claw/IUpdateable#IUpdateable) .<br />
## GameComponent
```csharp
public GameComponent() { }
```
## UpdateOrder
```csharp
public virtual int UpdateOrder { get; set; } 
```
## Enabled
```csharp
public virtual bool Enabled { get; set; } 
```
## EnabledChanged
```csharp
public event System.EventHandler<System.EventArgs> EnabledChanged;
```
## UpdateOrderChanged
```csharp
public event System.EventHandler<System.EventArgs> UpdateOrderChanged;
```
## Initialize
```csharp
public virtual void Initialize() { }
```
## Step
```csharp
public virtual void Step() { }
```
