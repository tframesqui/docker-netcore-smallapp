FROM microsoft/aspnetcore-build:1.1.2-jessie

COPY ./VoteApp /app
WORKDIR /app
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]

EXPOSE 88/tcp
ENTRYPOINT dotnet run --port 88