FROM subquerynetwork/subql-node-starknet:latest

WORKDIR /app
RUN mkdir -p /app/

COPY . /app/

RUN npm install -g pnpm

RUN pnpm install

RUN pnpm build
 
CMD ["pnpm", "test"]
