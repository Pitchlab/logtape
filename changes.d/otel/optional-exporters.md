 -  The gRPC and HTTP/protobuf log exporters are now optional peer
    dependencies, so a project that passes its own `loggerProvider` no longer
    installs *@grpc/grpc-js*.  To use `OTEL_EXPORTER_OTLP_PROTOCOL=grpc` or
    `http/protobuf`, install *@opentelemetry/exporter-logs-otlp-grpc* or
    *@opentelemetry/exporter-logs-otlp-proto*; a missing one is reported with
    the package name.
