# Elixir Reference Implementation of UCB

This is a reference implementation of the **Universal Connect Bridge (UCB)** as defined in the accompanying research paper.

## Architecture

- Full UCB concentric security model implemented in Elixir
- Hyper-dimensional Computing (Vector Symbolic Architecture) core
- Reversible `Extend-Write` primitive with diff records
- Real LLM integration with **Claude Sonnet 4.6** via OpenRouter using strict structured outputs

## Why Elixir ?

Elixir’s process model, immutability and supervision trees are an excellent fit for the sovereign, isolated and reversible nature of the UCB core.

## Quick Start

```bash
cd elixir
mix deps.get

# Add your OpenRouter key
echo "OPENROUTER_API_KEY=sk-or-..." > .env
source .env

iex -S mix
UCBExample.run()
