0. remove empty lines before complete lines (no more than one, because the number of empty lines contains information. we're only stripping out one of them to make it more human-readable, and perhaps a bit easier to parse.)

1. strip out quotations
  * find the name after the quotation and remove the line above it. That *should* get all of them.
2. match flavors from table
  * the ingredients are sorted alphabetically
  * each ingredient is in all-caps and has (at least) three line breaks before it starts   

We have styles (e.g. "Moroccan cuisine") and ingredients (e.g. garlic). Some styles and ingredients are really sets of other styles and ingredients. For example, the cuisine "African Cuisine" encompasses "Moroccan Cuisine", "Ethiopian Cuisine", and more. The ingredient "wine" encompasses "Cabernet Sauvignon", "Riesling", and more.