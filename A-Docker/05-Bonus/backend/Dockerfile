FROM mcr.microsoft.com/dotnet/sdk:9.0-alpine AS build


# TODO: add the Docker commands to do these build steps:

WORKDIR '/src'
COPY backend.csproj .
RUN dotnet restore 
COPY . .
RUN dotnet build -c Release 
RUN dotnet publish -c Release -o /app

FROM mcr.microsoft.com/dotnet/aspnet:9.0-alpine

ENV ASPNETCORE_URLS=http://+:5000
EXPOSE 5000

# TODO: add the Docker commands to do these image build and container run steps:

WORKDIR '/app'
# copy the content from the app folder on the build stage above
COPY --from=build /app .

# as the container starts:
# `dotnet backend.dll`
CMD ["dotnet", "backend.dll"]
