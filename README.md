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

Can text() be used for input fields?

Answer: No. text() works only for elements that contain visible text between opening and closing tags. Input fields do not have inner text; their data is stored in attributes such as value, name, or placeholder.
<img width="995" height="440" alt="image" src="https://github.com/user-attachments/assets/2ddb4231-282d-4a6b-ac1f-5cae690bae87" />

//xpath with partial Text --> contains()
		// //tagname[contains(@attribute,'partialValue')]
		//The contains() function takes two arguments separated by a comma:
		//contains() is used when the attribute value is dynamic or only partially known. It performs a partial match.
		driver.findElement(By.xpath("//input[contains(@placeholder, 'lastname')]")).sendKeys("Kuar");

