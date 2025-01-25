# Search Module Load Tests

This project aims to analyze the performance and behavior of the search module on [n11.com](https://www.n11.com/) through load tests.

## Objective
To measure the performance of the search module and observe its behavior under different scenarios.

## Requirements
- Perform a dynamic search for a specified product.
- Identify and search for the most popular term from the homepage.
- Tests are conducted using **Apache JMeter** or **Locust** (1 user is sufficient).

## Test Scenarios

### 1. Dynamically Search for a Specified Product
- **Objective**: To search for a product specified by the user.
- **Steps**:
  1. The user inputs a product name (e.g., "phone").
  2. The search module is triggered.
  3. Measure the time taken for results to load.
  4. Verify HTTP response codes.

### 2. Search for the Most Popular Term from the Homepage
- **Objective**: To select one of the most popular searches from the homepage and search for it.
- **Steps**:
  1. Fetch the list of popular search terms from the homepage.
  2. Select the first item from the list.
  3. Search for the selected item in the system.
  4. Measure the time taken for results to load.
  5. Verify HTTP response codes.

## Tools and Technologies Used
- **Apache JMeter**: Used to perform the load tests.
- **Dynamic Data Usage**:
  - User inputs are allowed for specified product searches.
  - HTTP responses are parsed to identify popular search terms.

## How to Use
1. Clone the project:
   ```bash
   git clone https://github.com/username/jmeter-test-plans.git
   ```
2. Open the `.jmx` file in JMeter.
3. Update the test parameters (e.g., search keyword).
4. Run the test and analyze the results.

## Test Results
- **Dynamic Product Search**:
  - Average response time: 2000 ms
  - HTTP success rate: 100%

- **Popular Search**:
  - Average response time: 3500 ms
  - HTTP success rate: 100%

## Notes
- Tests are designed for 1 user. To test with more users, update the `Thread Group` settings.
- To ensure proper functionality of popular searches, analyzing the target system's API structure might be necessary.

```
```
## **Contributors**

- **Irem Vardan, Msc**
    -  Senior Test Automation Engineer
    - [GitHub Profile](https://github.com/remvrdn)
---
