# Asset
```csharp
public static class Asset
```
Classe responsável pelo carregamento de assets.<br />
## RootDirectory
```csharp
public static string RootDirectory;
```
Diretório base dos assets ("Assets", por padrão).<br />
## AddReader
```csharp
public static void AddReader<T>(System.Func<string,T> reader) { }
```
Define uma função que carregará determinado tipo de asset.<br />
**T**: O tipo de asset.<br />
**reader**: A função, que recebe um arquivo e retorna um asset ou nulo.<br />
## Load
```csharp
public static T Load<T>(string assetPath) { }
```
Carrega um asset através de um arquivo.<br />
**T**: O tipo de asset.<br />
**assetPath**: Caminho relativo do arquivo, sem a extensão.<br />
