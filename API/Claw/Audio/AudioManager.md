# AudioManager
```csharp
public sealed class AudioManager
```
Representa o controle de áudios do jogo.<br />
## PauseMusic
```csharp
public bool PauseMusic;
```
## MaxConcurrent
```csharp
public static int MaxConcurrent;
```
Máximo de efeitos sonoros simultâneos.<br />
## FadeSpeed
```csharp
public static float FadeSpeed;
```
Velocidade de transição entre músicas.<br />
## SampleRate
```csharp
public const int SampleRate;
```
## MasterVolume
```csharp
public float MasterVolume { get; set; } 
```
Volume geral (entre 0 e 1).<br />
## MusicVolume
```csharp
public float MusicVolume { get; set; } 
```
Volume geral das músicas (entre 0 e 1).<br />
## OnSoundEffectEnd
```csharp
public event System.Action<Claw.Audio.SoundEffectInstance> OnSoundEffectEnd;
```
Evento executado quando um efeito sonoro termina, sem loop.<br />
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
## GetVolume
```csharp
public float GetVolume(Claw.Audio.SoundEffectGroup group) { }
```
Retorna o volume geral de um grupo.<br />
## SetVolume
```csharp
public void SetVolume(float value, Claw.Audio.SoundEffectGroup group) { }
```
Altera o volume geral de um grupo.<br />
**value**: Entre 0 e 1.<br />
## Play
```csharp
public void Play(Claw.Audio.SoundEffectInstance soundEffect) { }
```
Inicia/reinicia um sonoro.<br />
## Stop
```csharp
public void Stop(Claw.Audio.SoundEffectInstance soundEffect) { }
```
Pausa um efeito sonoro.<br />
## SetMusic
```csharp
public void SetMusic(Claw.Audio.Music music) { }
```
Inicia a troca de música.<br />
