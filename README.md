# python
Learning new tricks to be solve things and get easy solutions.

How to Extract a Product Name From a URL Using Python

python
Copy code
import re

url = "https://www.example.com/products/red-sneakers-123"

# Extract the product name using a regular expression
product_name = re.search(r"/([^/]+)/?$", url).group(1)

print(product_name) # Output: "red-sneakers-123"

In this example, the URL is for a product page on an imaginary website called https://yourdigitalteam.com. The product name appears in the URL after the "/products/" segment and before any query parameters (if present).

The regular expression pattern used in the re.search() function extracts the text between the last forward slash and the end of the URL. The group(1) method returns the captured text as a string.

Note that this is just one example of how to extract product names from URLs, and the approach may need to be modified for different website and URL structures.
