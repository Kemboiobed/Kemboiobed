from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.chrome.service import Service
from selenium.webdriver.chrome.options import Options
import time

# Set up Chrome options
chrome_options = Options()
chrome_options.add_argument("--user-data-dir=./User_Data")  # Keep user data to avoid scanning QR code every time

# Path to your ChromeDriver
chrome_driver_path = 'path/to/chromedriver'

# Initialize the WebDriver
service = Service(chrome_driver_path)
driver = webdriver.Chrome(service=service, options=chrome_options)

# Open WhatsApp Web
driver.get('https://web.whatsapp.com')

# Wait for the user to scan the QR code
input("Press Enter after scanning the QR code")

# List of contacts to monitor
contacts = ["Contact Name 1", "Contact Name 2"]

def check_status(contact):
    try:
        # Search for the contact
        search_box = driver.find_element(By.XPATH, '//div[@contenteditable="true"][@data-tab="3"]')
        search_box.clear()
        search_box.send_keys(contact)
        search_box.send_keys(Keys.ENTER)
        time.sleep(2)

        # Check the status
        status = driver.find_element(By.XPATH, '//span[@title="online"]')
        if status:
            print(f"{contact} is online")
        else:
            print(f"{contact} is offline")
    except Exception as e:
    
