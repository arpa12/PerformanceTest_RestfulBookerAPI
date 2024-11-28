# PerformanceTest_RestfulBookerAPI

This repository contains performance test results for the **Restful Booker API**, a commonly used API for managing bookings. The tests were performed to evaluate the API's scalability, response time, and its ability to handle a range of concurrent requests. The repository also includes detailed test reports and performance data.

## Table of Contents

- [Test Overview](#test-overview)
- [Test Results](#test-results)
- [Test Configuration](#test-configuration)

## Test Overview

The performance tests were designed to evaluate the **Restful Booker API** under various load conditions. The tests involve sending multiple concurrent requests with a loop count of 1 and measuring the average transactions per second (TPS) and the total number of concurrent API requests handled.

The tests were executed on a server with the IP address `000.000.000.00`.

## Test Results

### Summary of Test Results

| Concurrent Requests | Total Concurrent API Requests | Avg TPS (Transactions Per Second) |
|---------------------|-------------------------------|-----------------------------------|
| 150                 | 600                           | ~10                               |
| 160                 | 640                           | ~11                               |
| 180                 | 720                           | ~12                               |
| 195                 | 780                           | ~13                               |
| 199                 | 796                           | ~13.267                           |
| 200                 | 800                           | ~13.333                           |
| 300                 | 1200                          | ~20                               |
| 1000                | 4000                          | ~66                               |
| 2000                | 8000                          | ~133                              |

### Observations:
- As the number of concurrent requests increased, the system was able to handle more API requests with a steady increase in throughput.
- The performance showed good scalability up to 2000 concurrent requests, with a substantial rise in TPS as the load increased.
- For extremely high loads (e.g., 2000+ concurrent requests), the system's performance remained stable, but further optimizations could be needed for larger-scale testing.

## Test Configuration

- **Test Server:** IP Address - `000.000.000.00`
- **API Tested:** Restful Booker API
- **Test Method:** Load testing with increasing concurrent requests
- **Loop Count:** 1 per request (requests executed once per loop)
- **Performance Metric:** Average Transactions Per Second (TPS)
- **Test Environment:** All tests executed in a controlled server environment.


