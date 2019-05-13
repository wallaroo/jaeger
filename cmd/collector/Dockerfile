FROM alpine
RUN apk add --update --no-cache ca-certificates

EXPOSE 14267
EXPOSE 14250
COPY collector-linux /go/bin/
ENTRYPOINT ["/go/bin/collector-linux"]
