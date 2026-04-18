from selenium import webdriver from selenium.webdriver.common.by import By from selenium.webdriver.common.keys import Keys import time

#Initialize the Chrome driver (make sure you have chromedriver installed) driver webdriver. Edge()

#Open Google homepage driver.get("https://www.google.com") time.sleep(300)

#Maximize window driver maximize_window()

#Test 1: Check if the search box is present search box driver.find_element(By.NAME, "q") #Test 2: Enter a query and submit search_box.send_keys("Selenium WebDriver")

search_box.send_keys (Keys. RETURN)

time.sleep(3000) # wait for results to load

search_button-driver.find element(By.NAME, "btnk") apps_button-driver.find element(By.CLASS_NAME, "gb_D")

sign_in_button-driver.find_element(By.1LINK_TEXT, "sign.in")

footer links-drivr.find_elements (By.TAG NAME, "a")

for link in footer links: print(link, text,"->",link.get_attribute("href"))

driver.quit()
from selenium import webdriver from selenium.webdriver.common.by import By from selenium.webdriver.common.keys import Keys import time

#Initialize the browser driver webdriver.Chrome()

#Open the login page of your target site driver.get("https://facebook.com/login") time.sleep(15)

#Find the username and password fields

username_box = driver.find_element(By.NAME, "username") password_box = driver.find_element(By.NAME, "password")

#Enter credentials

username_box.send_keys("your_username")

password_box.send_keys("your_password")

#Submit the form

password_box.send_keys(Keys.RETURN)

#Wait for a while to see the result time.sleep(300)

#Close the browser driver.quit()Create a Simple HTML File
Open a text editor and create a new file named index.html.
Add the following HTML content:
<!DOCTYPE html>
<html>
<head>
    <title>Hello, World!</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>FROM nginx:latest

# Copy the HTML file to the Nginx default directory
COPY index.html /usr/share/nginx/html/index.html

# Expose port 80
EXPOSE 80FROM alpine:latest

# Install Nano text editor
RUN apk add --no-cache nano

# Set the default command to launch a shell
CMD ["/bin/sh"]
Save and close the file.
