# Vuex - State Management

* Replacing provide/ inject with data that you want to share across multiple components. 
* Understanding & Using Vuex

## What is “Vuex?”

A library for managing global state

State -> Data that your component needs (Reactive data that may change/ trigger on the screen) 

Differentiate between local state and global state. 

**Local State:**

* Affects one component. 
* E.g. entered user input, show/ hide container

**Global State:**

* Affects multiple components/ entire app
* E.g. user auth status, shopping cart items

Global state is where Vuex can help us. 

Managing app-wide/ global state can be difficult.

With Vuex - outsourced state management, with predictable management flo, clearly defined data flow. 

____

## To Run

``npm i``

``npm run serve``

``npm install --save vuex``
____

## Learnings 

* main.js import createStore and initialise Store

<img src="images/createStore.png" width=500 />

* add store to App.vue - format is used as $store.state 

<img src="images/store.state.counter.png" width=500 />

<img src="images/counter1.png" with=500 />

The above image now has a counter. The button does nothing... yet. 

* added methods, computer to increment the counter. 

<img src="images/counterButton.png" width=500 />

<img src="images/addsOne.png" width=500 />

## Mutations in Vuex

Mutations takes an object and can define the methods. 

<img src="images/mutations.png" width=500 />

* add mutations to the main.js file. From this one file, you can change the state across the app in multiple locations. 

* can have multiple mutations for your app. 

* to use the mutation, add it to the methods using this.$store.commit() method.
Inside the commit method use the name of your mutation as a string. In this case the name is 'increment'

<img src="images/updateMutation.png" width=500 />

The logic now has update two counter. Button name reflects this. Using a mutation across the two different button components. 

<img src="images/addTwo.png" width=500 />

Added Auth

<img src="images/auth.png" width=500 />

Completed exercise

<img src="images/final.png" width=500 />

* additional component - UserAuth.vue
* store folder, includes modules and counter  


## Resources

Practice is from Udemy course by Maximilian Schwarzmüller. Vue - The Complete Guide. 