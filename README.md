# 🏨 Project Overview
The client for this research is the hotel chain “Like Home”. To attract more customers, the chain added an option to book rooms without prepayment on its website. However, when customers canceled their bookings, the company suffered losses. Hotel staff might have already purchased supplies for the guest’s arrival or missed the chance to book the room for someone else.

To solve this issue, your task is to develop a system that predicts booking cancellations. If the model predicts that a booking will be canceled, the customer will be asked to pay a deposit. The deposit amount is 80% of the cost of one night’s stay plus the one-time cleaning fee. This amount will be charged if the customer cancels the booking.

## 💰 Business Metric and Other Details
The main business metric for any hotel chain is profit. Hotel profit is the difference between the total room cost for all nights and the service expenses — both for preparing the room and during the guest’s stay.

There are several room types, each with its own nightly rate and cleaning cost. If the guest stays for a long time, cleaning is done every two days.

### Room Pricing:
Category	Nightly Rate	One-Time Cleaning
A	1,000	400
B	800	350
C	600	350
D	550	150
E	500	150
F	450	150
G	350	150
### Seasonal Pricing Coefficients:
- Spring & Autumn: +20%
- Summer: +40%

### Cancellation Losses:
If a booking is canceled, the hotel loses the cost of one night and one cleaning, adjusted by the seasonal coefficient.

## 💼 Budget and ROI
The budget for developing the prediction system is 400,000 rubles. The system must pay for itself during the test period — meaning the revenue it generates must exceed development costs.

## 🧭 Project Instructions
### Step 1: Load the Data
Paths to the files:

- /datasets/hotel_train.csv — training data
- /datasets/hotel_test.csv — test data

### Step 2: Data Preprocessing and Exploratory Analysis
- Check and clean the data if needed.
- Perform exploratory data analysis.
- Describe any findings: missing values, outliers, etc.

### Step 3: Calculate the Business Metric
- Estimate hotel profit without implementing deposits.

### Step 4: Develop the ML Model
- Train different models and evaluate their performance using cross-validation.
- Choose the best model and test it on the test set.
- Describe your conclusions.
- Select a metric for training.
- Estimate the profit the chosen model would generate over a year.

### Step 5: Identify “Unreliable” Customers
- Based on your data analysis, describe the profile of a customer likely to cancel a booking.

### Step 6: Write a Final Summary
- Describe the model that delivers the greatest business benefit.
- Provide recommendations to the business based on your findings.

## 📝 Formatting Guidelines
- Complete the task in Jupyter Notebook.
- Use code cells for code and markdown cells for explanations.
- Use formatting and headings for clarity.

## 📊 Data Description
Both hotel_train and hotel_test contain the same columns:

- id — record ID
- adults — number of adult guests
- arrival_date_year — year of arrival
- arrival_date_month — month of arrival
- arrival_date_week_number — week of arrival
- arrival_date_day_of_month — day of arrival
- babies — number of babies
- booking_changes — number of booking changes
- children — number of children aged 3–14
- country — guest’s nationality
- customer_type — customer type:
  - Contract — corporate contract
  - Group — group booking
  - Transient — individual booking
  - Transient-party — individual booking linked to a group
- days_in_waiting_list — days the booking waited for confirmation
- distribution_channel — booking channel
- is_canceled — booking cancellation flag
- is_repeated_guest — whether the guest has booked before
- lead_time — days between booking and arrival
- meal — meal plan:
  - SC — no meals
  - BB — breakfast
  - HB — breakfast and lunch
  - FB — breakfast, lunch, and dinner
- previous_bookings_not_canceled — number of confirmed bookings by the customer
- previous_cancellations — number of canceled bookings by the customer
- required_car_parking_spaces — need for parking
- reserved_room_type — reserved room type
- stays_in_weekend_nights — weekend nights stayed
- stays_in_week_nights — weekday nights stayed
- total_nights — total nights stayed
- total_of_special_requests — number of special requests

## ✅ Project Evaluation Criteria
Reviewers will assess your project based on:

- Quality of data preparation and analysis
- Models built and how their performance is evaluated
- Completion of all steps with clear commentary
- Code structure and cleanliness
- Avoidance of code duplication
- Notebook formatting and organization
- Quality of conclusions
Everything you need to complete the project is covered in previous course topics.

Good luck! 🍀
