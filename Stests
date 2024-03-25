from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time

# Create an instance of WebDriver (Chrome, Firefox, etc.)
driver = webdriver.Chrome()

# Maximize the browser window
driver.maximize_window()

# Navigate to the website under test
driver.get("https://www.example.com")

# Wait for the page to load (you can use more sophisticated waits)
time.sleep(2)

# Find the search input element by its name attribute
search_input = driver.find_element(By.NAME, "q")

# Enter a search query
search_input.send_keys("Hello World")

# Submit the search query
search_input.submit()

# Wait for search results to load
time.sleep(2)

# Verify if the search results page title contains the search query
assert "Hello World" in driver.title

# Print the page title
print("Page title:", driver.title)

# Close the browser window
driver.quit()
