FROM alpine:latest
RUN apk add --update --no-cache ca-certificates

EXPOSE 14270
EXPOSE 14271
COPY ingester-linux /go/bin/
ENTRYPOINT ["/go/bin/ingester-linux"]
