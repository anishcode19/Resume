//xpath with 'and', 'or' operators
		//and --> Both attribute should be correct or true
		driver.findElement(By.xpath("//input[@type='text' and @name='filter_search']")).sendKeys(" Test2");
		//or --> atleast one attribute should be true or correct
		driver.findElement(By.xpath("//input[@type='text' or @name='Anish']")).sendKeys(" Test3");
