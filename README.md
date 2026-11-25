# FlowShip Config

Centralized configuration repository for the FlowShip microservices project.

## Files

- `application.yml` — shared/default configuration for all Config Client applications.
- `user-service.yml` — configuration specific to `user-service`.
- `shipment-service.yml` — configuration specific to `shipment-service`.
- `tracking-service.yml` — configuration specific to `tracking-service`.

The service-specific filenames must match each application's:

```yaml
spring:
  application:
    name: <service-name>
```

This repository is intended to be read by Spring Cloud Config Server.

> Do not commit secrets such as passwords, API keys, or private tokens to this repository.
