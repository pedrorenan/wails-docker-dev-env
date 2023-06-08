FROM mcr.microsoft.com/devcontainers/go:0-1.20-bullseye

RUN apt update && apt install npm \
    build-essential libgtk-3-dev \
    libwebkit2gtk-4.0-dev -y
RUN npm install npm@latest -g && \
    npm install n -g && \
    n latest

USER vscode
RUN go install github.com/wailsapp/wails/v2/cmd/wails@latest