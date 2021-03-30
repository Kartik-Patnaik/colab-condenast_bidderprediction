# colab-condenast_bidderprediction
Business Objective: 
You'll be chasing down robots for an online auction site. Human bidders on the site are becoming increasingly frustrated with their inability to win auctions vs. their software-controlled counterparts. As a result, usage from the site's core customer base is plummeting.
In order to rebuild customer happiness, the site owners need to eliminate computer generated bidding from their auctions. Their attempt at building a model to identify these bids using behavioral data, including bid frequency over short periods of time, has proven insufficient. 
The goal is to identify “robots” which are making bids, helping the site owners easily flag these users for removal from their site to prevent unfair auction activity. 
 
Data Description: 
There are two datasets in this task. One is a bidder dataset that includes a list of bidder information, including their id, payment account, and address. The other is a bid dataset that includes 7.6 million bids on different auctions. The bids in this dataset are all made by mobile devices.
The online auction platform has a fixed increment of dollar amount for each bid, so it doesn't include an amount for each bid. You are welcome to learn the bidding behavior from the time of the bids, the auction, or the device. 
File descriptions
train.csv - the training set from the bidder dataset
test.csv - the test set from the bidder dataset
sampleSubmission.csv - a sample submission file in the correct format
bids.csv - the bid dataset
Data fields
For the bidder dataset
bidder_id – Unique identifier of a bidder.
payment_account – Payment account associated with a bidder. These are obfuscated to protect privacy. 
address – Mailing address of a bidder. These are obfuscated to protect privacy. 
robot_act_prob_lk - An anonymised characteristic of a bidder.
outcome – Label of a bidder indicating whether or not it is a robot. Value 1.0 indicates a robot, where value 0.0 indicates human.
 
For the bid dataset
bid_id - unique id for this bid
bidder_id – Unique identifier of a bidder (same as the bidder_id used in train.csv and test.csv)
auction – Unique identifier of an auction
merchandise –  The category of the auction site campaign, which means the bidder might come to this site by way of searching for "home goods" but ended up bidding for "sporting goods" - and that leads to this field being "home goods". This categorical field could be a search term, or online advertisement. 
device – Phone model of a visitor
time - Time that the bid is made (transformed to protect privacy).
country - The country that the IP belongs to
ip – IP address of a bidder (obfuscated to protect privacy).
url - url where the bidder was referred from (obfuscated to protect privacy). 


Submission:

You are required to code the solution in Python and mail the a).ipynb file b)scored test file along with a deck presenting the model insights.

