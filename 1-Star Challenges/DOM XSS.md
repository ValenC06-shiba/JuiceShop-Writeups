<img width="478" height="196" alt="image" src="https://github.com/user-attachments/assets/24c853c6-dfdb-4d26-a216-b3fc96e950bd" />

# DOM XSS (Document Object Model Cross-Site Scripting)
So now the first challenge is about Cross-Site Scripting(XSS), specifically **DOM XSS** which is a type of XSS that runs the script entirely on the client side 

We can also see that the script for our XSS attack has been given by the challenge :
`<iframe src="javascript:alert(`xss`)">`

~> When this is rendered as HTML, it creates an `<iframe>` element which will be a pop up box on the current page
that runs the JavaScript `alert('xss')`.

After getting to know what the challenge wants, now we just need to find a way to get the payload to run as html code
