# Maps


## Exercises


## **1. Create and Print a Map**
* Create a `Map` where keys are country names and values are their capitals.
* Print the `Map`.

## **2. Access Elements**
* Create a `Map` of fruits and their prices: `{"apple": 2, "banana": 1, "cherry": 3}`.
* Access and print the price of `"banana"`.

## **3. Add and Remove Elements**
* Create an empty `Map` of strings (keys) and integers (values).
* Add the following key-value pairs: `"one": 1`, `"two": 2`, `"three": 3`.
* Remove the key `"two"`.
* Print the updated `Map`.

## **4. Iterate Through a Map**
* Create a `Map` of students and their grades: `{"Alice": 85, "Bob": 90, "Charlie": 78}`.
* Use a `for` loop to print each student's name and grade.

## **5. Check for Key and Value**
* Create a `Map` of products and their stock: `{"laptop": 10, "phone": 15, "tablet": 5}`.
* Check if `"tablet"` is a key in the `Map` and if any product has a stock of 15. Print the results.

## **6. Filter a Map**
* Create a `Map` of items and their prices: `{"pen": 1.5, "notebook": 3.0, "eraser": 0.5, "ruler": 2.0}`.
* Use the `where()` method to filter and print items with prices greater than 2.

## **7. Transform Map Values**
* Create a `Map` of items and their prices: `{"pen": 1.5, "notebook": 3.0, "eraser": 0.5}`.
* Use the `map()` method to apply a 10% discount to each price and print the updated `Map`.

## **8. Count Entries**
* Create a `Map` of ages: `{"John": 25, "Emma": 30, "Sophia": 22}`.
* Print the number of entries in the `Map`.

## **9. Combine Two Maps**
* Create two `Map`s: `{"a": 1, "b": 2}` and `{"c": 3, "d": 4}`.
* Merge them into a single `Map` and print the result.

## **10. Find Key by Value**
* Create a `Map` of countries and their dialing codes: `{"US": 1, "IN": 91, "UK": 44}`.
* Use the `entries` property to find and print the key (country) corresponding to the dialing code `91`.

## **11. Sort a Map by Keys**
* Create a `Map` of grades: `{"Charlie": 78, "Alice": 85, "Bob": 90}`.
* Sort the `Map` by keys alphabetically and print the result.

## **12. Sort a Map by Values**
* Create a `Map` of items and their prices: `{"notebook": 3.0, "pen": 1.5, "eraser": 0.5}`.
* Sort the `Map` by values in ascending order and print the result.

## **13. Use Default Values**
* Create a `Map` of countries and their capitals: `{"France": "Paris", "Italy": "Rome"}`.
* Access the value for `"Germany"`, but provide a default value of `"Unknown"` if it doesn't exist.

## **14. Convert Map to List**
* Create a `Map` of students and their grades: `{"Alice": 85, "Bob": 90, "Charlie": 78}`.
* Convert the keys to a `List` and print them.
* Convert the values to a `List` and print them.

## **15. Check If All Values Meet Condition**
* Create a `Map` of items and their quantities: `{"pens": 10, "notebooks": 15, "erasers": 5}`.
* Use the `values` property and the `every()` method to check if all quantities are greater than 4. Print the result.

## **16. Check If Any Key Meets Condition**
* Create a `Map` of products and their prices: `{"laptop": 1000, "phone": 700, "tablet": 400}`.
* Use the `keys` property and the `any()` method to check if any product name starts with `"p"`. Print the result.

## **17. Group by Key Prefix**
* Create a `Map` of words and their frequencies: `{"apple": 3, "ape": 2, "banana": 5, "berry": 4}`.
* Group words by their first letter into a new `Map`, where the keys are the first letters and the values are lists of words. Print the result.

## **18. Invert a Map**
* Create a `Map` of country codes: `{"US": "America", "FR": "France", "JP": "Japan"}`.
* Swap keys and values to create a new `Map` where the values become the keys and the keys become the values.

## **19. Compute If Absent**
* Create a `Map` of product stock: `{"pen": 10, "notebook": 5}`.
* Use `putIfAbsent()` to add `"eraser"` with a stock of `20` only if it doesn't already exist. Print the updated `Map`.

## **20. Aggregate Map Values**
* Create a `Map` of sales data: `{"January": 1000, "February": 1200, "March": 900}`.
* Use the `values` property and the `reduce()` method to calculate and print the total sales.
