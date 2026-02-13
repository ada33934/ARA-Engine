# Alberta Revenue Analytics (ARA) Engine

A quantitative framework designed to identify valuation asymmetries within the Alberta electricity market during the structural transition from fossil fuels to renewable generation.

## Investment Thesis
The Alberta power grid is currently undergoing an accelerated transition, characterized by the 2026 TIER carbon price freeze and the integration of large-scale renewable assets. This transition creates significant "Capture Price" discrepancies and margin expansion opportunities that are often mispriced by traditional equity research. The ARA-Engine quantifies these gaps through real-time asset-level data integration.

## Technical Architecture
- **Automated Asset Discovery**: Dynamic mapping of TSX-listed tickers (e.g., CPX.TO, TA.TO) to physical AESO generation units.
- **Revenue Modeling**: Real-time cash flow estimation utilizing pool price volatility and Total Net Generation (TNG).
- **Transition Alpha**: Differentiated valuation of legacy "Baseload" gas assets versus "Capture-driven" wind and solar assets.

## Project Structure
- **core/**: Principal logic for market discovery and valuation engines.
- **data/**: Relational mapping between market participants and physical assets.
- **tests/**: Connectivity verification and data integrity protocols.

## Deployment
1. Initialize virtual environment: `python -m venv aeo_env`
2. Install dependencies: `pip install -r requirements.txt`
3. Configure environment variables in `.env` (refer to .env.example).

Disclaimer: Market data is sourced via the AESO API Gateway. This project is for analytical and educational purposes only. The author is not responsible for the accuracy of third-party data or any financial decisions made based on this software.
