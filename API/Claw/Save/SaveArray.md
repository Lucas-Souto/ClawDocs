# SaveArray
```csharp
public class SaveArray : System.Collections.ObjectModel.Collection<object>
```
Representação de um array no save.<br />
## SaveArray
```csharp
public SaveArray() { }
```
## Lock
```csharp
public virtual void Lock() { }
```
Tranca o objeto para não receber mais mudanças.<br />
## InsertItem
```csharp
protected virtual void InsertItem(int index, object item) { }
```
Insere um elemento no array.<br />
## RemoveItem
```csharp
protected virtual void RemoveItem(int index) { }
```
Remove um elemento do array.<br />
## ClearItems
```csharp
protected virtual void ClearItems() { }
```
Limpa o array.<br />
## SetItem
```csharp
protected virtual void SetItem(int index, object item) { }
```
Altera um elemento do array.<br />
## Cast
```csharp
public virtual object Cast(System.Type type, System.Collections.Generic.Dictionary<Claw.Save.ISaveValue,object> references) { }
```
Converte o [SaveArray](/API/Claw/Save/SaveArray#SaveArray) em um [Não encontrado!] .<br />
