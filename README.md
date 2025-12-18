# Quantum Crypto Options Research Report

## Overview

This repository contains a comprehensive research report on applying **quantum computing techniques to cryptocurrency options pricing**. The study analyzes advanced volatility models and quantum algorithms for financial derivative valuation in the crypto markets.

## Key Research Areas

- **Classical Models**: Black-Scholes, Heston, SABR, Jump Diffusion
- **Quantum Approaches**: Quantum Amplitude Estimation (QAE), Quantum Heston Implementation
- **Market Data**: Real options data from OKX and Deribit exchanges
- **Use Case**: BTC options pricing across multiple expiration dates

## Research Highlights

### Model Comparison
Comprehensive analysis of 5 pricing models tested on BTC options:
- **Black-Scholes**: Baseline reference model
- **Heston**: Stochastic volatility model, improves with time to expiry (6.5% → 4.5% MAPE)
- **SABR**: Stochastic alpha-beta-rho model for smile dynamics
- **Jump Diffusion**: Captures large price movements, 100-1,200% premium vs BS depending on expiry
- **Quantum Heston**: 65x simulated speedup (requires fault-tolerant quantum hardware, 5-10 year timeline)

### Market Validation
- Validated jump diffusion premiums against real market data from Deribit (11-day) and OKX (17-day)
- Shorter-dated options exhibit higher jump premiums
- All findings backed by live exchange data

## Technology Stack

- **Quantum Framework**: IBM Qiskit, Quantum Amplitude Estimation (QAE)
- **Classical Pricing**: NumPy, SciPy for stochastic modeling
- **Data Sources**: OKX API, Deribit API for real-time options data
- **Analysis**: Python-based backtesting and statistical validation

## Quantum Computing Implications

The research demonstrates:
1. **Theoretical Speedup**: QAE provides √N quadratic speedup vs Monte Carlo methods
2. **Current Limitations**: 6+ qubits required for practical pricing in simulations
3. **Timeline to Production**: Fault-tolerant quantum computers (1000+ logical qubits) needed in 5-10 years
4. **Near-term Use**: NISQ algorithms (Variational Quantum Eigensolver) for calibration optimization

## Key Findings

✅ **Real Market Data Validation**: Jump diffusion premiums confirmed across multiple exchanges
✅ **Model Performance Metrics**: Heston volatility smile captured accurately for BTC options
✅ **Quantum Feasibility**: Theoretical framework established for quantum pricing algorithms
✅ **Risk Analysis**: Clear documentation of model limitations and practical constraints

## Report Contents

The full research report includes:
- Detailed mathematical frameworks for each pricing model
- Quantum algorithm implementations and performance analysis
- Real market data validation with OKX and Deribit
- Comparative performance metrics and error analysis
- Recommendations for implementation roadmap
- Timeline analysis for quantum advantage in production systems

## Created

November 10, 2025

## License

This research is provided as-is for educational and research purposes.

---

**For questions about this research**, please refer to the comprehensive report PDF included in this repository.
