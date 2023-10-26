# Game
```csharp
public class Game
```
Classe central do jogo.<br />
## Game
```csharp
public Game() { }
```
## Instance
```csharp
public static Game Instance { get; private set; } 
```
## Window
```csharp
public Claw.Window Window { get; private set; } 
```
## Renderer
```csharp
public Claw.Graphics.Renderer Renderer { get; private set; } 
```
## Audio
```csharp
public Claw.Audio.AudioManager Audio { get; private set; } 
```
## Tilemap
```csharp
public Claw.Tilemap Tilemap { get; set; } 
```
## Components
```csharp
public Claw.GameComponentCollection Components { get; } 
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
## Run
```csharp
public void Run() { }
```
Tenta inicializar o jogo e, se obter sucesso, executa o [Game.Initialize](/API/Claw/Game.md#Initialize) e o game loop.<br />
## Close
```csharp
public void Close() { }
```
Fecha o jogo.<br />
## Initialize
```csharp
protected virtual void Initialize() { }
```
## Step
```csharp
protected virtual void Step() { }
```
## Render
```csharp
protected virtual void Render() { }
```
