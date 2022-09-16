# pagerank_p4e
This project develops a page ranking system for a given website. The purpose of this project is to emulate the functioning of a search engine

There are 3 key components to this project

1)	Web Crawling
2)	Index Building 
3)	Visualising

The data retrieved from the web will be stored in an SQLite3 database.

<ins>Web Crawling</ins>

A web crawler is an automated program that crawls through the web. A common application could be storing a copy of visited pages and indexing them (or rank them) in order to build a search engine which provides optimal results.

Here are the steps involved in this process:

-	Retrieve a page.
-	Look through the page for links.
-	Add the links in a queue of “to be retrieved”
-	Repeat the process with the sites in the queue.
-	
There are things accounted for in a real-world application. This is a simple application that will not account for:

-	A selection policy for which pages to download
-	A re-visit policy to see when to check for updates on a page
-	A politeness policy to see how to avoid overloading Web sites
-	A parallelization policy that states how to coordinate distributed web crawlers.

Another component is to check for robots.txt of the website to check for disallowed pages. 

<ins>Index Building</ins>

Search Engine collects parses and stores data to facilitate fast and accurate information retrieval. Based on keywords and links in a page, it develops a ranking system in order to render relevant pages when a something is searched, as opposed to searching every document one by one per search.

<ins>Visualisation</ins>
For the purpose of this project, we will simply visualise the ranks for each page using JavaScript’s D3 library. 
