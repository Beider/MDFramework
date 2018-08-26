# MDFramework
A multiplayer C# game framework for Godot 3 dependent on GDNet (https://github.com/PerduGames/gdnet3)

# Installation
1. Clone the repo to your Godot project's directory.

2. Add the MDFramework files to your `Project.csproj`, inside of `<ItemGroup>`, making sure the path matches where you cloned the repo. 

```xml
<Compile Include="src\MDFramework\MDHelpers\MDArguments.cs" />
<Compile Include="src\MDFramework\MDGameInstance.cs" />
<Compile Include="src\MDFramework\MDGameMode.cs" />
<Compile Include="src\MDFramework\MDGameSession.cs" />
<Compile Include="src\MDFramework\MDNetEntity.cs" />
<Compile Include="src\MDFramework\MDNode.cs" />
<Compile Include="src\MDFramework\MDPlayer.cs" />
```

3. Setup your `project.godot` to AutoLoad either `MDGameInstance` or your subclass of it.

```ini
[autoload]
MDGameInstance="*res://src/MDFramework/MDGameInstance.cs"
```
