

FROM mcr.microsoft.com/dotnet/core/aspnet:3.1-buster-slim
FROM mcr.microsoft.com/dotnet/core/sdk:3.1-buster
WORKDIR /app
COPY /. /app
RUN dotnet restore
RUN dotnet publish -o /out -c Release
EXPOSE 5000
ENTRYPOINT ["dotnet", "/out/dockertest.dll"]
