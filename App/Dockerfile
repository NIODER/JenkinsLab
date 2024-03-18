FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build
WORKDIR /App
COPY . .
RUN dotnet restore
ENTRYPOINT [ "dotnet", "publish", "-o", "build" ]