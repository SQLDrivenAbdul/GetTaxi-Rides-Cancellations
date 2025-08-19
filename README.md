# GetTaxi-Rides-Cancellations


## Project Overview
<p align="justify">
Gett, previously known as GetTaxi, is an Israeli-developed technology platform solely focused on corporate Ground Transportation Management (GTM). They have an application where clients can order taxis, and drivers can accept their rides (offers). At the moment, when the client clicks the Order button in the application, the matching system searches for the most relevant drivers and offers them the order. In this task, i investigated some matching metrics for orders that were not completed successfully, i.e., the customer didn't end up getting a car.
</p>


## Data Source
These Datasets were gotten from Stratascatch, a platform for solving Data Science problems. The platform provided two tables data_orders and data_offers


### 📖 Data Dictionary — data_orders  

| **Column Name**              | **Description**                                                                 |
|------------------------------|---------------------------------------------------------------------------------|
| `order_gk`                   | Unique identifier for each order                                                 |
| `order_datetime`             | Date and time when the order was created                                         |
| `origin_longitude`           | Longitude of the customer’s pickup location                                      |
| `origin_latitude`            | Latitude of the customer’s pickup location                                       |
| `m_order_eta`                | Estimated time of arrival for driver to reach the customer (in minutes)          |
| `cancellations_time_in_seconds` | Time (in seconds) before cancellation occurred after order placement          |
| `order_status_key`           | Status code of the order (e.g., completed, cancelled)                            |
| `is_driver_assigned_key`     | Indicates whether a driver was assigned (1 = Yes, 0 = No)                        |




### 📖 Data Dictionary — data_offers  

| **Column Name**              | **Description**                                                                 |
|------------------------------|---------------------------------------------------------------------------------|
| `order_gk`                   |Order number, associated with the same column from the `data_orders` dataset                                                |
| `offer_id`                   |  Unique identifier of an offer                                                  |





