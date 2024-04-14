FROM oven/bun

WORKDIR /app

COPY . .

RUN ls -lach

RUN bun install

# Set environment variables

EXPOSE 3000

CMD [ "bun", "run" ]