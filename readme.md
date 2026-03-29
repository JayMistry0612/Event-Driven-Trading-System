# ⚡ Event-Driven Trading System

## Overview

A real-time simulated trading system built using an event-driven architecture. The system processes market data as a stream and reacts through a structured event pipeline.

---

## Architecture

Event Flow:

```
MARKET → SIGNAL → ORDER → PORTFOLIO
```

---

## Features

* Event-driven architecture using queue
* Decoupled components:

  * Data Handler
  * Strategy
  * Execution Engine
  * Portfolio Manager
* Real-time simulation using historical data stream
* Accurate state management and execution timing
* Full validation against backtesting engine

---

## Tech Stack

* Python
* Deque (event queue)
* Pandas, NumPy

---

## Project Structure

```
src/
  event.py
  event_queue.py
  data_handler.py
  strategy.py
  execution.py
  portfolio.py
main.py
```

---

## What I Learned

* Event-driven system design
* Separation of concerns in trading systems
* State management across time
* Debugging complex system inconsistencies
* Data flow vs control flow distinction

---

## Key Insights

* Event-driven systems require strict data flow discipline
* Small timing bugs can break entire systems
* Debugging requires trade-level validation, not just final output
* Consistency between systems is critical

---

## Challenges Faced

* Signal timing mismatch
* Execution using wrong candle
* State update ordering issues
* Numerical precision differences (// vs /)

---

## Future Improvements

* Multi-asset portfolio support
* Multi-strategy integration
* Live market data integration (WebSockets/API)
* Asynchronous event processing
