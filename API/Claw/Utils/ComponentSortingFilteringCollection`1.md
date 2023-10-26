# ComponentSortingFilteringCollection\<T>
```csharp
public sealed class ComponentSortingFilteringCollection<T>
```
Representa um [GameComponentCollection](/API/Claw/GameComponentCollection.md#GameComponentCollection) filtrado e ordenado.<br />
**T**: Tipo que será filtrado.<br />
## ComponentSortingFilteringCollection\<T>
```csharp
public ComponentSortingFilteringCollection<T>(Claw.GameComponentCollection componentCollection, System.Predicate<T> filter, System.Comparison<T> sort, System.Action<T,System.EventHandler<System.EventArgs>> filterChangedSubscriber, System.Action<T,System.EventHandler<System.EventArgs>> filterChangedUnsubscriber, System.Action<T,System.EventHandler<System.EventArgs>> sortChangedSubscriber, System.Action<T,System.EventHandler<System.EventArgs>> sortChangedUnsubscriber) { }
```
Cria uma lista de componenetes que será sempre o produto filtrado e ordenado de uma [GameComponentCollection](/API/Claw/GameComponentCollection.md#GameComponentCollection) .<br />
**componentCollection**: A coleção original.<br />
**filter**: A condição para a filtragem.<br />
**sort**: O que servirá de parâmetro para a ordenação.<br />
**filterChangedSubscriber**: Adiciona o evento que deverá ser chamado quando o filtro mudar de valor.<br />
**filterChangedUnsubscriber**: Remove o evento que deverá ser chamado quando o filtro mudar de valor.<br />
**sortChangedSubscriber**: Adiciona o evento que deverá ser chamado quando a ordem mudar de valor.<br />
**sortChangedUnsubscriber**: Remove o evento que deverá ser chamado quando a ordem mudar de valor.<br />
## ComponentCollection
```csharp
public readonly Claw.GameComponentCollection ComponentCollection;
```
## Count
```csharp
public int Count { get; } 
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## ForEach
```csharp
public void ForEach(System.Action<T> action) { }
```
Executa uma ação para cada elemento da coleção.<br />
