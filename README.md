# Hospital Ward Flow Simulation (Simio)

Discrete-event simulation of patient flow through a hospital’s acute wards and ICU, built in **Simio**.  
The project models time-varying arrivals, fitted service-time distributions, and patient routing logic to evaluate congestion and operational policies.

## What this project does
- **Input modeling:** estimates arrival patterns by hour/day and fits service-time distributions for acute wards and ICU using Excel + R.
- **Base model:** simulates patient flow across multiple acute wards and ICU with capacity constraints, waiting, and diversion outcomes.
- **Scenario analysis:** compares alternative operating policies (e.g., ward structure changes and diversion rules).
- **Policy recommendation:** identifies a diversion threshold policy that reduces congestion and blocked beds (see report).

## Repository contents
- `report/` – Final write-up with modeling assumptions, experiments, and results.
- `simio/` – Simio project files (model + experiments).
- `data/` – Input data used by the model (arrivals + service time datasets).
- `analysis/` – R scripts used for distribution fitting / parameter estimation (if included).
- `images/` – Screenshots of the model + key outputs for easy viewing.

## How to run (Simio)
1. Open the Simio project file in `simio/`.
2. Confirm file paths to any external data tables in `data/` (if your Simio file uses linked tables).
3. Run the experiments (base model + scenarios) from within Simio.

## Notes
- This repo is primarily intended as a **portfolio artifact**. If you don’t have Simio, you can still read the full methodology and results in the PDF report.
