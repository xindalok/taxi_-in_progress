# taxi

### Introduction
This Jupyter Notebook is dedicated to analyzing municipal expenditures on Snow and Ice removal in the year 2022.

The primary objectives of this analysis are as follows:

1. Using Python, perform EDA on the taxi data from the New York City TLC to get a general understanding of what taxi ridership looks like

2. I would suggest at the very least a box plot of the ride durations and some time series plots, like a breakdown by quarter or month. Whatever you think makes the most sense.

3. Additionally, the management team has recently asked all EDA to include Tableau visualizations. We’ve found these to be particularly helpful in status reports to the client and board members. Make sure it is easy to understand to someone who isn’t data savvy and remember that the assistant director at the New York City TLC is a person with visual impairments.

4. it would be really helpful if you included an executive summary of your analysis attached via email.



---

## 📄 Dataset Description

The dataset includes trip-level records for yellow taxis in NYC. Below is a description of the key columns:

- **ID**: Trip identification number  
- **VendorID**: Code indicating the TPEP provider  
  - `1` = Creative Mobile Technologies, LLC  
  - `2` = VeriFone Inc.

- **tpep_pickup_datetime**: Timestamp when the meter was engaged  
- **tpep_dropoff_datetime**: Timestamp when the meter was disengaged  
- **passenger_count**: Number of passengers (driver-entered)  
- **trip_distance**: Distance traveled (in miles)  
- **PULocationID**: Pickup location (TLC zone ID)  
- **DOLocationID**: Drop-off location (TLC zone ID)  
- **RateCodeID**: Rate code used for the trip  
  - `1` = Standard rate  
  - `2` = JFK  
  - `3` = Newark  
  - `4` = Nassau or Westchester  
  - `5` = Negotiated fare  
  - `6` = Group ride  

- **store_and_fwd_flag**: Whether the trip data was temporarily stored before sending  
  - `Y` = Store and forward  
  - `N` = Not stored  

- **payment_type**: How the passenger paid  
  - `1` = Credit card  
  - `2` = Cash  
  - `3` = No charge  
  - `4` = Dispute  
  - `5` = Unknown  
  - `6` = Voided trip  

- **fare_amount**: Meter-calculated fare  
- **extra**: Misc. surcharges (rush hour, overnight, etc.)  
- **mta_tax**: $0.50 MTA tax  
- **improvement_surcharge**: $0.30 fee added at flag drop  
- **tip_amount**: Tip amount (credit card tips only)  
- **tolls_amount**: Total tolls charged  
- **total_amount**: Total fare (excluding cash tips)

---

*Let’s dive into the data to uncover trends and insights that could help align snow removal budgeting with ridership demand patterns.*


