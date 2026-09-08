# 🐍 Learn Python Series

Welcome to the **Learn Python** repository! This repository contains a structured collection of interactive Jupyter & Google Colab notebooks covering Python concepts from basic fundamentals to advanced async architecture, data structures, and system design patterns.

---

## 📌 Repository Contents

| # | Topic / Module | Description | Google Colab |
| :--- | :--- | :--- | :---: |
| **01** | **[Asyncio & Concurrency Mastery](./01_asyncio_mastery.ipynb)** | Deep dive into synchronous execution, blocking I/O, Event Loop architecture, 7 async design patterns, and performance benchmarks. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rohit-Saini-Sfdc/learn-python/blob/main/01_asyncio_mastery.ipynb) |

---

## 🚀 How to Use These Notebooks

### 1. Run in Google Colab (Recommended)
Click the **"Open in Colab"** badge on any notebook to open and execute it directly in Google Colab without any local setup.

### 2. Run Locally
Clone the repository and launch Jupyter Notebook or VS Code:

```bash
git clone https://github.com/Rohit-Saini-Sfdc/learn-python.git
cd learn-python
jupyter notebook
```

---

## 🎯 What's Covered in Notebook 01 (`01_asyncio_mastery.ipynb`)

1. **Synchronous Execution Model**: Sequential single-threaded execution and CPU idle time during blocking I/O.
2. **Asyncio Core Architecture**: Event loop, Coroutines (`async def`), Tasks, and Futures.
3. **Key Benefits**: Scalability ($O(1)$ max wait time), low memory footprint (~KB per task), and safe cooperative multitasking.
4. **7 Essential Async Patterns**:
   - `asyncio.gather()` — Concurrent execution
   - `asyncio.as_completed()` — Processing stream as tasks complete
   - `asyncio.wait_for()` — Timeouts and task cancellation
   - `async for` & `async yield` — Asynchronous iterators and streams
   - `async with` — Asynchronous context managers
   - `asyncio.Queue` — Producer-consumer worker queues
   - `asyncio.to_thread()` — Running blocking synchronous code off-thread
5. **Sync vs. Async Benchmark**: Empirical speedup demonstration (~10x faster for I/O operations).

---

## 📄 License
MIT License. Free for learning, sharing, and contributions!
