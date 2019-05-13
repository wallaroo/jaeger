FROM alpine:latest
RUN apk add --update --no-cache ca-certificates

EXPOSE 16686
COPY query-linux /go/bin/

ENTRYPOINT ["/go/bin/query-linux"]
