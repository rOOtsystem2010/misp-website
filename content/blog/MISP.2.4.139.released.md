---
title: MISP 2.4.139 released (Quality of life and bugfix release)
date: 2021-02-16
layout: post
banner: /img/blog/dashb.png
---

# MISP 2.4.139 released

We have released 2.4.139, the latest release for MISP squashes a set of pretty annoying bugs, whilst also adding some shiny new features to play with, along with the usual update of the JSON libraries.

Besides that, several usability and performance issues have been resolved along with a host of small improvements, additional API improvements, etc. Make sure that you read the detailed changelog to see all the improvements.

# MISP modules are now Event Report aware!

The Event Reports are the hot new feature of the past few weeks and we are working on ensuring that analyst reports are becoming the standard companions of the classic event format. For anyone that hasn't played with them before, have a look at the [blog post](/2020/10/08/Event-Reports.html) describing how you can create rich, interlinked reports to accompany your events.

The main update to the Event Report system is its inclusion in the module system as of this version, so if you are building integrations with MISP or simply want to build a convenient way to incorporate reports from your favourite information sources, this feature will make your life much easier.

# MISP modules can impose options for the event fetcher

Want to restrict what parts of an event your module should receive from MISP? Would you like to include the decay score in your module? Pass parameters back to the fetcher so it can prepare an event that better fits your module's needs!

# EventStream widget

![](/img/blog/dashb.png)

The built in Dashboard system in MISP has been underutilised since its inception, partially due to its initial focus on a non CTI use-case. We have been working on remedying this over the past few months, including the addition of new widgets to monitor your instance's health as an administrator, to gain high level insights into your sharing community's sharing practices, etc.

Something that has been missing for a while though was the ability to monitor ongoing trends based on your own interests, such as any new events coming in that relate to a topic that you are interested in. The EventStream widget aims to solve that, by offering a customisable event index widget.

Users can set their interests in terms of organisation sources and applied tags (such as threat actor, tool and other names) to show the most recent additions that touch on the given subjects.

This widget also brings a flexible reusable UI layer with itself that widget developers can reuse for a host of other use-cases.

# Acknowledgement

We would like to thank all the [contributors](/contributors), reporters and users who have helped us in the past months to improve MISP and information sharing at large. This release includes multiple updates in [misp-objects](/objects.html), [misp-taxonomies](/taxonomies.html) and [misp-galaxy](/galaxy.html)
.

As always, a detailed and [complete changelog is available](/Changelog.txt) with all the fixes, changes and improvements.

