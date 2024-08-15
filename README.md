# Easy selenium automation

**Easy selenium automation** is a simple Python library that simplifies Selenium automations by providing utility functions for common tasks like waiting for elements, clicking, and filling fields.

## Installation

You can install the package via pip:

```bash
pip install easy-selenium-automation
```

**Usage**
- Here is an example of how to use


from easy-selenium-automation.selenium_utils import wait_element_xpath, click_element_xpath

# Example usage in Selenium
driver = webdriver.Chrome()

# Wait for an element to be present and click on it
element = wait_element_xpath(driver, "//div[@id='example']", 10)
if element:
    click_element_xpath(driver, "//div[@id='example']", 10)

driver.quit()

## Functions
- wait_element_xpath(driver, xpath, timeout=10): Waits for an element to be present in the DOM by XPath.
- wait_element_id(driver, element_id, timeout=10): Waits for an element to be present in the DOM by ID.
- wait_element_name(driver, name, timeout=10): Waits for an element to be present in the DOM by Name.
- wait_element_class(driver, class_name, timeout=10): Waits for an element to be present in the DOM by Class Name.
- wait_element_tag(driver, tag_name, timeout=10): Waits for an element to be present in the DOM by Tag Name.
- wait_element_css(driver, css_selector, timeout=10): Waits for an element to be present in the DOM by CSS Selector.
- wait_element_link_text(driver, link_text, timeout=10): Waits for an element to be present in the DOM by Link Text.
- click_element_xpath(driver, xpath, timeout=10): Waits for an element identified by XPath and clicks on it.
- click_element_css(driver, css_selector, timeout=10): Waits for an element identified by CSS Selector and clicks on it.
- fill_field_xpath(driver, xpath, text, timeout=10): Waits for an element identified by XPath and fills it with text.
- fill_field_name(driver, name, text, timeout=10): Waits for an element identified by Name and fills it with text.
- is_element_present_xpath(driver, xpath, timeout=10): Checks if an element is present in the DOM by XPath.
- is_element_present_css(driver, css_selector, timeout=10): Checks if an element is present in the DOM by CSS Selector.
- is_element_present_id(driver, element_id, timeout=10): Checks if an element is present in the DOM by ID.
- is_element_present_name(driver, name, timeout=10): Checks if an element is present in the DOM by Name.
- is_element_present_class(driver, class_name, timeout=10): Checks if an element is present in the DOM by Class Name.


**License**
- This project is licensed under the MIT License - see the LICENSE file for details.