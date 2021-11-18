FROM node:16-alpine as node

ARG ENV=prod
ARG APP=ejercicio3

ENV ENV ${ENV}
ENV APP ${APP}

# Apartado i

# Apartado ii

RUN npm ci

RUN npm run build --prod

# Apartado iii

FROM nginx:1.13.8-alpine

# Apartado iv
COPY --from=  

# Apartado v
