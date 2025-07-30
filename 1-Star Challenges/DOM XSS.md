<img width="478" height="196" alt="image" src="https://github.com/user-attachments/assets/24c853c6-dfdb-4d26-a216-b3fc96e950bd" />

# DOM XSS (Document Object Model Cross-Site Scripting)
So now the first challenge is about Cross-Site Scripting(XSS), specifically **DOM XSS** which is a type of XSS that runs the script entirely on the client side 

We can also see that the script for our XSS attack has been given by the challenge :
`<iframe src="javascript:alert(`xss`)">`

~> When this is rendered as HTML, it creates an `<iframe>` element which will be a pop up box on the current page
that runs the JavaScript `alert('xss')`.

After getting to know what the challenge wants, now we just need to find a way to get the payload to execute as html code


# Find ways to manipulate URL
Since we are working with XSS, my first instinct was to look for ways to maniuplate the URL
At first, I tried to insert the payload directly into the URL path to see if the application would execute it.

<img width="1594" height="175" alt="image" src="https://github.com/user-attachments/assets/2ca81433-8003-48e6-929e-b1030876f2f6" /> <br/><br/>

No luck as it just returns us to the previous URL when we press enter.

Seeing this, I tried to find elements of the UI that could potentially let me manipulate the URL.

<img width="1597" height="163" alt="image" src="https://github.com/user-attachments/assets/803b71a1-878c-4e02-bec7-51583d65fded" /> <br/><br/>

Here I discovered that the search element on the top right of the page lets us potentially craft a payload on to the URL bar

Knowing this, I copied the payload into the search bar and pressed enter

<img width="1601" height="840" alt="image" src="https://github.com/user-attachments/assets/bff03a0a-3a49-4475-a432-ddb9b6986780" /> <br/><br/>

Success!! Due to improper input sanitization, the web app processed the search bar input directly into the DOM, allowing the XSS payload to execute.

This reveals the dangers of improper input sanitization, as it allows attackers to inject and execute scripts, potentially leading to session hijacking, data theft, or full account compromise. For this reason, Developers should always be careful and validate, sanitize, and properly encode all user inputs, especially when inserting them into the DOM, to prevent vulnerabilities like DOM-based XSS.









