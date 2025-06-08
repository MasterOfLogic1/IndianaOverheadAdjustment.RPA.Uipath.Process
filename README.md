### Indiana Overhead Adjustment RPA Uipath Process ###

The screenshots here are the screenshots fof the application been automated . the info you see on the screen are only fakepatient data nad not real. the screenshots were downloaded from https://www.crowdreviews.com/matrixcare/product-info

![image](https://github.com/user-attachments/assets/d7896ff4-aff4-4bbc-b7d5-19e3c4026ad8)

![image](https://github.com/user-attachments/assets/be76c909-e89b-4087-a1dc-9a1ccde5f891)

![image](https://github.com/user-attachments/assets/b08923ba-0990-4a13-9a77-a907251ded0c))


**Overhead Adjustment – Automated Process**

1. Load the invoice data into the bot queue.
2. The bot logs in to the MatrixCare application.
3. It pulls the next invoice item from the queue.
4. The bot navigates to **Billing ▸ Search Invoices** in MatrixCare.
5. It searches by *Invoice ID*, *Office*, and *Invoice Date*.
6. The search returns a table of transactions for that invoice.
7. The bot targets rows whose **Posting Balance** equals **– \$34.50**.
8. For each matching row, it updates the **Posting Balance** and **Posting Date**.
9. The bot returns to the queue and repeats steps 3–8 until every item is processed.
10. When the queue is empty, the bot sends a completion email.

