# 🐍 Learn Python Series

Welcome to the **Learn Python** repository! This repository contains a structured collection of interactive Jupyter & Google Colab notebooks covering Python concepts from basic fundamentals to advanced async architecture, data structures, and system design patterns.

---

## 📌 Repository Contents

| # | Topic / Module | Description | Google Colab |
| :--- | :--- | :--- | :---: |
| **01** | **[Asyncio & Concurrency Mastery](./01_asyncio_mastery.ipynb)** | Deep dive into synchronous execution, blocking I/O, Event Loop architecture, 7 async design patterns, and performance benchmarks. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rohit-Saini-Sfdc/learn-python/blob/main/01_asyncio_mastery.ipynb) |
| **02** | **[Python HTTPX Mastery](./02_httpx_mastery.ipynb)** | Complete guide to modern HTTP requests: sync (`httpx.Client`) & async (`httpx.AsyncClient`), HTTP/2, streaming, timeouts, error handling, and `MockTransport` testing. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rohit-Saini-Sfdc/learn-python/blob/main/02_httpx_mastery.ipynb) |

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

## 🎯 What's Covered in Notebook 02 (`02_httpx_mastery.ipynb`)

1. **Why HTTPX?**: Comparison matrix (`httpx` vs. `requests` vs. `aiohttp`), dual sync/async APIs, and default 5s timeouts.
2. **Basic HTTP Operations**: Synchronous GET, POST, PUT, DELETE requests, JSON payloads, headers, query params, and `httpx.Response` methods.
3. **Connection Persistence (`httpx.Client`)**: Reusing connection pools, setting base URLs, default headers, and Keep-Alive optimization.
4. **Asynchronous Client (`httpx.AsyncClient`)**: Writing `async`/`await` HTTP code, parallel fetching with `asyncio.gather()`, and speedup benchmarks.
5. **Response Streaming**: Handling large files/datasets without memory overhead using `iter_bytes()`, `iter_lines()`, and `aiter_bytes()`.
6. **Advanced Features**: Fine-grained timeouts (`httpx.Timeout`), HTTP/2 multiplexing (`http2=True`), authentication flows, and redirects.
7. **Resilient Error Handling & Testing**: Catching `httpx.HTTPError`, `httpx.HTTPStatusError`, `raise_for_status()`, event hooks, and network-free unit testing with `httpx.MockTransport`.

---

## 📄 License
MIT License. Free for learning, sharing, and contributions!
