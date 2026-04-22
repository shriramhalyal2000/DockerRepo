FROM nginx:alpine AS builder
WORKDIR /src
COPY . .


FROM nginx:alpine
COPY --from=builder /src /usr/share/nginx/html

EXPOSE 80