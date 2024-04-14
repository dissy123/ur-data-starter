FROM node:20.1.0-alpine3.16

RUN apk add --no-cache openssh

WORKDIR /app

COPY . .

RUN corepack enable && corepack prepare pnpm@latest --activate

RUN pnpm install
RUN pnpm build

# Set environment variables
ENV HOST 0.0.0.0
EXPOSE 3000

CMD [ "node", ".output/server/index.mjs" ]