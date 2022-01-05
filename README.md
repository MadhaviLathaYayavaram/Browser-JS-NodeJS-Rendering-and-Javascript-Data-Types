# (Browser-JS-NodeJS-Rendering-and-Javascript-Data-Types)

# Browser JS(console) v Nodejs

## Browser Js

A web browser uses javascript as the programming language to render the code and display the results. It is easy to build web pages using browser understandable script language and HyperText Markup Language. 

A programmer can deal with only Javascript to develop front-end applications. We can interact with DOM and other web API applications through Browser JS. ES 6-7-8-9 versions code of javascript can be written to get it understandable by modern browsers and also by NodeJS.

We have a limited access to the system resources because the javascript is covered with safety encapsulations. We cannot handle the backend server through browser, it needs another support system for that. 

The rendering machine of browser manipulates code, divide it into trees, parses and print the output on web page. Browser code uses import() to include other coding modules and enhance the execution. 


## Node JS

NodeJS is a runtime-based javascript on a V8 engine, basically hailed from Chrome, and runs on all platforms. It uses a single thread and event queue to run javascript code. 
Users can have complete access to the system resources through javascript so that, it is a supporting tool for web development for server-side applications. 

A programmer can handle both front-end and back-end code in NodeJS which can be further combined and rendered through the browser with more efficiency. It is advantageous for both client and server applications. Document and window will not be available here to handle, which can only be done by Browser JS.

A great advantage of NodeJS is that we can access the whole file system from a server and manage the whole database. We can control the server environment and the frontend at the same time. A programmer can control the users and specify which browsers to use for the applications. 

Uses require() function to insert required modules and run the program. NodeJS creates a package of different types of software utilities which are understandable by browsers and rendering machines. 


_______________________________________________________________________________________________________________________________________________________________________

# Javascript Code:


 The typeof operator returns a string indicating the type of the unevaluated operand. it requires an object or primitive data to check and returns its type. 

- typeof(1)	- Output : ‘Number’.          Identifies integers, decimals, Math() and Number() parameters are identified as a number data type.

- typeof(1.1)	- Output : ‘Number’.        As 1.1 is a decimal, it is taken as the 'number' data type in Javascript.

- typeof('1.1')	- Output : ‘String’.      Even though 1.1 is a decimal value, it is treated as a 'String' data type if it is given in quotes. Strings in double quotes, String() parameters are treated as strings. 

- typeof(true)	- Output : ‘Boolean’.     True, false Boolean(), and !() operators are treated as boolean data types in Javascript.

- typeof(null)	- Output : ‘Object’.      Null is an object in Javascript since it's earlier versions.

- typeof(undefined)	- Output : ‘Undefined’.   Undefined is an independent object (data type) in Javascript.

- typeof([])	- Output : ‘Object’.        Square brackets are recognized as an independent object, because an array contains independent mixed data of different data types which is enclosed by square brackets.

- typeof({})	- Output : ‘Object’.        Whatever code that is given in the flower brackets / parenthesis are treated as a separate group of coding statements that returns a single output finally, which is an object itself. 

- typeof(NaN)	- Output : ‘Number’.        Not-A-Number is an object of number datatype. 


Other data types include Bigint, Symbol, and function.







_____________________________________________________________________________________________________________________________________________________________________

# Summary of the Video:  https://www.youtube.com/watch?v=SmE4OwHztCc

The concepts covered : 
Render a website
Binding
Rendering: parsing, layout, print, etc.
Javascript virtual machine

- Steps that include after page load. 
Parsing ->  DomTree -> Render Tree (4 trees) -> The computation of the position of the Node -> Painting computes the bitmaps and composites to the screen.

- Parse HTML, parse CSS, and JS: Both the data structures are rendered together with a layout and printed on the browser.

- HTML will not stop the execution of the web page for simple errors because the parser is not that strict to cease the output. The browser actually tries to accept the code in positive and automatically adds extra code such as <html> tag.

- Tokenizer helps to parse the tags as tokens to complete the code and send it to the parser.
Parse Tree checks for all the elements for open and close tags of HTML code and also a DOM tree.

- <script>, <link>, and <style> tags from the code halt the parser and slow the rendering process. Speculative parsing is done in order to look ahead for external images, scripts, and CSS. The stylesheets fetch the necessary information and finish the parsing process. 

- The parsing process can also be interrupted through the Reetrant process. Render tree handles multiple objects such as RenderObjects, RenderStyles, Lineboxes, and RenderLayers. 

- The recursive process will be done finally to form batch layouts. Modern JS frameworks do internal fastDOM and prevent internal Layout Thrashing. Finally, the ‘Paint’ process will be done using canvas API after completing the render process. All the render trees will be processed which further creates layers and build up the output through 12 phases.

