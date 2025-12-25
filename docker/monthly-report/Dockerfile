FROM mcr.microsoft.com/dotnet/aspnet:9.0

RUN apt-get update && apt-get install -y \
    libdbus-1-3 \
    libnss3 \
    libxss1 \
    libasound2 \
    fonts-liberation \
    libatk1.0-0 \
    libgtk-3-0 \
    libdrm2 \
    libgbm1 \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app

ENTRYPOINT ["dotnet", "/app/MonthlyReport.Server.dll"]
