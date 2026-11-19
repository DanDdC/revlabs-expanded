# Dados legados

`laps.json` contém metadados agregados das 15 voltas do banco antigo:

- car_code, track_id, lap_number
- lap_time_ms, setores
- velocidades, throttle, brake, RPM
- source_lap_id

**Não contém frames nem posições (`position_x/y/z`).** Portanto:

- serve para calibração de tempo e validação de modelo;
- não serve para gerar track map;
- para geometria, é necessário capturar novas voltas com o probe.
