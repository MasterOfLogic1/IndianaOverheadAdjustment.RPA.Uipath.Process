### Indiana Overhead Adjustment RPA Uipath Process ###

The screenshots here are the screenshots fof the application been automated . the info you see on the screen are only fakepatient data nad not real. the screenshots were downloaded from https://www.crowdreviews.com/matrixcare/product-info

![image](https://github.com/user-attachments/assets/d7896ff4-aff4-4bbc-b7d5-19e3c4026ad8)

![image](https://github.com/user-attachments/assets/be76c909-e89b-4087-a1dc-9a1ccde5f891)

![image](https://github.com/user-attachments/assets/b08923ba-0990-4a13-9a77-a907251ded0c))


IN Overhead Adjustment
 
1.) we load the invoice data into the bot queue
2.) bot logs into matrix care app
3.) bot picks up an invoice item from the queue 
4.) Bot Navigates to "Billing> Search Invoices" Page on Matrix care app
5.) Bot searches for the invoice on the "Search Invoices Page" going by invoice id , office and invoice date
6.) This result of the search is table showing several transactions related to the given invoice
7.) On this result, the bot focuses on items which have balance of $-34.50 as posting balance
6.) for each item with $-34.50, the bot updates the posting balance and posting date
7.) The bot returns back to the queue to get the next queue item
8.) the steps rom 3-7 are repeated until all items on the queue are finished
10.) when the process finishes an email is sent
