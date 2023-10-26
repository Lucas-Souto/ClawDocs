# Layer
```csharp
public sealed class Layer
```
Representa uma camada dentro do [Tilemap](/API/Claw/Tilemap.md#Tilemap) .<br />
## Opacity
```csharp
public float Opacity;
```
## Color
```csharp
public Claw.Color Color;
```
## Name
```csharp
public string Name { get; set; } 
```
## DrawOrder
```csharp
public virtual int DrawOrder { get; set; } 
```
## Visible
```csharp
public virtual bool Visible { get; set; } 
```
## Layer[Claw.Vector2 position]
```csharp
public int Layer[Claw.Vector2 position] { get; set; } 
```
Retorna/muda um tile da layer.<br />
## Layer[int x, int y]
```csharp
public int Layer[int x, int y] { get; set; } 
```
Retorna/muda um tile da layer.<br />
## DrawOrderChanged
```csharp
public event System.EventHandler<System.EventArgs> DrawOrderChanged;
```
## VisibleChanged
```csharp
public event System.EventHandler<System.EventArgs> VisibleChanged;
```
## Initialize
```csharp
public virtual void Initialize() { }
```
## GetData
```csharp
public int[] GetData() { }
```
Retorna todos os tiles da layer.<br />
## SetMultipleTiles
```csharp
public void SetMultipleTiles(string[] map) { }
```
Muda vários tiles de uma layer. Esse método não chama o [Tilemap.OnTileChange](/API/Claw/Tilemap.md#OnTileChange) !<br />
**map**: Sequência de tiles (["0,1,2,0,0,1", "0,1,1,3,0,1"]). Sem espaço.<br />
## SetMultipleTiles
```csharp
public void SetMultipleTiles(int[] mapData) { }
```
Muda vários tiles de uma layer. Esse método não chama o [Tilemap.OnTileChange](/API/Claw/Tilemap.md#OnTileChange) !<br />
## SetChunkTiles
```csharp
public void SetChunkTiles(Claw.Vector2 chunk, string[] chunkTiles) { }
```
Muda vários tiles de um chunk imaginário. Esse método não chama o [Tilemap.OnTileChange](/API/Claw/Tilemap.md#OnTileChange) !<br />
**chunkTiles**: Sequência de tiles (["0,1,2,0,0,1", "0,1,1,3,0,1"]). Sem espaço.<br />
## SetChunkTiles
```csharp
public void SetChunkTiles(Claw.Rectangle chunk, int[] chunkData) { }
```
Muda vários tiles de um chunk imaginário. Esse método não chama o [Tilemap.OnTileChange](/API/Claw/Tilemap.md#OnTileChange) !<br />
## Clear
```csharp
public void Clear() { }
```
Limpa a layer.<br />
## CheckCollision
```csharp
public bool CheckCollision(Claw.Vector2 position, out int tile) { }
```
## CheckCollision
```csharp
public bool CheckCollision(Claw.Vector2 position, int[] filterTiles, out int tile) { }
```
## Raycast
```csharp
public bool Raycast(Claw.Line ray, float maxDistance, out int tile, out Vector2? hitPoint, out Claw.Vector2 tileIndex) { }
```
## Pathfind
```csharp
public Claw.Vector2[] Pathfind(Claw.Vector2 start, Claw.Vector2 end, bool diagonalMovement) { }
```
Implementa o algoritmo A* para encontrar um caminho entre duas posições.<br />
**diagonalMovement**: Define se o pathfind terá movimentos na diagonal.<br />
**Retorna**: Lista de indexes do mapa.<br />
## Render
```csharp
public virtual void Render() { }
```
