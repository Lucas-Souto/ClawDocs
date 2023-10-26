# Polygon
```csharp
public sealed class Polygon
```
Representa um colisor poligonal.<br />
## Polygon
```csharp
public Polygon(Claw.GameObject gameObject) { }
```
## Polygon
```csharp
public Polygon(Claw.GameObject gameObject, Claw.Line[] lines) { }
```
## CanRotate
```csharp
public bool CanRotate;
```
## CanScale
```csharp
public bool CanScale;
```
## Offset
```csharp
public Claw.Vector2 Offset;
```
## GameObject
```csharp
public readonly Claw.GameObject GameObject;
```
## Lines
```csharp
public Claw.Line[] Lines;
```
## Enabled
```csharp
public bool Enabled { get; set; } 
```
## LinesInWorld
```csharp
public Claw.Line[] LinesInWorld { get; } 
```
## Top
```csharp
public float Top { get; } 
```
## Bottom
```csharp
public float Bottom { get; } 
```
## Right
```csharp
public float Right { get; } 
```
## Left
```csharp
public float Left { get; } 
```
## Center
```csharp
public Claw.Vector2 Center { get; } 
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
## Box
```csharp
public static Polygon Box(Claw.GameObject gameObject, Claw.Rectangle rectangle) { }
```
Cria um colisor quadrado.<br />
## Circle
```csharp
public static Polygon Circle(Claw.GameObject gameObject, float radius, Claw.Vector2 center, int segments) { }
```
Cria um colisor circular.<br />
## OverlapPolygon
```csharp
public static Claw.CollisionResult OverlapPolygon(Polygon polygon, System.Collections.Generic.IEnumerable<Claw.Line> lines) { }
```
Checa se um polígono está colidindo com outro (formado apenas por linhas).<br />
## Intersect
```csharp
public static Claw.CollisionResult Intersect(Claw.Vector2 point, Polygon polygon) { }
```
Checa se um ponto está colidindo com um [Polygon](/API/Claw/Polygon.md#Polygon) .<br />
## Intersect
```csharp
public static Claw.CollisionResult Intersect(Claw.Vector2 point, string tag, float distance, bool first) { }
```
Checa se um ponto está colidindo com um [Polygon](/API/Claw/Polygon.md#Polygon) .<br />
## Intersect
```csharp
public static Claw.CollisionResult Intersect<T>(Claw.Vector2 point, float distance, bool first) { }
```
Checa se um ponto está colidindo com um [Polygon](/API/Claw/Polygon.md#Polygon) .<br />
## Intersect
```csharp
public static Claw.CollisionResult Intersect(Polygon polygon, Polygon other) { }
```
Checa se dois polígonos estão colidindo.<br />
## Intersect
```csharp
public static Claw.CollisionResult Intersect(Polygon polygon, string tag, float distance, bool first, bool invert) { }
```
Checa se dois polígonos estão colidindo.<br />
## Intersect
```csharp
public static Claw.CollisionResult Intersect<T>(Polygon polygon, float distance, bool first, bool invert) { }
```
Checa se dois polígonos estão colidindo.<br />
## IntersectRay
```csharp
public static Claw.CollisionResult IntersectRay(Claw.Line ray, Polygon polygon, float cellSize) { }
```
Checa se uma linha está colidindo com um [Polygon](/API/Claw/Polygon.md#Polygon) .<br />
## IntersectRay
```csharp
public static Claw.CollisionResult IntersectRay(Claw.Line ray, string tag, float distance, bool first, float cellSize) { }
```
Checa se uma linha está colidindo com um [Polygon](/API/Claw/Polygon.md#Polygon) .<br />
## IntersectRay
```csharp
public static Claw.CollisionResult IntersectRay<T>(Claw.Line ray, float distance, bool first, float cellSize) { }
```
Checa se uma linha está colidindo com um [Polygon](/API/Claw/Polygon.md#Polygon) .<br />
## IntersectList
```csharp
public static Claw.CollisionResult[] IntersectList(Claw.Vector2 point, System.Func<Claw.GameObject,bool> predicate) { }
```
Retorna uma lista de colisões com o ponto especificado.<br />
## IntersectList
```csharp
public static Claw.CollisionResult[] IntersectList(Polygon polygon, System.Func<Claw.GameObject,bool> predicate) { }
```
Retorna uma lista de colisões com o polígono especificado.<br />
## IntersectWith
```csharp
public static Claw.CollisionResult IntersectWith(Claw.Vector2 point, System.Collections.Generic.IEnumerable<Claw.GameObject> gameObjects, float distance, bool first) { }
```
Checa se um ponto está colidindo com um dos [Polygon](/API/Claw/Polygon.md#Polygon) s de uma lista.<br />
## IntersectWith
```csharp
public static Claw.CollisionResult IntersectWith(Polygon polygon, System.Collections.Generic.IEnumerable<Claw.GameObject> gameObjects, float distance, bool first, bool invert) { }
```
Checa se um [Polygon](/API/Claw/Polygon.md#Polygon) está colidindo com um dos [Polygon](/API/Claw/Polygon.md#Polygon) s de uma lista.<br />
