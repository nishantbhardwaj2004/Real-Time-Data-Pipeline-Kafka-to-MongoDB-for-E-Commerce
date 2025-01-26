# Real-Time Data Pipeline: Kafka to MongoDB for E-Commerce

### Table of Contents:
1. Overview
2. Features
3. Architecture
4. Prerequisites
5. Project Setup
6. Usage
7. Dashboard Insights
8. Conclusion
9. License

### Overview:
This project showcases a real-time data pipeline connecting Confluent Kafka and MongoDB. Designed for an e-commerce platform, it simulates continuous data production of order information by a Kafka producer. The data flows through Kafka to MongoDB, where it is stored and visualized in real-time on a dashboard.

### Features:
- Real-time data ingestion: Simulate continuous streaming of order data into Kafka.
- Efficient data processing: Kafka topics handle high-throughput, fault-tolerant data streaming.
- MongoDB integration: Real-time ingestion and storage of order data.
- Interactive visualization: Use MongoDB Compass or Atlas dashboards to explore and monitor data.

### Architecture:
1. Kafka Producer: Simulates an e-commerce order system by generating order data and publishing it to Kafka topics categorized by country.
2. Kafka Topics: Buffer data with partitioning for scalability and efficient processing.
3. Kafka MongoDB Sink Connector: Transfers data from Kafka topics to MongoDB collections in real-time.
4. MongoDB Dashboard: Visualizes and analyzes stored order data for insights.

### Prerequisites:
Ensure you have the following installed and configured:-

- Confluent Kafka (Confluent Platform or Confluent Cloud).
- MongoDB (local or cloud instance, e.g., MongoDB Atlas).
- Kafka Connect MongoDB Sink Connector.
- Python (to develop Kafka producer/consumer scripts).
- MongoDB Compass (for data visualization).

### Project Setup:
1. Start Confluent Kafka and ensure all services are running.
2. Create a Kafka topic to handle order data categorized by country.
3. Configure and deploy the Kafka MongoDB Sink Connector to transfer data to MongoDB.
4. Use MongoDB Compass or Atlas to visualize and monitor real-time data in the database.

### Usage:
1. Start the Kafka producer to simulate real-time e-commerce order data.
2. Monitor the Kafka topic to verify data flow.
3. Confirm data ingestion into MongoDB.
4. Visualize the data using MongoDB Compass or Atlas dashboards.

### Dashboard Insights:
The dashboard in MongoDB represents the total number of records (orders) categorized by country. This provides a clear, real-time view of the volume of orders originating from different regions. Key insights include:-

- Order Distribution by Country: Total number of orders grouped by country.
- Data Trends: Ability to observe trends over time, such as order spikes or consistent activity from specific regions.

### Conclusion:
This project demonstrates the effectiveness of integrating Kafka and MongoDB to create a scalable and efficient real-time data pipeline for e-commerce platforms. By leveraging Kafka's streaming capabilities and MongoDB's robust data storage and visualization tools, this pipeline provides actionable insights into order distributions and trends. This solution can be further adapted to various industries requiring real-time data processing and analysis.
