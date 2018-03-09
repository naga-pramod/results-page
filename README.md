# results-page
Scraping Results data from the results page 



<from selenium import webdriver
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.support.ui import Select

browser = webdriver.Firefox()
#The results page's url is used we are going to access it directly
browser.get("https://doeresults.gitam.edu/onlineresults/pages/newgrdcrdinput1.aspx")
semester_choose = browser.find_element_by_xpath("/html/body/form/table/tbody/tr[3]/td/table/tbody/tr/td/table/tbody/tr/td/table/tbody/tr[2]/td[2]/table/tbody/tr[2]/td[3]/select/option[2]").click()
regnumber = browser.find_element_by_name("txtreg")
regnumber.clear()
regnumber.send_keys("1210316011")
regnumber.send_keys(Keys.RETURN)> 

