# SaveObject
```csharp
public class SaveObject
```
Representação de um objeto no save.<br />
## SaveObject
```csharp
public SaveObject() { }
```
## SaveObject[string property]
```csharp
public object SaveObject[string property] { get; set; } 
```
## Lock
```csharp
public virtual void Lock() { }
```
Tranca o objeto para não receber mais mudanças.<br />
## Cast
```csharp
public virtual object Cast(System.Type type, System.Collections.Generic.Dictionary<Claw.Save.ISaveValue,object> references) { }
```
Converte um [SaveObject](/API/Claw/Save/SaveObject.md#SaveObject) em um objeto.<br />
## GetEnumerator
```csharp
public virtual System.Collections.Generic.IEnumerator<System.Collections.Generic.KeyValuePair<string,object>> GetEnumerator() { }
```
