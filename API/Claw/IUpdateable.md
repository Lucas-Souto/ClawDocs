# IUpdateable
```csharp
public interface IUpdateable
```
Interface para componentes que fazem parte do Update.<br />
## Enabled
```csharp
public bool Enabled { get; } 
```
## UpdateOrder
```csharp
public int UpdateOrder { get; } 
```
## EnabledChanged
```csharp
public event System.EventHandler<System.EventArgs> EnabledChanged;
```
## UpdateOrderChanged
```csharp
public event System.EventHandler<System.EventArgs> UpdateOrderChanged;
```
## Step
```csharp
public void Step() { }
```
