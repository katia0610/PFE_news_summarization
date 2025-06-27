# Étape 1 : build
FROM node:20 AS builder

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# Injecter la variable d'env au build React
ARG REACT_APP_BACKEND_HOST
ENV REACT_APP_BACKEND_HOST=$REACT_APP_BACKEND_HOST

RUN REACT_APP_BACKEND_HOST=$REACT_APP_BACKEND_HOST npm run build

# Étape 2 : serveur statique
FROM node:20

WORKDIR /app

RUN npm install -g serve

COPY --from=builder /app/build ./build

EXPOSE 3000

CMD ["serve", "-s", "build", "-l", "3000"]