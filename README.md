------------------------------------------Video-1-------------------------------------
In this video i learned basic things about React:-

Why we use react?
=>makes easy to manage and build complex front end
=>used to make single-page applications 

Why was React created?
-facebook met with a problem of phantom messages
phantom messages typically refer to notifications or alerts indicating the presence of a new message, even when there is no actual new message.

facebook me you can chat with people from 3 different options . ab hota kya tha ki agr mne chatbox se message pdhliya fir bhi message ka notification count(jse ki 1,2,3) hat ta nhi tha ye thi problem , ki agr mne message pdh liya hai toh upar q count likha aa rha hai?

ab hota kya tha ki state ( variable ki state ki vha pr 1 dikhana hai ki 5 ) was managed by javascript and UI was managed by DOM ,toh js aur UI me koi sync hi nhi tha ki js DOM ko bta paye ki 1 bhi message nhi hai toh UI m kuch mat show kro. is dikkt k krn occur hoti thi phantom message ki dikkt ki message na hote sote bhi notification count dikhta tha.

ye problem of INCONSISTENT UI ko solve krne k liye bna react in 2011 by facebook team 
The development of React started as an internal project by Jordan Walke, a software engineer at Facebook, in 2011.

React was then open-sourced by Facebook in May 2013
 
then khan academy and unsplash adopted React

consistency of React made it popular 

React is a library 

library vs framework?

library:- A library is a collection of pre-written code that developers can use to optimize tasks. It provides specific functionality and is typically focused on a particular area or task
(COOL DUDE)
Control: You are in control of the application. You decide when and where to call the library.

eg:-React JS , GSAP , FRAMER MOTION , bootstrap , sheryJS

framework:-A framework is a comprehensive platform for building software applications. It provides a foundation and predefined structure that developers follow, enforcing a certain way to build and organize code.

Control: The framework is in control of the application's flow. It dictates the architecture and flow of the application.
(MILITARY -strict rules)
eg:- Next JS , Angular

--------------------------------------Video-2-----------------------------------------
Pre-requisites
node.js- is used to execute javascript
code editor - to write code

if we want to use react without a framework or as a library we use bundlers like:-
vite or parcel
bundlers combines our code from multiple files and gives a single file

*react is core foundational library*

react-dom = implemantation of react on  web
react-native = implemantation of react on  mobile apps 

-------------------------------ways to create react projects--------------------------
1:-CRA                                               2:-using VITE

-----------------------------comparison of both --------------------------------------
1:- create react app (npx create react app)

-  we dont use this method very often because because this is a bulky utility which has big package size thus takes too much time to install things which arent even neccesary , so we use another method i.e through vite

-  in package.json  you will find extra testing libraries which we dont need 
project chalane k liye look for 'start scripts'

- to start the project use "npm run start"

------react flow and structure--------

index.html - yhi main page hai jo laod hoga aur ye ek hi page hai isliye single page application bnti hai react se , sara kaam isi k andr hota hai .

noscript tag :- message deta hai ki agr kisi browser m js enable nhi hai toh krdo

div root = 


2:- npm create vite@latest :- lightweight utility
a:-npm run dev
-only main libraries are provided to us by vite which are react and react-dom
-many dev dependencies are provided which are used only during development and not served while production qki inse sirf kaam hota hai 








-------------------------------------------------------------------------------------
now to understand any project we open package.json as it is a entry point where everything is defined 

scripts are the one responsible for running a project and makes application ready for production 

bulid - jab production m jaati hai application tab build folder hi serve kiya jaata hai users ko na ki source folder 

linting(esLint) -  every dveloper has his/her own writting style so when many people are working on a single project eslint helps us to set some rules which are to be followed while writting code or ortherwise error will come . this helps to bring uniformity in the code.

browser list defines :- kon se browser pr project chalega ki nahi. which browser is supported 

node modules - package.json file ki jitni bhi dependencies install hone k baad yha dikhti hai

gitignore - jo files git pr push nhi krni hai

package.lock json - package.json ki trh hi hai bas yha pr dependencies lock ho jaati hai ki isi version pr chlegi.stable version lock krdia jata hai 

DOM ek tree structure hai 
browser k paas khudka DOM hota hai
react khudka DOM bnata hai which is known as virtual DOM

ab ye virtual DOM khudko main DOM se compare krta hai aur sirf voi changes krta hai jinki zrurat hai(diffing algo)

DOM ka 1 method hai createRoot

react has the power of JSX 
JSX
- javascript syntax extension  , java script and xml (to write js in html)
- used to make user defined tags

so we made <app/> as a custom tag

ReactDOM.createRoot(document.getElementById('root')).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
)

what does this line do?



