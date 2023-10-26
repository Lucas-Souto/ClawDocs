# SoundEffectInstance
```csharp
public sealed class SoundEffectInstance
```
Representa uma instância de [SoundEffect](/API/Claw/Audio/SoundEffect.md#SoundEffect) .<br />
## SoundEffectInstance
```csharp
public SoundEffectInstance(Claw.Audio.SoundEffect audio, Claw.Audio.SoundEffectGroup group) { }
```
## IsLooped
```csharp
public bool IsLooped;
```
## Group
```csharp
public readonly Claw.Audio.SoundEffectGroup Group;
```
## Volume
```csharp
public float Volume { get; set; } 
```
Volume do áudio (entre 0 e 1).<br />
