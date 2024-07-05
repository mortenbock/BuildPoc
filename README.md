This is a sample repo demonstrating an issue with `Directory.Build.props`

When running this command:

```
dotnet build .\BuildPoc.sln -c MyConfig
```

Then no `.pdb` files are produced, as instructed in the `Directory.Build.props` file.


However, when building the project directly:

```
dotnet build .\src\MyProject\MyProject.csproj -c MyConfig
```

Then the `.pdb` files are created.

I do no understand why there is a difference?