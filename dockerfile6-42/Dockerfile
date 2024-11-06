# 開発環境用
# Common
FROM ubuntu:20.04 AS base
# Common
RUN apt update
# Common
CMD ["sh", "-c", "echo My name is $my_name"]


# Dev-> TEST, Prod-> Bob
# 開発環境用
FROM base AS development
ENV my_name="TEST"    

# 本番環境用
FROM base AS production
ENV my_name="Bob"