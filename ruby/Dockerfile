# ベースイメージとして公式のRubyイメージを使用
FROM ruby:3.3-slim-bookworm

# 作業ディレクトリを設定
WORKDIR /app

# 必要なGemをインストールするためのGemfileとGemfile.lockをコピー
COPY Gemfile Gemfile.lock ./

# Bundlerをインストール
RUN gem install bundler

# 必要なGemをインストール
RUN bundle install