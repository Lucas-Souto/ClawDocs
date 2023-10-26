# Save
```csharp
public static class Save
```
Funções prontas para lidar com um save.<br />
## Open
```csharp
public static void Open(string path, bool useCrypt) { }
```
Abre o save.<br />
## Write
```csharp
public static void Write(string section, string key, object value) { }
```
Escreve numa seção do save.<br />
## Read
```csharp
public static T Read<T>(string section, string key, T defaultValue) { }
```
Lê uma chave de uma seção do save.<br />
## Clear
```csharp
public static void Clear() { }
```
Limpa o save.<br />
## RemoveSection
```csharp
public static void RemoveSection(string section) { }
```
Remove uma seção inteira do save.<br />
## RemoveKey
```csharp
public static void RemoveKey(string section, string key) { }
```
Remove uma chave de uma seção do save.<br />
## SectionExists
```csharp
public static bool SectionExists(string section) { }
```
Verifica se a seção existe.<br />
## KeyExists
```csharp
public static bool KeyExists(string section, string key) { }
```
Verifica se a chave existe.<br />
## Close
```csharp
public static void Close() { }
```
Fecha o save.<br />
