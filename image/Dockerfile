# --- Stage 1: Builder ---
FROM alpine:latest AS builder
WORKDIR /app

RUN cat <<EOF > hello.sh
#!/bin/sh
echo "Hello Containers"
EOF
RUN chmod +x hello.sh

# --- Stage 2: Final lightweight image ---
FROM alpine:3.18
COPY --from=builder /app/hello.sh .

CMD ["./hello.sh"]

