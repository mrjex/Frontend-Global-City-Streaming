# Global City Streaming Frontend

This repository is the **frontend submodule** of the [Global City Streaming](https://github.com/mrjex/Global-City-Streaming) project. It provides an interactive web interface for the data gathered in real-time across the system components.

## Overview

- **Interactive World Map:** Select countries to view real-time city data, including temperature and video feeds
- **3D Globe Visualization:** See monitored cities in real time on a dynamic globe
- **Live Video & Temperature Charts:** Watch city video streams and explore temperature trends
- **Kafka & Flink Analytics:** View real-time streaming analytics from the backend pipeline
- **Flink Log Viewer:** Inspect raw and database logs from the Flink processor
- **Production Charts Gallery:** Browse a gallery of production charts and city comparisons
- **Live Database Counter:** See the current number of records in the database, updated in real time


## Getting Started

<details>
  <summary>Localhost</summary>

1. **Install dependencies:**
   ```bash
   npm install
   ```
2. **Run the development server:**
   ```bash
   npm run dev
   ```
The app will be available at [http://localhost:3001](http://localhost:3001)

</details>


<details>
  <summary>Docker</summary>

1. **Build the Docker image:**
   ```bash
   docker build -t global-city-streaming-frontend .
   ```
2. **Run the container:**
   ```bash
   docker run -p 3001:3001 global-city-streaming-frontend
   ```

</details>


This frontend system component expects backend services ([City API](https://github.com/mrjex/City-API-Global-City-Streaming), [Kafka Producer](https://github.com/mrjex/Kafka-Producer-Global-City-Streaming), [Flink Processor](https://github.com/mrjex/Flink-Processor-Global-City-Streaming)) to be available as described in the [Global City Streaming](https://github.com/mrjex/Global-City-Streaming) main repository.
