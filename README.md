# Chef's Favourite Meals

Welcome to the Chef's Favourite Meals app! This JavaScript application interacts with The Meal DB API to take and complete orders of the chef's favourite meals. The application uses the `prompt()` and `alert()` functions for user interactions, the `fetch` API for consuming the Meal DB API, and `sessionStorage` to store order details.

## Features

1. **Taking Orders:**
   - Prompt the user for the main ingredient.
   - Call the API to retrieve a list of meals based on the main ingredient.
   - Randomly select a meal from the list and set it as the order.
   - Store the order details in `sessionStorage`.

2. **Storing Orders:**
   - Ensure each new order has a unique order number.
   - Store the collection of orders as a single value in a JSON array.
   - Store the last generated order number separately.

3. **Displaying and Completing Orders:**
   - Display all incomplete orders stored in `sessionStorage`.
   - Prompt the user to enter the order number to mark as complete or enter zero to skip.
   - Update the order's completion status and save it to `sessionStorage`.

## How to Use

1. **Open the HTML File:**
   - Open the `mealingredients.html` file in your web browser.

2. **Taking an Order:**
   - The app will prompt you to enter the main ingredient for your meal.
   - Enter the main ingredient (e.g., "chicken", "beef", "pork").
   - The app will fetch meals from The Meal DB API based on the ingredient and randomly select a meal.
   - The order details will be displayed in an alert box.

3. **Completing an Order:**
   - After taking an order, the app will display all incomplete orders.
   - Enter the order number to mark it as complete or enter zero to skip.
   - The app will update the order's status and save it to `sessionStorage`.

## Example

1. **Taking an Order:**
   - Prompt: "Enter the main ingredient for your meal:"
   - User Input: "chicken"
   - Alert: "Order Details:\nOrder Number: 1\nMeal: Chicken Alfredo\nStatus: Incomplete"

2. **Completing an Order:**
   - Prompt: "Incomplete Orders:\nOrder Number: 1, Meal: Chicken Alfredo\n\nEnter the order number to mark as complete, or 0 to skip:"
   - User Input: "1"
   - Alert: "Order Number 1 marked as complete."

## Notes

- If the API returns no meals for the entered ingredient, the app will prompt you to enter another ingredient.
- The app uses `sessionStorage` to store order details, so the data will be lost when the browser is closed.

## License

This project is licensed under the MIT License.

## Contact

For any questions or feedback, please contact Sipho Sisusa at sisusasipho@gmail.com.
