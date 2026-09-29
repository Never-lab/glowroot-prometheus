# glowroot-prometheus

Export delle metriche Glowroot in formato Prometheus (`/metrics`), fuori dal monorepo upstream.

Tracker upstream: [glowroot/glowroot#1249](https://github.com/glowroot/glowroot/issues/1249) (anche #1099 / #952).

## Perché un repo a parte

Le PR su `glowroot/glowroot` sono già tante. Qui si prototipa l’exporter senza bloccare il merge queue: quando c’è qualcosa di solido, si propone upstream o si documenta come sidecar.

## Scope (bozza)

- **v0:** scrape endpoint OpenMetrics/Prometheus (pull)
- Serie minime: throughput / error rate / latency (aggregati) e/o gauge JVM già noti a Glowroot
- Target: agent embedded e/o Central — da decidere al primo spike
- Fuori scope v0: dual instrumentation OTel, StatsD push

## Stato

Scaffold vuoto. Nessun codice ancora.

## Licenza

Apache-2.0 (allineata a Glowroot).
