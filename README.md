# kata-test
First thing I did was to break down the task into the various variables needed to track/calculate the checkout system.

Next I focused on getting the individual items to add up correctly, including triggering the discount and the simple button layout.

For the discount I needed a item counter so it would trigger the code, along with resetting so if more were items were added the discount would retrigger. I also added a total item counter which I thought I might be able to use later on for the total amount.

Once I had the discount in place, I looked at implementing into the other items so if discounts were needed for C & D the code is in place to update. This required me to add addition varibles and make the discount more flexible and robust so you could turn on/off for any of the items (e.g aMultiDiscount).

Next up was trying to implement the total price of number of items. I added the updateShopTotal() function to handle the calculation, with a new boolean so that only correct item loop would trigger, so not to add other total costs of other items together.

Sadly this didn't work as intended as shopTotalCost += aTotalCost; is adding the shopTotalCost again, and not just adding aTotalCost onto the shopTotalCost figure.

And that is were I got up to by the end of the 1.5 hour time limit.

If I had more time I would obviously look at fixing the total shop calculation but also look at adding a removal option from the cart, which I thought about when adding the aTotalCount varibles. Though I would need a better maths solution to the discount option as I would have to calculate it on the total item amount and not just after 3 clicks on the A button for example.
