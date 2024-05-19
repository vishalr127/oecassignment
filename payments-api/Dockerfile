FROM mcr.microsoft.com/dotnet/sdk:7.0 AS build

WORKDIR /app

COPY payments-api.csproj ./
RUN dotnet restore

COPY . .


RUN dotnet publish -c Release -o out


FROM mcr.microsoft.com/dotnet/aspnet:7.0 AS runtime


WORKDIR /app


COPY --from=build /app/out .


EXPOSE 8081


ENTRYPOINT ["dotnet", "payments-api.dll"]

