# Tilemap
```csharp
public sealed class Tilemap
```
Realiza a rendrização e a organização de um tilemap ortogonal.<br />
## Tilemap
```csharp
public Tilemap() { }
```
## Tilemap
```csharp
public Tilemap(Claw.Vector2 size, Claw.Vector2 gridSize) { }
```
## GridSize
```csharp
public Claw.Vector2 GridSize;
```
## OnTileChange
```csharp
public System.Action<int,string,Claw.Vector2> OnTileChange;
```
É executado quando um tile é mudado ([novo tile], [nome da layer], [posição do tile]).<br />
## OutOfView
```csharp
public static int OutOfView;
```
Define quantos tiles fora da view serão desenhados (1 por padrão).<br />
## LayerCount
```csharp
public int LayerCount { get; } 
```
## Size
```csharp
public Claw.Vector2 Size { get; set; } 
```
## Tilemap[int layerIndex]
```csharp
public Claw.Layer Tilemap[int layerIndex] { get; } 
```
Retorna uma layer.<br />
## Tilemap[string layerName]
```csharp
public Claw.Layer Tilemap[string layerName] { get; } 
```
Retorna uma layer.<br />
## GetTileIndex
```csharp
public int GetTileIndex(int palette, Claw.Vector2 index) { }
```
Transforma um index 2D em um index 1D.<br />
## AddPalette
```csharp
public void AddPalette(Claw.Graphics.Sprite palette, int margin, int spacing) { }
```
Adiciona uma paleta ao [Tilemap](/API/Claw/Tilemap#Tilemap) .<br />
## AddLayer
```csharp
public int AddLayer(int drawOrder, string name, float priority, float opacity, Claw.Color color) { }
```
Adiciona uma layer nova.<br />
## AddLayer
```csharp
public int AddLayer(int drawOrder, string name, bool visible, float priority, float opacity, Claw.Color color, int[] data) { }
```
Adiciona uma layer nova e já insere os tiles dela.<br />
## Addlayer
```csharp
public int Addlayer(Claw.Layer layer) { }
```
Adiciona uma layer.<br />
## RemoveLayer
```csharp
public void RemoveLayer(int index) { }
```
Remove uma layer.<br />
## RemoveLayer
```csharp
public void RemoveLayer(string name) { }
```
Remove uma layer.<br />
## LayerExists
```csharp
public bool LayerExists(int index) { }
```
Verifica se a layer existe.<br />
## LayerExists
```csharp
public bool LayerExists(string name) { }
```
Verifica se a layer existe.<br />
