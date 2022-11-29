# Scrapping-and-analysis-of-immigration-data-from-reddit

Using this code, we can retrieve reddit posts between two dates defined as "posted after" and "posted before".
As the pushshift API has a maximum of 250 posts each iteration, we use a while loop to increment "posted after" by 10 days in each iteration, giving us the most recent 250 posts in that 10 day span.

We will lose data because we are incrementing 864000, which will result in collecting 250 posts in 10 days. To avoid this, reduce the time in the while loop to 86400, which will increase the number of iterations and result in 250 posts every day. 
This can also result in duplicate values so make sure to remove duplicates.

Libraries used:
Datetime
Requests
Json
Pandas
Numpy
Re

To run the file simply start running the code from the first cell.
