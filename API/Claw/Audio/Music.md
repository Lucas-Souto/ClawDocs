# Music
```csharp
public class Music
```
Representa uma música no jogo.<br />
## Channels
```csharp
public readonly Claw.Audio.Channels Channels;
```
## Volume
```csharp
public float Volume { get; set; } 
```
Volume da música (entre 0 e 1).<br />
## Length
```csharp
public long Length { get; } 
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
