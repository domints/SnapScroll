#FROM node:20.12.0-alpine3.19
FROM gcr.io/distroless/nodejs20-debian12
ARG PORT=3000
ENV PORT=$PORT
ENV NODE_ENV=production

WORKDIR /src

COPY ./.output /src/.output
# Optional, only needed if you rely on unbundled dependencies
# COPY ./node_modules /srcś/node_modules

EXPOSE $PORT/tcp
CMD [ ".output/server/index.mjs" ]