# Architecture

```text
Households / community loads → meter/profile data → demand + renewable forecast
                                                → Neighbourhood Energy Coordinator
                                                   ├─ shared battery
                                                   ├─ smart/flexible loads
                                                   └─ grid import/export
                                                → reliability monitoring / resident notice
```

Energy flow carries solar, wind, battery and grid power. Data flow carries demand profiles, generation and SOC. Decision flow carries forecast, priorities and response actions. Money flow is an estimated avoided grid-energy cost. The current Express process holds simulation state in memory; the React client reads it through REST endpoints. MongoDB is not needed.
