# Logistics network: three dashboards, three decisions

One French logistics network (3 existing warehouses: Paris, Lyon, Lille; 20 real French cities), and three dashboards built for three different people who make three different decisions from the same data.

**Live dashboards:** https://jaures-business-intelligence.github.io/logistics-dashboards/

| Page | Who | Decision | Charts |
|---|---|---|---|
| `co2.html` | Sustainability manager | Which routes to prioritize to cut CO2, and which warehouse is the least efficient per tonne | ranked bar chart, bar chart with a reference line, scatter over a France outline |
| `cost.html` | Operations manager | For each warehouse, is the problem transport or storage? | stacked bar chart, table of exact figures |
| `network.html` | Strategy manager | Open Bordeaux or Marseille, or close Lille? | bar chart of scenarios, two side-by-side maps |

## How it works

1. `data/cities.csv` has the 20 cities, their coordinates and population.
2. `scripts/compute_kpis.py` assigns each city to its nearest warehouse (straight-line distance) and computes the three sets of KPIs. It writes `docs/data/co2.json`, `cost.json` and `network.json`.
3. The three HTML pages in `docs/` read these JSON files and draw the charts with Chart.js. `docs/js/france-map-background.js` draws a simplified outline of France behind the maps.
4. `.github/workflows/compute.yml` recomputes everything on demand (manual run) and commits the results.

## Assumptions (please read)

- **Demand is a population proxy**: 50 tonnes per year per 1,000 residents. It is not real shipment data.
- **CO2 factor**: 0.10 kg CO2e per tonne-km. It is inside a published range for road freight (about 0.047 to 0.12), but it should be checked against ADEME's current Base Empreinte before professional use.
- **Costs** (0.12 EUR per tonne-km for transport, 40 EUR per tonne per year for storage) are illustrative and not sourced.
- Distances are straight-line, not by road. Population figures are approximate.
- The network analysis only uses distance. It does not include the cost of building a warehouse, lease exit costs, or non-distance factors (for example Lille's position near Belgium and the UK).

## Main results (baseline network)

- Total CO2: about 6,236 t per year (16.8 kg per tonne on average). Lyon is the least efficient (24.34 kg per tonne), Paris 9.09, Lille 0 (it only serves its own city).
- Lyon has the highest cost per tonne (69.21 EUR); its extra cost comes from transport.
- Average distance (population-weighted): baseline 168.04 km, with Marseille 115.03 km, with Bordeaux 139.89 km, closing Lille 174.43 km.

## Files

| File | Role |
|---|---|
| `data/cities.csv` | input data |
| `scripts/compute_kpis.py` | KPI computation |
| `docs/index.html`, `co2.html`, `cost.html`, `network.html` | dashboards (GitHub Pages) |
| `docs/js/france-map-background.js` | shared map background |
| `docs/data/*.json` | generated results |
| `.github/workflows/compute.yml` | recompute workflow |
| `REFLECTIONS.md` | answers to the 7 reflection questions |

## Run it yourself

```bash
python scripts/compute_kpis.py
cd docs && python -m http.server
```
