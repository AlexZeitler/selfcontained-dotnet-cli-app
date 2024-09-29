# selfcontained-dotnet-cli-app
Experiments with self-contained .NET CLI apps

## Publishing as self contained single file without optimizations

```bash
dotnet publish --self-contained true -p:PublishSingleFile=true -p:IncludeNativeLibrariesForSelfExtract=true
```

## Environment

Copy it to `~/bin` to make it available globally.

```bash
cp bin/Release/net8.0/linux-x64/publish/SelfContainedCliApp ~/bin/
```

Run it in `~`

Output will be:

```bash
SelfContainedCliApp
Hello, World!
Directory: /home/<your-username>
```