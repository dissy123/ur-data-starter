FROM oven/bun

WORKDIR /app

COPY . .

RUN ls -lach

RUN bun install
RUN bun run build


# Set environment variables

EXPOSE 3000

CMD [ "node", ".output/server/index.mjs" ]