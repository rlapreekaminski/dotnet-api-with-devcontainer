# 🚀 .NET API Project with Dev Containers

This project is a **minimal .NET API** using a **DevContainer** for a ready-to-use development environment.

## 📁 Project Structure

The project structure is as follows:

```plaintext
dotnet-multiapi-containerized-devcontainer/
├── .devcontainer/            # Dev Container configuration
│   ├── devcontainer.json
│   └── Dockerfile            # Development environment configuration
├── .vscode/                  # VS Code configuration
│   ├── tasks.json
│   └── launch.json
├── dotnet-api-with-devcontainer.csproj
├── Program.cs
└── README.md                 # Documentation (you are here)
```

## ⚙️ Prerequisites

Before starting, ensure you have the following tools installed:

- **[Docker Desktop](https://www.docker.com/products/docker-desktop/)** (to run containers locally)
- **[Visual Studio Code](https://code.visualstudio.com/)** with the **Dev Containers** extension (`ms-vscode-remote.remote-containers`)
- **[.NET SDK 9.0](https://dotnet.microsoft.com/download)** only if you or a member of your team want to work outside the container

## 🚧 Getting Started

### 1. Launch Development Environment with Dev Containers

Open the project in VS Code.

Ensure the Dev Containers extension is installed.

Open the command palette (Ctrl+Shift+P or Cmd+Shift+P) and select:

```bash
Dev Containers: Reopen in Container
```

This will rebuild and launch the development environment inside a Docker container.

### 2. Build and Run the API

To run the API from your devcontainer, launch dotnet run command :

```bash
dotnet run
```

The API will be accessible at the following addresses <http://localhost:5002>

### 3. Debugging with VS Code

To debug thean API:

- Place breakpoints in your code.
- Use the pre-configured **_launch.json_** file.
- Start debugging with F5.+

## 🔗 Useful Resources

- [.NET Minimal API Documentation](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/minimal-apis/overview?view=aspnetcore-9.0)
- [Dev Containers based on Dockefile Documentation](https://code.visualstudio.com/docs/devcontainers/create-dev-container#_dockerfile)

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
