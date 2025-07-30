<img width="366" height="163" alt="Screenshot 2025-07-30 142003" src="https://github.com/user-attachments/assets/63ac7c0a-a835-4acc-85dd-3ae790cd9122" />

# Exposed Metrics
In the challenge description, there was a link that led to `https://github.com/prometheus/prometheus`

After reading the GitHub repository on prometheus, I assumed that it was the monitoring system that the challenge was talking about, 
now all we need to do is find the endpoint.

So... at this point I can't be bothered to read through more of the GitHub to find the answer so I did a quick google search: `prometheus endpoint`

Clicking on the first link that shows up like a lazy person, I searched the page for the keyword `endpoint` and found:

<img width="1916" height="912" alt="image" src="https://github.com/user-attachments/assets/93c79a06-1e37-4525-92ca-843fef9014e9" /> <br/><br/>

The metrics endpoint was being served on the `/metrics` subdirectory so I tried it on JuiceShop:

<img width="923" height="647" alt="image" src="https://github.com/user-attachments/assets/dee15da1-8ab6-47de-8727-37ce73a130d4" /> <br/><br/>

And there it was the metrics endpoint. To verify that i had the correct one, I went back to the home page and the challenge had been marked completed so I guess it was the correct one 


