//xpath with 'and', 'or' operators
		//and --> Both attribute should be correct or true
		driver.findElement(By.xpath("//input[@type='text' and @name='filter_search']")).sendKeys(" Test2");
		//or --> atleast one attribute should be true or correct
		driver.findElement(By.xpath("//input[@type='text' or @name='Anish']")).sendKeys(" Test3");


// XPath with inner text using text()

// Syntax:
// //tagname[text()='value']

// Example:
driver.findElement(By.xpath("//a[text()='Marketplaces']")).click();

// Notes:
// 1. text() is used to locate elements based on their visible text (inner text).
// 2. text() cannot be used for input fields because <input> elements do not have inner text.
//    Their values are stored in attributes such as value, placeholder, name, etc.
// 3. Link text is the visible text of an <a> (anchor) tag.
// 4. Every LinkText is an inner text, but every inner text is not a LinkText.
