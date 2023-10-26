# ParticleEmitter
```csharp
public sealed class ParticleEmitter : Claw.DrawableGameComponent
```
Classe de emissão e manuseio de partículas.<br />
## ParticleEmitter
```csharp
public ParticleEmitter(Claw.Particles.ParticleEmitterConfig config) { }
```
## ParticleEmitter
```csharp
public ParticleEmitter() { }
```
## Position
```csharp
public Claw.Vector2 Position;
```
## DrawOffset
```csharp
public Claw.Vector2 DrawOffset;
```
## ParticleOriginDistortion
```csharp
public Claw.Vector2 ParticleOriginDistortion;
```
## Stopped
```csharp
public bool Stopped;
```
## PauseParticles
```csharp
public bool PauseParticles;
```
## Config
```csharp
public Claw.Particles.ParticleEmitterConfig Config;
```
Configuração da emissão de partículas.<br />
## PoolCount
```csharp
public static int PoolCount() { }
```
Retorna a quantidade de partículas que estão esperando na pool.<br />
## ClearPool
```csharp
public static void ClearPool() { }
```
Limpa a lista de partículas que estão esperando na pool.<br />
## Count
```csharp
public int Count() { }
```
Retorna a quantidade de partículas deste [ParticleEmitter](/API/Claw/Particles/ParticleEmitter.md#ParticleEmitter) .<br />
## Clear
```csharp
public void Clear() { }
```
Elimina todas as partículas.<br />
## Emit
```csharp
public void Emit(Claw.Vector2 basePosition, float? direction) { }
```
Emite partículas em uma direção.<br />
**direction**: Null para deixar o [ParticleValue<T>](/API/Claw/Particles/ParticleValue`1.md#ParticleValue\<T>) como padrão. A direção deve ser em graus.<br />
## Step
```csharp
public void Step() { }
```
## Render
```csharp
public void Render() { }
```
