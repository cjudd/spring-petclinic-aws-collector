# Spring Petclinic AWS Distro for OpenTelemetry (ADOT)

It is an AWS Distro for OpenTelemetry (ADOT) Collector that received otel data and sending it to AWS X-RAY and Metrics.

To start:
```shell
docker-compose up -d
```

To shutdown:
```shell
docker-compose down
```

The demo forwards to the following backends:

- awsxray - X-Ray Exporter
  - https://aws-otel.github.io/docs/getting-started/x-ray
  - https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/exporter/awsxrayexporter
- awsemf - CloudWatch Embedded Metrics Format (EMF) Exporter 
  - https://aws-otel.github.io/docs/getting-started/cloudwatch-metrics
  - https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/exporter/awsemfexporter
- awscloudwatchlogs 
  - https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/exporter/awscloudwatchlogsexporter
