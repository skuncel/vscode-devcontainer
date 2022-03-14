FROM debian:unstable-slim

RUN apt update && \
    apt install -y vim curl zsh git && \
    adduser --shell /bin/zsh vscode && \
    touch /home/vscode/.zshrc && \
    passwd --lock root

USER vscode
WORKDIR /home/vscode
CMD "/bin/zsh"