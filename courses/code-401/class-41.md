# Reading 41 Notes

## getting started with react native

### Name three Core Components of React Native and describe what they do

`<View>`

flex container with touch handling, style, accessibility controls

`<Text>`

displays strings and handles touch events

`<Image>`

### What problem does React Native solve (why call it native)?

allows mobile apps to look and feel like they were written in mobile OS native language, but are actually written in Javascript/React

the React Native rendering engine converts the app to mobile OS views

android Kotlin/Java

iOS Objective C/Swift

### What are the building blocks of a React Native app? How does that compare to a React app?

The building block of a mobile app is a "view"

A React native "view" is one of the core component

## expo

### What solution does expo provide?

Expo allows you to write a mobile app in Javascript/Typescript and publish it to the mobile app stores (android/IOS)

### Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow

managed

### What is the difference between React Native and Expo?

expo is a framework for building with React Native, it builds upon React Native which is the library

## expo snack

### Checkout this tool. What does snack allow you to do?

snack is a like a REPLIT for react native apps

## ejecting

### What does “eject” mean within the context of Expo?

eject means leaving the Expo development environment

### When should you not eject?

if you don't know what you are doing WRT to build configuration or native code

### Why might you choose to eject?

if your project needs to go in a direction that would require the "bare workflow"

NOTE "ejecting" as a concept is deprecated in Expo per the docs
