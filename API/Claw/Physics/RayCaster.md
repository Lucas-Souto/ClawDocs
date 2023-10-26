# RayCaster
```csharp
public static class RayCaster
```
Calculador de raycast.<br />
## Cast
```csharp
public static void Cast(Claw.Line ray, System.Func<Claw.Vector2,bool> onMove, out Claw.Vector2? hitPoint, Claw.Vector2 cellSize) { }
```
## Cast
```csharp
public static void Cast(Claw.Line ray, float maxDistance, System.Func<Claw.Vector2,bool> onMove, out Claw.Vector2? hitPoint, Claw.Vector2 cellSize) { }
```
