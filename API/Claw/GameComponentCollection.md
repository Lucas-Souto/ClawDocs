# GameComponentCollection
```csharp
public sealed class GameComponentCollection : System.Collections.ObjectModel.Collection<Claw.IGameComponent>
```
Uma coleção de instâncias de [IGameComponent](/API/Claw/IGameComponent#IGameComponent) .<br />
## GameObjects
```csharp
public System.Collections.ObjectModel.ReadOnlyCollection<Claw.GameObject> GameObjects;
```
Filtragem dos game objects dessa coleção (fora de ordem).<br />
## ComponentAdded
```csharp
public event System.EventHandler<Claw.IGameComponent> ComponentAdded;
```
## ComponentRemoved
```csharp
public event System.EventHandler<Claw.IGameComponent> ComponentRemoved;
```
## CreateForUpdate
```csharp
public Claw.Utils.ComponentSortingFilteringCollection<Claw.IUpdateable> CreateForUpdate() { }
```
Cria um [ComponentSortingFilteringCollection<T>](/API/Claw/Utils/ComponentSortingFilteringCollection`1#ComponentSortingFilteringCollection\<T>) configurado.<br />
## CreateForDraw
```csharp
public Claw.Utils.ComponentSortingFilteringCollection<Claw.IDrawable> CreateForDraw() { }
```
Cria um [ComponentSortingFilteringCollection<T>](/API/Claw/Utils/ComponentSortingFilteringCollection`1#ComponentSortingFilteringCollection\<T>) configurado.<br />
## InsertItem
```csharp
protected virtual void InsertItem(int index, Claw.IGameComponent component) { }
```
Adiciona um [IGameComponent](/API/Claw/IGameComponent#IGameComponent) na coleção e chama o evento [GameComponentCollection.ComponentAdded](/API/Claw/GameComponentCollection#ComponentAdded) .<br />
## RemoveItem
```csharp
protected virtual void RemoveItem(int index) { }
```
Remove um [IGameComponent](/API/Claw/IGameComponent#IGameComponent) da coleção e chama o evento [GameComponentCollection.ComponentRemoved](/API/Claw/GameComponentCollection#ComponentRemoved) .<br />
## ClearItems
```csharp
protected virtual void ClearItems() { }
```
Remove todos os os [IGameComponent](/API/Claw/IGameComponent#IGameComponent) da coleção e chama o evento [GameComponentCollection.ComponentRemoved](/API/Claw/GameComponentCollection#ComponentRemoved) para cada um.<br />
## SetItem
```csharp
protected virtual void SetItem(int index, Claw.IGameComponent item) { }
```
