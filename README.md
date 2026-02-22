# Emax PD Model – Concentration‑Effect Visualisation (MATLAB)

This script demonstrates a simple Emax pharmacodynamic (PD) model. Given a pre‑computed concentration‑time profile (`Cp`), it calculates the corresponding drug 
effect using a direct Emax model and generates multiple plots to visualise the relationship between concentration, time, and effect.

## What I Built

- **PD model**: Direct Emax model without sigmoidicity (n=1)  
  `E = (Emax * Cp) / (EC50 + Cp)`
- **Visualisation**:
  1. **Three separate subplots** (in one figure):
     - Concentration vs. time
     - Effect vs. time
     - Effect vs. concentration (direct relationship)
  2. **Combined dual‑axis plot** (in a second figure):
     - Concentration on left y‑axis, effect on right y‑axis, both vs. time
- The code assumes `Cp` and `t` are already defined (e.g., from a prior PK simulation).
<img width="456" height="275" alt="image" src="https://github.com/user-attachments/assets/0f7cdf1c-3944-44eb-910a-8e4790d2c8e0" />
<img width="456" height="275" alt="image" src="https://github.com/user-attachments/assets/3e159e74-1f20-489f-b303-d152ddcf8511" />



## Skills Demonstrated

- MATLAB programming (scripting, vectorised operations)
- Pharmacodynamic modelling (Emax model)
- Data visualisation (subplots, `yyaxis`, multiple line styles, labels, grids)
- Clear presentation of concentration‑effect relationships

## How to Run

1. Ensure you have a concentration vector `Cp` and corresponding time vector `t` in your workspace (e.g., from running a PK simulation script).
2. Append this script to your existing PK code, or run it separately after defining `Cp` and `t`.
3. Modify the Emax parameters (`Emax`, `EC50`) as desired.
4. Execute the script to generate two figures.

**Note**: The script is self‑contained except for the prerequisite `Cp` and `t`. It is designed to be added to the end of any PK simulation that produces a concentration‑time profile.

## Files

- `Emax_PD_Visualisation.m` – the script containing the Emax calculation and plotting.
