# Utilise l'image officielle .NET 9 SDK
FROM mcr.microsoft.com/devcontainers/dotnet:dev-9.0   

# Configure le répertoire de travail
WORKDIR /workspace

# Installe le client Docker pour utiliser Docker depuis le conteneur
RUN apt-get update && apt-get install -y docker.io

# Installe le débogueur .NET (vsdbg)
RUN curl -sSL https://aka.ms/getvsdbgsh | bash /dev/stdin -v latest -l /vsdbg

# Nettoyage
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# Expose les ports pour .NET Minimal API (HTTP et HTTPS)
EXPOSE 5002 7002

# Définit le point d'entrée par défaut
CMD ["sleep", "infinity"]
