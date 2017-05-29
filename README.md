1. SETUP 

1.1 First you need to download all the files. You can do this manually by clicking on "Clone or download" > "Download Zip". You can also clone the files with GitHub, refer to https://help.github.com/articles/cloning-a-repository/ for more information.

1.2 After you have downloaded all the files, you can run this website by opening index.html with a browser.

1.3 How to use google PageSpeed Insights:

1.3.1 First download python3 and ngrok

1.3.2 Open your terminal(Windows: windows key + r, type in cmd and accept. Linux: ctrl+alt+t)

1.3.3 Change directory to the current directory of your downloaded files(cd C:\"your_directory"\)

1.3.5 Enter "python -m http.server 8080" for a local host

1.3.6 Place your ngrok.exe file in the same directory, execute it and a terminal tab will open. Enter "ngrok.exe http 8080"

1.3.7 Copy the website that appears in your terminal(http://******.ngrok.io for example) and paste in https://developers.google.com/speed/pagespeed/insights 

2. Optimizations
2.1 index.html
- Optimized/deleted js/css files that provoked render blocking
- Minified css and js
- Compressed images

2.2 main.js (pizza.html)
- resizePizzas function: Refactored code and removed determineDx.
- updatePositions function: Phase value moved out of main loop so that there are not repeated calculations and moved items variable out of the function.
- Fixed number of moving pizzas based on the screen.