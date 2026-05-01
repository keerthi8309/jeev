1)from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time
driver = webdriver.Edge()
driver.get("https://www.google.com")
time.sleep(2)
search_box = driver.find_element(By.NAME, "q")
search_box.send_keys("YouTube")
search_box.send_keys(Keys.RETURN)
time.sleep(5)
driver.quit()



2)import selenium
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time
driver=webdriver.Edge()
driver.get("https://facebook.com")
time.sleep(2)
element=driver.find_element(By.TAG_NAME,"h1")
print(element.txt)
driver.quit()



3)from selenium import webdriver
from selenium.webdriver.common.by import By
driver = webdriver.Edge()
driver.get("https://www.google.com")
print("Title:", driver.title)
print("Search box:", driver.find_element(By.NAME, "q").is_displayed())
print("Buttons:", len(driver.find_elements(By.NAME, "btnK")))
print("Links:", len(driver.find_elements(By.TAG_NAME, "a")))
driver.quit()
