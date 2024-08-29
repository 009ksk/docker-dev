# ベースイメージとしてDebian Bookworm Slimを使用
FROM debian:bookworm-slim

# パッケージリストを更新し、必要なパッケージをインストール
RUN apt-get update && \
    apt-get install -y g++ make cmake && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# 作業ディレクトリを設定
WORKDIR /app