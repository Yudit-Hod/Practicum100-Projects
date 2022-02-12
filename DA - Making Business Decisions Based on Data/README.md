# Project description
You are an analyst at a big online store. Together with the marketing department, you've compiled a list of hypotheses that may help boost revenue.
You need to prioritize these hypotheses, launch an A/B test, and analyze the results.

# Description of the data  

**The dataset used to prioritize the hypothesis contains the following fields:**  
`Hypotheses` — brief descriptions of the hypotheses  
`Reach` — user reach, on a scale of one to ten  
`Impact` — impact on users, on a scale of one to ten  
`Confidence` — confidence in the hypothesis, on a scale of one to ten  
`Effort` — the resources required to test a hypothesis, on a scale of one to ten.   
The higher the Effort value, the more resource-intensive the test.  

**The data containing the A/B test results consists of 2 tables:**   
Table **`orders`** contans information about orders:  
`transactionId` — order identifier  
`visitorId` — identifier of the user who placed the order  
`date` — of the order  
`revenue` — from the order  
`group` — the A/B test group that the user belongs to  

Table **`visits`** contains information about visits:  
`date` — date  
`group` — A/B test group  
`visits` — the number of visits on the date specified in the A/B test group specified
