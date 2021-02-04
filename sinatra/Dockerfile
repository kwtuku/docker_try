# ベースのイメージを指定
FROM ruby:2.7

# 行う作業
WORKDIR /var/www

COPY ./src /var/www


# Docker起動時に行うコマンド
# CMD [ "/bin/bash" ]


# bashに入力して実行していたことをここに書いても実行できる
RUN bundle config --local set path 'vendor/bundle' \
  && bundle install

CMD [ "bundle", "exec", "ruby", "app.rb" ]
