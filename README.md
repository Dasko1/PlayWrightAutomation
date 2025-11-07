# ReadMe

## Open a browser to "https://rahulshettyacademy.com/loginpagePractise/"
// "require" = import, so call specifically 'test' from '@playwright. Wrap it in the const-type variable 'test' 
const {test, expect} = require('@playwright/test');

// Use test with 2 arguments: the first one being an annotation, the second declares the program asynchronous and creates a 'page' instance from 'test' in l.1.
test('@Web UI Controls', async ({page})=>

// 'await' tells the line to wait for the line to complete before going on to the next. This is what 'asynchronous' does!
await page.goto('https://rahulshettyacademy.com/loginpagePractise/');

// Wait for a few seconds to visually confirm the page loaded
await page.waitForTimeout(3000);

// Close the browser after the test
await browser.close();

});
