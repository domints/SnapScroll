FROM node:20.12.0-alpine3.19
ARG PORT=3000
ENV PORT=$PORT
ENV NODE_ENV=production

WORKDIR /src

COPY ./.output /src/.output
# Optional, only needed if you rely on unbundled dependencies
# COPY ./node_modules /srcś/node_modules

EXPOSE $PORT/tcp
CMD [ "node", ".output/server/index.mjs" ]