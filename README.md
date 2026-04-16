"my git repositary" 
import selenium
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



git init
echo "# My Git Repository" > README.md
git add README.md
git commit -m "Initial commit"
git remote add origin https://github.com/username/repository.git
git branch -M master
git push -u origin master
type nul > 1.txt
type nul > 2.txt
git add .
git commit -m "Added files"
git push
git checkout -b MITS
git push -u origin MITS
git checkout master
git checkout MITS
git status
git branch
git log --oneline
