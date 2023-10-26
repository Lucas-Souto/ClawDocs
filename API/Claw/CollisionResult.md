# CollisionResult
```csharp
public struct CollisionResult
```
Dados do resultado de uma colisão.<br />
## CollisionResult
```csharp
public CollisionResult(bool intersect, Claw.Vector2? collisionPoint, Claw.GameObject gameObject, Claw.Polygon polygon) { }
```
## Intersect
```csharp
public bool Intersect { get; private set; } 
```
## CollisionPoint
```csharp
public Claw.Vector2? CollisionPoint { get; private set; } 
```
## GameObject
```csharp
public Claw.GameObject GameObject { get; private set; } 
```
## Polygon
```csharp
public Claw.Polygon Polygon { get; private set; } 
```
## Equals
```csharp
public virtual bool Equals(object obj) { }
```
## GetHashCode
```csharp
public virtual int GetHashCode() { }
```
## operator ==
```csharp
public static bool operator ==(CollisionResult a, CollisionResult b) { }
```
## operator !=
```csharp
public static bool operator !=(CollisionResult a, CollisionResult b) { }
```
## operator ==
```csharp
public static bool operator ==(CollisionResult a, bool b) { }
```
## operator !=
```csharp
public static bool operator !=(CollisionResult a, bool b) { }
```
## operator ==
```csharp
public static bool operator ==(CollisionResult a, Claw.Vector2 b) { }
```
## operator !=
```csharp
public static bool operator !=(CollisionResult a, Claw.Vector2 b) { }
```
## operator ==
```csharp
public static bool operator ==(CollisionResult a, Claw.GameObject b) { }
```
## operator !=
```csharp
public static bool operator !=(CollisionResult a, Claw.GameObject b) { }
```
## operator ==
```csharp
public static bool operator ==(CollisionResult a, Claw.Polygon b) { }
```
## operator !=
```csharp
public static bool operator !=(CollisionResult a, Claw.Polygon b) { }
```
## implicit operator
```csharp
public static bool implicit operator(CollisionResult a) { }
```
## implicit operator
```csharp
public static Claw.Vector2? implicit operator(CollisionResult a) { }
```
## implicit operator
```csharp
public static Claw.GameObject implicit operator(CollisionResult a) { }
```
## implicit operator
```csharp
public static Claw.Polygon implicit operator(CollisionResult a) { }
```
