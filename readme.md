# Building Your Resume Like a Boss with CI

![BuildStatus](https://travis-ci.org/sedouard/resume.svg?branch=master)

## Introduction

If you're a developer geek like I am, you'll want to check this out. This repository builds my resume using continuous integration. Seriously! You can find the live resume **[here](http://resume.stevenedouard.com)**.

What other way can you show you know the agile development lifecycle by expressing it through your resume itself. It's just a few easy steps.

Here you'll find all you need to deploy and create your own resume. We are using the nifty [resume-cli](https://www.npmjs.org/package/resume-cli) command line tool from [JSON Resume](http://jsonresume.org) to compile our resume from a JSON schema into HTML and even PDF. This guide will walk through how to use Continuous Integration to validate and git deploy your resume!

## Getting Setup

You're going to want to first **fork** this repository. Then install the resume command line interface (cli) globally:

(hint: make sure you have **[nodejs](http://nodejs.org)** installed first!!)

```bash
# You may have to do sudo npm install depending on your system
npm install resume-cli -g

```

Now, cd to this repository install the required packages


```bash
cd ./path-to-your-local-repo
npm install

```

## The Resume.json file

This [resume.json](./resume.json) file contains all the data in your resume. You can modify my own or create your own by doing:

```bash
resume init
```
The schema is pretty clear, just put in the links and data where appropriate:

```json
{
  "basics": {
    "name": "Steven Edouard",
    "label": "Developer Evangelist",
    "picture": "https://scontent-b-sjc.xx.fbcdn.net/hphotos-prn1/t1.0-9/603953_10151522578258327_946466229_n.jpg",
    "email": "steven.edouard1@gmail.com",
    "website": "http://stevenedouard.com",
    "summary": "I'm a Developer Evangelist for Microsoft. Every day I work to empower individuals to build awesome things. I eventually hope to persue a role where I can have high impact on a product.",
    "location": {
      "city": "San Francisco",
      "countryCode": "US",
      "region": "California"
    },
    "profiles": [
      {
        "network": "Twitter",
        "username": "sedouard",
        "url": "http://twitter.com/sedouard"
      },
      {
```
The above json is truncated, checkout **[resume.json](./resume.json)** for the full thing.


Hope this guide inspires you to 'build' your own resume!
