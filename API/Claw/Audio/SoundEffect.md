# SoundEffect
```csharp
public class SoundEffect
```
Representa um efeito sonoro no jogo.<br />
## SoundEffect
```csharp
public SoundEffect(Claw.Audio.Channels channels, float[] samples) { }
```
**samples**: Valores entre -1 e 1.<br />
## Channels
```csharp
public readonly Claw.Audio.Channels Channels;
```
## Length
```csharp
public long Length { get; } 
```
## CreateInstance
```csharp
public Claw.Audio.SoundEffectInstance CreateInstance(Claw.Audio.SoundEffectGroup group) { }
```
Cria um [SoundEffectInstance](/API/Claw/Audio/SoundEffectInstance.md#SoundEffectInstance) deste áudio.<br />
