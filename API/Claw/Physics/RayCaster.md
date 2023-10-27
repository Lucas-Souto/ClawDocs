# RayCaster
```csharp
public static class RayCaster
```
Calculador de raycast.<br />
## Cast
```csharp
public static void Cast(Claw.Line ray, System.Func<Claw.Vector2,bool> onMove, out Claw.Vector2? hitPoint, Claw.Vector2 cellSize) { }
```
Realiza a movimentação do raio de um ponto ao outro.<br />
**onMove**: É executado sempre que o raio se move.<br />
Parâmetro Vector2: A posição atual do raio.<br />
Retorno bool: O resultado do seu cálculo de colisão (true para parar o raio, false para prosseguir).<br />
<br />
## Cast
```csharp
public static void Cast(Claw.Line ray, float maxDistance, System.Func<Claw.Vector2,bool> onMove, out Claw.Vector2? hitPoint, Claw.Vector2 cellSize) { }
```
Realiza a movimentação do raio de um ponto ao outro.<br />
**maxDistance**: Distância em células.<br />
**onMove**: É executado sempre que o raio se move.<br />
Parâmetro Vector2: A posição atual do raio.<br />
Retorno bool: O resultado do seu cálculo de colisão (true para parar o raio, false para prosseguir).<br />
<br />
