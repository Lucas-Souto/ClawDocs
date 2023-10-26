# PlatBody
```csharp
public class PlatBody : GameObject
```
Uma classe com física básica de plataforma.<br />
## PlatBody
```csharp
public PlatBody() { }
```
## Grounded
```csharp
protected bool Grounded;
```
## OnGhost
```csharp
protected bool OnGhost;
```
## IgnoreGhost
```csharp
protected bool IgnoreGhost;
```
## ApplyPhysics
```csharp
protected bool ApplyPhysics;
```
## CoyoteTime
```csharp
public static float CoyoteTime;
```
## CornerTolerance
```csharp
public static float CornerTolerance;
```
## TileCollisionLayer
```csharp
public static string TileCollisionLayer;
```
## WasGrounded
```csharp
protected bool WasGrounded { protected get; private set; } 
```
## CanJump
```csharp
protected bool CanJump { protected get; private set; } 
```
## GroundSpeed
```csharp
protected virtual float GroundSpeed { protected get; } 
```
## AirSpeed
```csharp
protected virtual float AirSpeed { protected get; } 
```
## WalkSpeed
```csharp
protected float WalkSpeed { protected get; } 
```
## JumpSpeed
```csharp
protected virtual float JumpSpeed { protected get; } 
```
## Gravity
```csharp
protected virtual float Gravity { protected get; } 
```
## MinSpeed
```csharp
protected virtual Claw.Vector2 MinSpeed { protected get; } 
```
## MaxSpeed
```csharp
protected virtual Claw.Vector2 MaxSpeed { protected get; } 
```
## Bounds
```csharp
public virtual Claw.Rectangle Bounds { get; } 
```
## GetSpeed
```csharp
public Claw.Vector2 GetSpeed() { }
```
Retorna a velocidade do [PlatBody](/API/Claw/Physics/PlatBody.md#PlatBody) .<br />
## Impulse
```csharp
public void Impulse(Claw.Vector2 impulse, bool resetXSpeed, bool resetYSpeed) { }
```
Acrescenta um valor na velocidade do [PlatBody](/API/Claw/Physics/PlatBody.md#PlatBody) .<br />
## Stop
```csharp
public void Stop() { }
```
Zera a velocidade do [PlatBody](/API/Claw/Physics/PlatBody.md#PlatBody) .<br />
## Stop
```csharp
public void Stop(bool horizontal, bool vertical) { }
```
Zera a velocidade do [PlatBody](/API/Claw/Physics/PlatBody.md#PlatBody) .<br />
## Jump
```csharp
public void Jump(float boost) { }
```
Faz com que o [PlatBody](/API/Claw/Physics/PlatBody.md#PlatBody) pule.<br />
**boost**: Multiplica a força do pulo<br />
## Walk
```csharp
public void Walk(float direction) { }
```
Faz com que o [PlatBody](/API/Claw/Physics/PlatBody.md#PlatBody) ande.<br />
## Step
```csharp
public virtual void Step() { }
```
## GetInput
```csharp
protected virtual void GetInput() { }
```
É chamado antes de fazer as checagens de colisão.<br />
## OnHorizontalCollision
```csharp
protected virtual bool OnHorizontalCollision(int platType, Claw.Vector2 collisionPoint) { }
```
É chamado sempre que ocorre uma colisão na horizontal.<br />
**Retorna**: True para zerar a velocidade e corrigir a posição.<br />
## OnVerticalCollision
```csharp
protected virtual bool OnVerticalCollision(int platType, Claw.Vector2 collisionPoint) { }
```
É chamado sempre que ocorre uma colisão na vertical.<br />
**Retorna**: True para zerar a velocidade, corrigir a posição e fazer a checagem de Grounded.<br />
## CustomHorizontalHandler
```csharp
protected virtual void CustomHorizontalHandler() { }
```
É chamado após a checagem de colisão com tiles e antes da movimentação.<br />
## CustomVerticalHandler
```csharp
protected virtual void CustomVerticalHandler() { }
```
É chamado após a checagem de colisão com tiles e antes da movimentação.<br />
# PlatTypes
```csharp
public static class PlatTypes
```
Tipos de plataforma (representam o index 1D do tile).<br />
## Block
```csharp
public static int Block;
```
## DontPassUp
```csharp
public static int DontPassUp;
```
## DontPassDown
```csharp
public static int DontPassDown;
```
## DontPassRight
```csharp
public static int DontPassRight;
```
## DontPassLeft
```csharp
public static int DontPassLeft;
```
## Setup
```csharp
public static void Setup(int block, int dontPassUp, int dontPassDown, int dontPassRight, int dontPassLeft) { }
```
Altera os tiles que representam cada tipo de plataforma.<br />
