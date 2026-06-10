# Derivatives Toolkit

**A practical introduction to derivatives pricing and risk -- from someone who has been doing it on a trading desk for 17 years.**

This is not another textbook port. Every notebook in this repo reflects how these concepts actually work when there is real money on the line. The theory is standard (Hull, Wilmott, Gatheral), but the intuition comes from watching these models succeed and fail in live markets since 2009.

10 modules. Each one is a self-contained Jupyter notebook. Start anywhere.

## Modules

| # | Notebook | What it covers |
|---|----------|---------------|
| 01 | [Black-Scholes from Scratch](notebooks/01_black_scholes.ipynb) | BSM formula, put-call parity, payoff diagrams |
| 02 | [Greeks Intuition](notebooks/02_greeks.ipynb) | Delta, gamma, theta, vega -- how they actually move |
| 03 | [FX Options -- Garman-Kohlhagen](notebooks/03_fx_options.ipynb) | Adapting BSM for currency pairs, forward points |
| 04 | [Implied Volatility & Smile](notebooks/04_implied_vol.ipynb) | Newton-Raphson IV solver, smile plotting, skew |
| 05 | [Volatility Surface](notebooks/05_vol_surface.ipynb) | SVI calibration, strike/expiry interpolation, 3D surface |
| 06 | [Monte Carlo Pricing](notebooks/06_monte_carlo.ipynb) | GBM simulation, vanillas, barriers, convergence |
| 07 | [Gamma Exposure (GEX)](notebooks/07_gex.ipynb) | Dealer gamma from open interest -- the public formula |
| 08 | [Exotic Payoffs](notebooks/08_exotics.ipynb) | Barriers, digitals, lookbacks -- payoff diagrams |
| 09 | [Heston Model](notebooks/09_heston.ipynb) | Stochastic vol basics, calibration, BSM comparison |
| 10 | [Risk Metrics](notebooks/10_risk_metrics.ipynb) | Historical VaR, stress testing, correlation |

## Requirements

```bash
pip install numpy scipy matplotlib pandas jupyter
```

No proprietary data needed. Every notebook runs with synthetic or freely available data.

## Who is this for

- Finance students who want to see how the formulas connect to real trading
- Junior quants building intuition before touching production code
- Self-taught traders who want to understand what their platform is actually computing
- Anyone preparing for interviews at derivatives desks

## Who is this NOT for

This is educational code. It is not production-grade. It does not connect to brokers. It does not execute trades. If you are looking for a professional-grade derivatives analytics platform, that is a different product entirely.

## Further reading

These notebooks cover the foundations. For deeper analysis on specific topics:

- **Options microstructure & dealer positioning** -- [Beyond Gamma Exposure](https://www.amazon.com/dp/B0H2RZGMY6) | [Working paper](https://doi.org/10.5281/zenodo.20509786)
- **FX derivatives structural biases** -- [FX Traders vs Brokers](https://www.amazon.com/dp/B0H3VSV88X) | [Working paper](https://doi.org/10.5281/zenodo.20509708)
- **AI infrastructure repricing** -- [The China AI Disruption Thesis](https://www.amazon.com/dp/B0H11WH3R9) | [Working paper](https://doi.org/10.5281/zenodo.20509816)
- **Private credit systemic risk** -- [Convergent Faults](https://doi.org/10.5281/zenodo.20558733) | [The Coming Shadow Banking Crash](https://www.amazon.com/dp/B0H4HMVSMR)

## Author

**Djellal Djouad** -- CrossVol Research
- 17 years on derivatives trading desks (equity, FX, fixed income)
- [crossvol.com](https://crossvol.com)
- [ORCID 0009-0002-4911-1118](https://orcid.org/0009-0002-4911-1118)
- [@DjouadDjellal](https://x.com/DjouadDjellal)

## License

MIT with Educational Use Clause -- see [LICENSE](LICENSE). Free for learning and research. Not for commercial trading systems. See the license file for details.

---

*If you find a bug or want to suggest a module, open an issue. If you use this in a course, I would like to hear about it.*
