# PwC-Switzerland-Power-BI-Job-Simulation
## 1. Diversity and Gender balance analysis
<img width="676" alt="image" src="https://github.com/user-attachments/assets/3c1a0dba-2a89-47bf-988b-4764d0a25715">

### a. Client context
Human Resources at our telecom client is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress. They’re reaching out to us for help.

### b. Dataset

| Column Name                       | Description                                                                           | Example                         |
|-----------------------------------|---------------------------------------------------------------------------------------|---------------------------------|
| Employee ID                       | Unique identifier for each employee.                                                  | 1                               |
| Gender                            | Gender of the employee (Male/Female).                                                 | Male                            |
| Job Level after FY20 promotions   | Job level of the employee after FY20 promotions.                                      | 6 - Junior Officer              |
| New hire FY20?                    | Indicates if the employee was a new hire in FY20 (Y/N).                               | N                               |
| FY20 Performance Rating           | Performance rating of the employee in FY20.                                           | 2                               |
| Promotion in FY21?                | Indicates if the employee received a promotion in FY21 (Yes/No).                      | No                              |
| In base group for Promotion FY21  | Indicates if the employee is part of the base group considered for promotion in FY21. | No                              |
| Target hire balance               | Indicates the target balance for hiring, likely for diversity purposes (e.g., 0.50).  | 0.5                             |
| FY20 leaver?                      | Indicates if the employee left the company in FY20 (Yes/No).                          | Yes                             |
| In base group for turnover FY20   | Indicates if the employee is part of the base group considered for turnover in FY20.  | Y                               |
| Department @01.07.2020            | Employee's department as of July 1, 2020.                                             | Operations                      |
| Leaver FY                         | Fiscal year in which the employee left, if applicable.                                | FY20                            |
| Job Level after FY21 promotions   | Job level of the employee after FY21 promotions.                                      | 4 - Manager                     |
| Last Department in FY20           | Last department of the employee in FY20.                                              | Operations                      |
| FTE group                         | Employment type (Full Time/Part Time).                                                | Full Time                       |
| Time type                         | Indicates whether the role is full-time or part-time.                                 | Full Time                       |
| Department & JL group PRA status  | PRA (Promotion Readiness Assessment) status by department and job level.              | Uneven - Men benefit            |
| Department & JL group for PRA     | Group classification for PRA by department and job level.                             | 4 - Manager & Sales & Marketing |
| Job Level group PRA status        | PRA status by job level.                                                              | Even                            |
| Job Level group for PRA           | Group classification for PRA by job level.                                            | 4 - Manager                     |
| Time in Job Level @01.07.2020     | Duration (in years) the employee has been in their job level as of July 1, 2020.      | 3                               |
| Job Level before FY20 promotions  | Job level of the employee before FY20 promotions.                                     | 6 - Junior Officer              |
| Promotion in FY20?                | Indicates if the employee received a promotion in FY20 (Yes/No).                      | N                               |
| FY19 Performance Rating           | Performance rating of the employee in FY19.                                           | 3                               |
| Age group                         | Age group classification of the employee.                                             | 30 to 39                        |
| Age @01.07.2020                   | Age of the employee as of July 1, 2020.                                               | 37                              |
| Nationality 1                     | Employee's primary nationality.                                                       | Spain                           |
| Region group: nationality 1       | Regional classification based on nationality.                                         | Europe                          |
| Broad region group: nationality 1 | Broader regional classification based on nationality.                                 | Europe                          |
| Last hire date                    | Most recent hire date of the employee.                                                | 01/04/2017                      |
| Years since last hire             | Number of years since the employee was last hired.                                    | 3                               |

### c. KPIs and Visualisation
#### Several KPIs that needs to be covered: 
- Number of men
- Number of women
- Number of leavers
- % employees promoted (FY21)
- % of women promoted
- % of hires men
- % of hires women
- % turnover 
- Average performance rating: men
- Average Performance rating: women

<img width="676" alt="image" src="https://github.com/user-attachments/assets/3c1a0dba-2a89-47bf-988b-4764d0a25715">


## 2. Customer retention analysis
<img width="715" alt="image" src="https://github.com/user-attachments/assets/f7230e01-87e1-46ae-aae4-b154a074cff7">

### a. Client inputs and requirement
#### Context from client:
- Customers in the telecom industry are hard-earned: client doesn’t want to lose them
- The retention department is here to get customers back in case of termination 
- Currently, client get in touch after they have terminated the contract, but this is reactionary: it would be better to know in advance who is at risk 
- Client  has done customer analysis with Excel: it has always ended in a dead-end
- Client would like to know more about our customers: visualised clearly so that it’s self-explanatory for our management

#### Client requirements:
Client would like to cover at least following issues: 
- Customers who left within the last month
- Services each customer has signed up for: phone, multiple lines, internet, online security, online backup, device protection, tech
support, and streaming TV and movies
Customer account information: how long as a customer, contract, payment method, paperless billing, monthly charges, total charges
and number of tickets opened in the categories administrative and technical
Demographic info about customers – gender, age range, and if they have partners and dependents

### b. Dataset
| Column Name      | Description                                                                            | Example          |
|------------------|----------------------------------------------------------------------------------------|------------------|
| customerID       | Unique identifier for each customer.                                                   | 7590-VHVEG       |
| gender           | Gender of the customer.                                                                | Female           |
| SeniorCitizen    | Indicates if the customer is a senior citizen (1 = Yes, 0 = No).                       | 0                |
| Partner          | Indicates if the customer has a partner (Yes/No).                                      | Yes              |
| Dependents       | Indicates if the customer has dependents (Yes/No).                                     | No               |
| tenure           | Number of months the customer has been with the company.                               | 1                |
| PhoneService     | Indicates if the customer subscribes to phone services (Yes/No).                       | No               |
| MultipleLines    | Indicates if the customer has multiple phone lines (Yes/No/No phone service).          | No phone service |
| InternetService  | Type of internet service the customer subscribes to (DSL/Fiber optic/No).              | DSL              |
| OnlineSecurity   | Indicates if the customer has online security service (Yes/No).                        | No               |
| OnlineBackup     | Indicates if the customer has online backup service (Yes/No).                          | Yes              |
| DeviceProtection | Indicates if the customer has device protection service (Yes/No).                      | No               |
| TechSupport      | Indicates if the customer has technical support service (Yes/No).                      | No               |
| StreamingTV      | Indicates if the customer subscribes to a TV streaming service (Yes/No).               | No               |
| StreamingMovies  | Indicates if the customer subscribes to a movie streaming service (Yes/No).            | No               |
| Contract         | Type of contract (Month-to-month/One year/Two year).                                   | Month-to-month   |
| PaperlessBilling | Indicates if the customer has paperless billing enabled (Yes/No).                      | Yes              |
| PaymentMethod    | Method used by the customer to pay bills (e.g., Electronic check, Mailed check, etc.). | Electronic check |
| MonthlyCharges   | Amount charged to the customer monthly (in USD).                                       | 29.85            |
| TotalCharges     | Total amount charged to the customer (in USD).                                         | 29.85            |
| numAdminTickets  | Number of administrative tickets raised by the customer.                               | 0                |
| numTechTickets   | Number of technical tickets raised by the customer.                                    | 0                |
| Churn            | Indicates if the customer churned (Yes/No).                                            | No               |

### c. KPIs and visualisation
<img width="715" alt="image" src="https://github.com/user-attachments/assets/f7230e01-87e1-46ae-aae4-b154a074cff7">


