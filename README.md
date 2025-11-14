

Variable Declarations

**int ProductID[10];**
Stores the ID of each product.

**int Quantity[10];**
Stores the quantity of each product.

**float Price[10];**
Stores the price of each product.

**char ProductName[10][50];**
Stores the name of each product (as a 2D array of strings).

**int num, a;**
`num` holds the number of products.
`a` stores the product ID to search.

**float Total, highest, lowest;**
`Total` stores total cost of each product.
`highest` and `lowest` track the highest and lowest prices.



 Input Section

**printf("Enter the number of products: ");**
Asks the user how many products they want to enter.

**scanf("%d", &num);**
Reads the number of products.



 Loop for Product Entry

**for (int i = 0; i < num; i++)**
Iterates once for each product.

**scanf("%d", &ProductID[i]);**
Reads product ID.

**scanf("%s", ProductName[i]);**
Reads product name.

**scanf("%d", &Quantity[i]);**
Reads product quantity.

**scanf("%f", &Price[i]);**
Reads product price.

**Total = Quantity[i] * Price[i];**
Calculates total cost of that product.



### Per-Product Output

Prints Product ID, Name, Quantity, Price, and Total.



Finding Highest & Lowest Price

**highest = Price[0]; lowest = Price[0];**
Initializes both to the first product’s price.

Loop through remaining prices:

* If a price is higher, update `highest`.
* If a price is lower, update `lowest`.

Print the highest and lowest price values.



Product Search

**printf("Enter a product ID to search: ");**
Asks the user for an ID.

**scanf("%d", &a);**
Stores the ID to search.

Loop through product list:

* If `ProductID[i] == a`, print its details.
* Set `found = 1`.

If `found` remains 0, display “product not found”.



Program Ends

**return 0;**
Exits the program successfully.
