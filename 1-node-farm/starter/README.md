### Lecture 1:

---

Let's do a high-level overview of what NodeJS actually is, what we use it for, and why we use Node instead of other technologies.

So, the official definition is that NodeJS is a JavaScript Runtime built on Google's open-source V8 JavaScript engine. Now, what does that actually mean?

Well, let's start by trying to understand what the JavaScript Runtime and the V8 engine actually are.

So, you have probably already used JavaScript before and it was probably always just inside a browser, right? Because any browser natively understands HTML, CSS, and JavaScript, and no matter if you write vanilla JavaScript or some JavaScript framework like React or Angular code, that's all just JavaScript that gets executed right in the browser. So, in this case, the browser is then the JavaScript Runtime.

But, what if we could take JavaScript out of the browser and simply execute our JavaScript code somewhere else without all the restrictions that we have in the browser? Well, it turns out that we actually can. And the solution for this, as you can guess, is called NodeJS, and so Node JS is just another JavaScript Runtime. It's just like a container, like an environment, in which a program written in JavaScript can be executed, but outside of any browser whatsoever. All right, it's actually a bit more complex than this, of course, but for now, this is enough.

Now, who actually does execute the code if not the browser? And that's where the V8 engine developed by Google comes into play. Because that is exactly where JavaScript code will be parsed and run in NodeJS, okay?

So, I hope that now the definition of NodeJS being a JavaScript Runtime on the V8 JavaScript engine makes a lot more sense, and again, this is just a very high-level overview of what Node is and how it works.

We are gonna go into a lot of detail about how Node really works behind the scenes right in the next section, but at this point, I just want you to get a quick overview so that you can start learning the fundamentals of NodeJS in practice throughout this section.

Anyway, now that we have JavaScript outside of the browser in a kind of standalone environment which just NodeJS, we can do so many more things with JavaScript that were completely impossible before like accessing the file system, or better networking capabilities are not possible with NodeJS, and all these factors together give us the perfect conditions for using NodeJS as a web server, meaning that now we can finally use JavaScript on the server side of web development in order to build fast, highly scalable network applications for powering the back-end of websites or web applications.

And this is absolutely fantastic and game-changing for web development.

So, let's now take a look at some use cases for Node and why it's such a great fit for back-end development.

And the first thing that we need to talk about is the fact that Node applications are so fast and so scalable because NodeJS is single-threaded based on an event-driven, non-blocking I/O model which makes NodeJS very lightweight and efficient.

Now, that, of course, sounds super complicated, I know, but once more we're gonna talk about exactly what all of this means a little late in the course. But, for now, just keep in mind that Node is perfect for building super fast, and scalable data-intensive web applications.

And that makes NodeJS a perfect fit for building all different kinds of applications like building an API with a database behind it and preferably a non-relational NoSQL database like MongoDB, and this is actually exactly what we're gonna do later in this course as we dive deeper and deeper into NodeJS.

But, there is, of course, all sorts of other apps that we can build like data streaming applications such as YouTube or Netflix, real-time chat apps, or even server-side web applications where the entire content is simply generated right on the server, so as you see, the possibilities really are endless.

But, there is actually, also, a type of apps that we should not build with Node. And this is when our app needs some super heavy server-side processing like having image manipulations, video conversion, file compression or anything like that, all right.

And you will learn why that is once we dive deeper into how Node actually works.

So, in this case, we're better off using something like Ruby on Rails, PHP, or Python.

Because NodeJS just wasn't developed for these use cases and although there are solutions for dealing with them, we should always use the right tool for the task at hand.

Okay, so these are the types of applications that we can and cannot build using NodeJS.

And if you choose to use Node, well, then you are in good company because many top companies like Netflix, Uber, PayPal, eBay, and many more have already started using NodeJS which really proves that the technology is stable enough at this point to be used in production.

Now, of course there are more reasons for using Node, and the biggest one is probably that using the same language across your entire stack both on the front-end and the back-end is a lot easier for you or for your team.

First, you don't have to learn a new programming language for building your back-end and, also, you don't have to keep switching back and forth between languages which will make the entire building process faster and more efficient.

Believe me, it's really amazing to be able to use JavaScript to build your entire application from start to finish. It's absolutely fantastic really.

And another great reason for using Node is that there is a huge library of open-source packages or modules, as we can also call them, available for everyone for free. It's called NPM and you've probably heard of it or even used it already.

And, of course, we're also gonna start using packages right in this section.

And, finally, it's also good to know that there is a huge active community of Node developers out there that are constantly improving NodeJS and helping beginners like you.

And, so you can really rely on the technology for all your projects in the years to come.

Okay, so that was a very brief intro and overview of NodeJS and some of its use cases.

So, for the rest of this section, we will now use Node to create a very simple web server and build an extremely simple API, so that you can get familiar with the basic principles of Node development.
