# dune-sim-galaxy-liquidity

# Urbit Galaxy Liquidity – Dune Sim Demo

Small proof-of-concept for Dune’s Solutions Architect application.

## Goal
Show that Urbit **galaxy** owners are (or aren’t) liquid by summing the USD
value of every token they hold across 60+ EVM chains (via Sim APIs).

## Quick-start

```bash
git clone https://github.com/<you>/urbit-galaxy-liquidity.git
cd urbit-galaxy-liquidity
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

export SIM_API_KEY=sk_...   # from https://sim.dune.com/dashboard
python fetch_liquidity.py addresses_sample.txt
cat liquidity.csv
