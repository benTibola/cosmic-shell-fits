# cosmic-shell-fits
### What’s inside?

| File | Purpose |
|------|---------|
| `kanku_pub.py` | Re‑fits Pantheon + SNe and DESI Ly‑α BAO with the decaying‑shell model. |
| `cosmic_shell_fit_summary_full.csv` | Output of `kanku_pub.py` (χ², dof, etc.). |
| `table_cosmic_shell_fit_body.tex` | LaTeX source for Table 1 in the manuscript. |
| `forecast_cosmic_shell.py` | Forecasts BAO significance to *z* ≈ 6 (DESI‑final + SKA). |
| `forecast_shell_offsets.{csv,png}` | CSV + figure from the forecast script. |
| `tau_sweep.{csv,png}` | χ²/dof as a function of shell half‑life |

### Quick reproduce

```bash
# clone and enter
git clone https://github.com/bentibola/cosmic-shell-fits.git
cd cosmic-shell-fits

# install deps
pip install -r requirements.txt

# fit Pantheon+ & DESI
python kanku_pub.py --sn Pantheon+SH0ES.dat

# generate BAO forecasts
python forecast_cosmic_shell.py
```
