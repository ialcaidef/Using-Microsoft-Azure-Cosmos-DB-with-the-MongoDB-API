Using Microsoft Azure Cosmos DB with the MongoDB API

Demonstration Steps

1. Open Microsoft Edge.
2. Go to https://portal.azure.com and sign in with your credentials.
3. In the left pane, click Azure Cosmos DB.
4. On the top bar, click Add.
5. In the Create Azure Cosmos DB Account pane, in the Account name box, type mod7demo3{YourInitials}.
6. In API, select MongoDB.
7. In Resource group section, select Create new, in the Name box type Mod7Demo3ResourceGroup and then click OK.
8. Click Review + Create and then click Create.
9. Wait for the database to be created.
10. In the left pane, click Azure Cosmos DB, and then click mod7demo3{YourInitials}.
11. In mod7demo3{YourInitials}, in the left pane, click Data Explorer.
12. On the top bar, click New Collection.
13. In Database id, select Create new, and then type mydb.
14. In Collection id, type customers.
15. Click Add unique key, and then type customerId.
16. Click Ok.
17. On the top bar, click New Collection.
18. In Database id, select Use existing, and then select mydb.
19. In Collection id, type orders.
20. Click Ok.
21. Right-click customers, and then select New Shell.
22. In [Repository Root]\Allfiles\Mod07\DemoFiles\Mod7Demo3Assets, from the CustomersCollectionData.json file, copy all the content.
23. In the shell 1 console, paste the customer data copied from CustomersCollectionData.json, and then press Enter.
24. In [Repository Root]\Allfiles\Mod07\DemoFiles\Mod7Demo3Assets, from the OrdersCollectionData.json file, copy all the content.
25. In shell 1 console, paste the orders data copied from OrdersCollectionData.json, and then press Enter.
26. Right-click orders, and then select New Query.
27. To get all the orders, paste the following query, and then click Execute Query.
         {}
28. To get all the orders at a price greater than $20, paste the following query, and then click Execute Query.
         { price: {$gt: 20} }
29. To get all the orders of customer 1, paste the following query, and then click Execute Query.
         { customerId: "1" }
30. Close all windows.

