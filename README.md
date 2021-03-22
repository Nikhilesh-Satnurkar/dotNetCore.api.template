# dotNetCore.api.template

# Introduction 
This repo consist of .Net Core Template that can be used to create new API structure. 

# Getting Started
Folder *.\\dotNetCore.api.template* is a .Net Core template. 
*.\\dotNetCore.api.template\\.template.config\\template.json* file has details of the .Net Core template. 
*templatepack.csproj* contains details of NuGet Package.

## Steps to update template and create NuGet Package
1. Make your changes in template. Add/Remove Project in template folder.
2. Update "template.json" file if required.
3. Update NuGet package details in "templatepack.csproj"
4. Run "dotnet pack templatepack.csproj". This command will create NuGet package in bin folder.

## dotnet commands to use for Template installation and uninstallation
| Sr. No.       | Command           | Description  |
|:--- |:-------------|:-----|
| 1 | dotnet new -i *packageName* | Install .Net Core template from NuGet Packages |
| 2 | dotnet new -i *packageName.nupkg*      |   Install .Net Core template from local path |
| 3 | dotnet new -i *parent path of .template.config folder*      |    Install .Net Core template using template folder |
| 4 | dotnet new -u *packageName*      |    UnInstall .Net Core template using NuGet package name |
| 5 | dotnet new -u *parent path of .template.config folder*      |    UnInstall .Net Core template using template folder |
