FROM microsoft/dotnet

WORKDIR /app
COPY backend.csproj .
RUN dotnet restore

COPY . /app
RUN dotnet build

ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000
CMD ["dotnet", "run"]

# Read more: https://jeremylindsayni.wordpress.com/2016/11/22/deploying-a-net-core-1-1-web-api-microservice-to-a-docker-container-in-windows/
