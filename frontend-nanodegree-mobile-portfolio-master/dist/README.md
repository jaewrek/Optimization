frontend-nanodegree-website-optimization
===============================

# Website Optimization Project
by Jerrik

## Descritpion
Optimizing the CRP in the HTML and editing Javascript to reach above 90 on PageSpeed Insights and secure greater than 60FPS while browsing the site.

## Install
You will need to host this page. I have done so through Python and Ngrok, using the resulting URL for analysis in PageSpeed Insights
    `python -m SimpleHttpServer 8080`
    `./ngrok http 8080`

## Contributions
Open source, feel free to make additions/optmizations.

## Extra Notes for Grader
I completely inlined both CSS files (style and bootstrap) into Header tags of HTML removing 2 critical rendering paths.
I deferred/asynced all JS scripts.
I declared a separate variable for document.body.scrollTop so it is not executed every iteration of the for loop.
I changed the call to `querySelectorAll('.mover')` to `getElementsbyClass('mover')`.
I minified all html/css/js files.
I compressed all pictures.
I used a picture element in pizza.html to use a smaller dimension picture for mobile viewports.
And I changed the maximum for the for loop from 200 to 35 as this still renders all the pizzas on the page and 200 was certainly too much!


I hosted my page through Python and Ngrok then used that URL for PageSpeed Insights.

## License
MIT License

Copyright (c) 2016 Jerrik Neri

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
