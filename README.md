# Global City Streaming Frontend

This repository is the **frontend submodule** of the [Global City Streaming](https://github.com/mrjex/Global-City-Streaming) project. It provides a modern, interactive web interface for real-time monitoring, visualization, and analytics of city data streamed from a global network.

## Overview

- **Interactive World Map:** Select countries to view real-time city data, including temperature and video feeds.
- **3D Globe Visualization:** See monitored cities in real time on a dynamic globe.
- **Live Video & Temperature Charts:** Watch city video streams and explore temperature trends.
- **Kafka & Flink Analytics:** View real-time streaming analytics from the backend pipeline.
- **Flink Log Viewer:** Inspect raw and database logs from the Flink processor.
- **Production Charts Gallery:** Browse a gallery of production charts and city comparisons.
- **Live Database Counter:** See the current number of records in the database, updated in real time.

## Tech Stack

- **Framework:** [Next.js](https://nextjs.org/) (React, TypeScript)
- **Styling:** [TailwindCSS](https://tailwindcss.com/)
- **Data Visualization:** [D3.js](https://d3js.org/), [Plotly.js](https://plotly.com/javascript/)
- **Animation:** [Framer Motion](https://www.framer.com/motion/)
- **Containerization:** Docker

## Features

### 🌍 Interactive World Map
- Select a country to view its cities, temperature data, and live video feeds.
- Initial load focuses on Sweden, but any country can be selected.

### 🟢 Real-Time Globe View
- Visualize all monitored cities (static and dynamic) on a 3D globe.
- Cities update in real time as data streams in.

### 📊 Production Charts Gallery
- Explore a variety of real-time and historical charts, including temperature rankings and city comparisons.
- Custom chart query panel for advanced analytics.

### ⚡ Kafka & Flink Analytics
- View the status and metrics of the Kafka producer and Flink processor.
- Inspect Flink logs (raw and database) directly from the UI.

### 🗄️ Live Database Counter
- Displays the current number of records in the database, updating every 2 seconds.

## Getting Started

### Prerequisites
- [Docker](https://www.docker.com/) (recommended for production)
- [Node.js](https://nodejs.org/) (for local development)

### Local Development

1. **Install dependencies:**
   ```bash
   npm install
   ```
2. **Run the development server:**
   ```bash
   npm run dev
   ```
   The app will be available at [http://localhost:3001](http://localhost:3001).

### Docker Deployment

1. **Build the Docker image:**
   ```bash
   docker build -t global-city-streaming-frontend .
   ```
2. **Run the container:**
   ```bash
   docker run -p 3001:3001 global-city-streaming-frontend
   ```

The frontend expects backend services (API, Kafka, Flink, database) to be available as described in the [Global City Streaming](https://github.com/mrjex/Global-City-Streaming) main repository.
