# Simulation methodology

The backend generates 96 quarter-hour records for a day. Demand combines an overnight base, morning and evening peaks, a small time variation and deterministic perturbation. Solar follows a daylight sine curve with scenario-specific cloud multipliers; wind is a variable profile. Each record includes actual generation, a transparent profile forecast and illustrative ±14% bounds.

Baseline serves renewable energy and bounded grid supply, without response or coordinated battery. GridFlex applies participation-scaled flexible demand reduction during net-load gaps, battery discharge subject to 30 kW and minimum SOC, renewable charging subject to 30 kW and maximum SOC, then grid support. Six scenarios alter cloud, evening demand or grid availability. Values are designed for explainable demonstration, not operational dispatch.
