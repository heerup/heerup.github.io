---
layout: post
title:  "Converting a vue.js app to typescript"
---

# Converting a vue.js app to typescript

I have now had the pleasure multiple times of finding myself unexpectedly working on a vue.js app.
I am a fan of strongly typed programming languages and most at home in C#, so working in javascript puts an extra load on my brain that I am used to offloading to the compiler/IDE.
That is why I usually cant work a day or two in a vue.js app before I start fantasizing about converting it to typescript.

A prerequisite for this is of course the type declarations from the vue library. Luckily they are included: https://vuejs.org/v2/guide/typescript.html

So I add the tsconfig.json file and install+run the typescript compiler.
Nothing happends. I get as far as configuring the typescript compiler to "compile" all of my .js files to ... .js files.

**I should say im not a frontend developer, hence this whole project**

I figure I need to find another approach. I google som more and find out this whole procedure is not only documented.
Someone put it in a script/plugin that I can use just by running `vue add typescript` in the commandline.
See more here: https://cli.vuejs.org/core-plugins/typescript.html 


After running the typescript conversion I have to run the application with `yarn serve` and it seems to have taken over my main page with a standard vue+ts page.
![Welcome to Your Vue.js + TypeScript App](assets/VueTS.PNG)


I think I have to revert only some of the changes to the App.vue file to make it work.
