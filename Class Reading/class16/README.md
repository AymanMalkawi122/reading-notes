
# Class 16

## Reading  Questions

### 1. What are the key differences between scraping static and dynamic websites?

***Static websites:*** Static websites have fixed ```HTML``` content that is already present in the source code. When you request a page from a static website, the server simply sends the pre-built ```HTML``` file to your browser. The content of a static website remains the same until it is manually updated. Scraping a static website involves parsing the ```HTML``` structure and extracting the desired data using techniques like web scraping libraries or regular expressions.

***Dynamic websites:*** Dynamic websites, on the other hand, generate content dynamically in response to user interactions or database queries. The server processes the user's request and generates ```HTML``` content on the fly. This means that the ```HTML``` structure of a dynamic website may change based on the user's actions or other factors. Scraping a dynamic website often requires more advanced techniques, such as using headless browsers or making requests to APIs that provide the required data.

### 2. Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites

1. Respectful Crawling: To avoid overwhelming a website's server and being flagged as a bot, it's crucial to practice respectful crawling. This involves setting a reasonable crawl rate by adding delays between requests and adhering to any rules specified in the website's robots.txt file. By simulating human-like behavior and avoiding excessive requests, you can minimize the risk of being blocked.

2. User-Agent Rotation: Websites often track user agents to identify automated bots. By rotating the User-Agent header in your requests, you can make your scraping requests appear more like regular user traffic. Using a variety of user agents and occasionally mimicking popular web browsers can help you fly under the radar and avoid detection.

3. Proxy Rotation: Employing a pool of proxies can help distribute your requests across different IP addresses, making it harder for websites to track and block your scraping activity. By rotating proxies, you can avoid hitting rate limits, prevent IP blocking, and maintain a level of anonymity. It's essential to use reputable proxy providers and ensure that your code is configured correctly to handle proxy rotation seamlessly.

### 3. What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial

* Playwright simplifies web scraping by providing a powerful and user-friendly interface to automate browser actions. Its cross-browser compatibility and support for dynamic web pages make it a valuable tool for scraping tasks that require interacting with JavaScript-heavy websites and extracting data efficiently.

* A use case where Playwright can be particularly beneficial is scraping dynamic web pages that heavily rely on JavaScript. Traditional scraping approaches may struggle to handle dynamic content, but Playwright's ability to execute JavaScript and interact with the page's elements makes it well-suited for such tasks.

### 4. Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage

* ```XPath``` is a powerful querying language used in web scraping to navigate and extract data from ```HTML``` and ```XML``` documents. It allows you to locate specific elements within the document structure based on their tag name, attributes, or their position in the hierarchy.

* Let's consider an example where we want to extract the titles of all the articles listed on a news website. Assume that the article titles are contained within ```<H2>``` tags with a class attribute of "article-title". Here's an XPath expression to select those elements:

### ***Example***

```python
//h2[@class='article-title']
```
