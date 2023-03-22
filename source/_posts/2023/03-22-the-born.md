---
title: The Born of Lightyears Traveler
date: 2023-03-22 18:00:00
tags:
- blog-building
---

I used to write my blog about my daily life using a self-hosted WordPress. Years ago, I wanted to make a new blog about techs, and today I finally decided on it.

## Step 0: Pick up a tool

It is not easy for me to build up a blog from scratch, especially when I know little about web development technologies. Instead of building my blog from scratch, I decided to pick up a blogging tool. And I eventually picked up Hexo, a popular static site-generating tool. I have seen many blogs using Hexo, including some of my friends' blogs. Time has proved that Hexo can be the right tool for making blogs.

When one uses Hexo, they write their blog post in Markdown format, and Hexo converts the markdown files to HTML blog posts. Most of the tedious jobs are handled by Hexo.

In Hexo, the *theme* defines the website's and blog posts' appearance. Hexo comes with a built-in theme named Landscape. There are also many lovely themes available on the Hexo showcase. I could use one of those themes, but since I keep telling myself that I want to polish my skills in building websites, why not make a brand-new theme myself? Let's do it.

## Step 1: Pick up some fonts

Let's pick the correct fonts for our website first. Although my mother tongue is Mandarin Chinese, I write my posts in English only to share my ideas with more readers. Chinese fonts are a headache: they are heavier than Latin fonts in file size. As the main language for the blog is English, using Latin fonts is enough, at least for now.

I am always fond of using free-and-open-source fonts. But where to find them? Not to kidding, but I find the [modding wiki page of Crusader King III](https://ck3.paradoxwikis.com/Fonts) quite useful. The page says that one can find fantastic fonts on Font Squirrel, Cool Text, Vic Fieger's Website and Google Fonts. Let's navigate to these sites and dig out our treasure fonts. (Remember to set the license filter.)

I will pick up a title font, a text font and a monospace font for displaying code snippets in the future. After some hours of digging, I still need to decide which fonts to pick up: There are too many fonts available, and I'm a bit selective. Aha, let's keep it simple for now. OK... System default font; that's the choice.

## Step 2: Make a simple layout

About the website layout, I would like to find some existing blogging websites/themes for reference. Without touching the source code of the Hexo engine, it will be easier for me to learn to make a theme by inspecting the popular themes built into the Hexo itself: the Landscape theme.

Following [the guide](https://hexo.io/docs/themes) on Hexo documentation, I make a basic theme in a few minutes.

Hexo uses a template-rendering engine to render the Markdown into HTML. One can control the appearance of the rendered result in a programming approach. Hexo officially supports multiple rendering engines. Among all the engines, I use EJS, the Embedded JavaScript engine. EJS shares a common syntax with plain JavaScript, and thus it is really easy to pick up.

When the page renders, Hexo interprets the original Markdown file into HTML and feeds the HTML and other metadata to the EJS engine so that the EJS engine can create some decorations around the HTML produced from Markdown. EJS engine parses the layout file and inflates the passing data into the final HTML output. For the very first version of my Hexo theme, I pipeline the HTML without extra processing. However, the page feels like a website in the 1990s. That's the start.

## Step 3: Name the blog and theme

After finishing the basic layout, I want to give the theme a beautiful name. *Alisha* comes to my mind. It is the character name from my favorite role-play game/anime *Tales of Zestiria*. And the blog is named *Lightyears Traveler*, which is inspired by the name of PRG *Octopath Traveler* published by Square Enix.

I deployed the blog and theme on GitHub Actions, and it is done for now. I admit it is a really simple theme, but it is the start after all years of hanging there.

I'm quite busy with school routines now. I plan to spare some time shortly to improve the theme. See you next time.
