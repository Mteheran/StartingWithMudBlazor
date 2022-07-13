# StartingWithMudBlazor
A started tutorial to crear an application using Blazor WebAssembly and MudBlazor

### Steps to intall mud blazor

- dotnet add package MudBlazor
- add import: @using MudBlazor
- Add font and style references:
<link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap" rel="stylesheet" />
<link href="_content/MudBlazor/MudBlazor.min.css" rel="stylesheet" />

- Add Script:
<script src="_content/MudBlazor/MudBlazor.min.js"></script>

- add the service in the Program.cs class

```csharp
using MudBlazor.Services;

builder.Services.AddMudServices();
```

- in MainLayout.razor add the following components:
<MudThemeProvider/>
<MudDialogProvider/>
<MudSnackbarProvider/>

- Navigate to Counter.razor and use the button component to test the library:
<MudButton Variant="Variant.Filled" Color="Color.Primary" OnClick="IncrementCount">Click Me</MudButton>
