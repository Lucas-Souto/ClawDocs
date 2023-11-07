# SceneManager
```csharp
public static class SceneManager
```
Realiza o manuseio dos [GameObject](/API/Claw/GameObject.md#GameObject) s da cena.<br />
## InstanceNearest
```csharp
public static Claw.GameObject InstanceNearest(string tag, Claw.Vector2 position, bool filterEnabled) { }
```
Encontra a instância mais próxima na cena com uma tag específica.<br />
## InstanceNearest
```csharp
public static Claw.GameObject InstanceNearest<T>(Claw.Vector2 position, bool filterEnabled) { }
```
Encontra a instância mais próxima na cena com um componente de um tipo específico.<br />
## FindObjectByTag
```csharp
public static Claw.GameObject FindObjectByTag(string tag, bool filterEnabled) { }
```
Encontra um objeto com uma tag específica.<br />
## FindObjectsByTag
```csharp
public static System.Collections.Generic.IEnumerable<Claw.GameObject> FindObjectsByTag(string tag, bool filterEnabled) { }
```
Encontra objetos com uma tag específica.<br />
## TagCount
```csharp
public static int TagCount(string tag) { }
```
Retorna o número de objetos com uma tag específica.<br />
## FindObjectByName
```csharp
public static Claw.GameObject FindObjectByName(string name, bool filterEnabled) { }
```
Encontra um objeto com um nome específico.<br />
## FindObjectsByName
```csharp
public static System.Collections.Generic.IEnumerable<Claw.GameObject> FindObjectsByName(string name, bool filterEnabled) { }
```
Encontra objetos com um nome específico.<br />
## FindObjectOfType
```csharp
public static T FindObjectOfType<T>(bool filterEnabled) { }
```
Encontra um objeto de um tipo.<br />
## FindObjectsOfType
```csharp
public static System.Collections.Generic.IEnumerable<Claw.GameObject> FindObjectsOfType<T>(bool filterEnabled) { }
```
Encontra objetos de um tipo.<br />
## ClearScene
```csharp
public static void ClearScene(bool runDestroy, bool deleteAll) { }
```
Destrói os objetos da cena.<br />
## Destroy
```csharp
public static void Destroy(Claw.GameObject gameObject, bool runDestroy) { }
```
Destrói um objeto.<br />
