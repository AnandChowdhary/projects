---
title: Blueboard
tags: projects
subcategory: IoT
intro: Bluetooth-powered smart billboard that shows relevant advertisements and information based on who's passing by it.
date: 2018-01-23
work: ["IoT", "Hardware"]
style: cover
timeline: 2 months
img_src: /assets/blueboard/blueboard_2x
img_type: png
icon: /assets/blueboard/icon.png
icon_bg: true
stack: ["C++", "Java"]
tools: ["Processing", "Arduino", "Android"]
---

BlueBoard is a Bluetooth-powered smart billboard that actually cares about you. Privacy-first and context-aware, it connects with your smartphone via Bluetooth and shows you relevant advertisements and information.

<!--more-->

Users can open the BlueBoard app and set their preferences by assigning points from 0 to 10 to everything you they like — from technology and fashion to food and the weather. BlueBoard listens to the app and securely transfers their preference data. It then understands their preferences and shows them the best, most relevant advertisements from multiple sources. With multiple users, it finds their common intersts and shows what works for everyone.

<div class="two-images">
  <img alt="" src="/assets/blueboard/1.jpg">
  <img alt="" src="/assets/blueboard/2.jpg">
</div>

BlueBoard was my project for the module "Smart Environments", a quarter of Creative Technology BSc's first year focused on ubitiquous computing and the IoT.

BlueBoard used a custom-built Android app written in Java, along with an Arduino program that would send the JSON data object via serial communication to Processing. Processing would compute and display the relevant information on the screen.

<div class="image"><img alt="" src="/assets/blueboard/team.png"></div>

<footer>This project was done in collaboration with <a href="https://portfolio.cr.utwente.nl/student/hesselbosma/">Hessel Bosma 🇳🇱</a>, <a href="https://portfolio.cr.utwente.nl/student/kmw/">Karlijn Wiggers 🇳🇱</a>, <a href="https://portfolio.cr.utwente.nl/student/pawirotaroenorzg/">Rezfan Pawirotaroeno 🇸🇷</a>, and <a href="https://portfolio.cr.utwente.nl/student/wcouwenbergh/">Wouter Couwenbergh 🇳🇱</a>. It wouldn've have been possible without our module coordinator <a href="http://wwwhome.ewi.utwente.nl/~scholten/" target="_blank" rel="noopener noreferrer">Hans Scholten</a>.</footer>
