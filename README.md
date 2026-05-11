### Uruchomienie kontenerów
```bash
docker compose up -d
```

### Sprawdzenie statusu
```bash
docker compose ps
```

### Logi
```bash
docker compose logs -f auth-service
```

### Konsument Kafka
```bash
docker compose exec kafka kafka-console-consumer `
  --bootstrap-server localhost:9092 `
  --topic tourist.registered `
  --from-beginning
  ```
