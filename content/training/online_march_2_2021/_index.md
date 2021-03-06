---
title: Velociraptor training (Online Edition)
type: bizcraft_page
layout: single
slider:
  image: /images/slider/bg3.jpg
  title: Enterprise Hunting and Incident Response (Online Edition)
  subtitle: Digging deeper with Velociraptor!
  buttons:
   - title: Book now!
     url: https://www.eventbrite.com.au/e/enterprise-hunting-and-incident-response-online-edition-tickets-122862989509
---

The life of an information security professional is a hectic one. It
seems like you are fighting fires every day and always behind the
eight ball. You know you should be proactively hunting for emerging
threats in your network but the tools at your disposal simply do not
scale. You can check each machine individually for hardening and
policy compliance but you have many thousands of endpoints deployed,
it is hard enough to keep up with the alerts.

You try to keep across the latest malware trends and threat Intel
feeds. You might even receive a tip-off that your network is
compromised by a specific variant of malware of an APT group. You wish
there was a way for you to easily inspect all your endpoints for the
indicators, digging deeper into any machines which might be
compromised.

# About this course

This online course will be split into 7 sessions over 2 weeks with 2-3
hours per day. We will deliver the course live over Zoom in an
interactive, hands on format. There will be time for questions and
free discussions.

# Schedule

We will cover one module per day. Modules are hands on and take about
2 hours. After the workshop we will stay on the Zoom for open
discussions.

|Topic| Time|
|------| ----|
|Topic: 01 - Velociraptor Installation and Overview | Time: March 2, 2021 09:00 AM Brisbane|
|Topic: 02 - VQL Fundamentals | Time: March 3, 2021 09:00 AM Brisbane|
|Topic: 03 - Forensic Analysis Pt 1 | Time: March 4, 2021 09:00 AM Brisbane|
|Topic: 04 - Forensic Analysis Pt 2 | Time: March 5, 2021 09:00 AM Brisbane|
|Topic: 05 - Interactive triage | Time: March 9, 2021 09:00 AM Brisbane|
|Topic: 06 - Proactive Hunting | Time: March 10, 2021 09:00 AM Brisbane|
|Topic: 07 - Extending VQL and API | Time: March 11, 2021 09:00 AM Brisbane|


## Times in your region

<a href="https://www.timeanddate.com/worldclock/converter.html?iso=20210301T230000&p1=47&p2=179&p3=104&p4=224"><img src="march_2_times.png" width="600" /></a>

***********************************************************************

# Overview

The course is an introduction to forensic analysis and incident
response with Velociraptor. It is intended for information security
professionals, system administrators and incident responders.

Velociraptor is a powerful endpoint tool – you can hunt for artifacts
in minutes across thousands of endpoints and perform advanced forensic
analysis on the endpoint, rapidly and at scale. Welcome to the future
of DFIR!

This training event is run by the company behind Velociraptor - you
will learn from the developers and practitioners who use Velociraptor
every day to respond to incidents and investigate breaches. Course
materials and detailed preparation instructions will be distributed to
participants the week prior to the course.

You will receive access to the online portal which includes all the
training materials, as well as video recordings of the course
afterwards.


# Course Contents

## Installation and introduction to the UI

The old way of performing in-depth forensic analysis and incident
response with your existing tools is clearly not adequate or scalable
to many endpoints. It is just too time consuming to analyze many
machines, acquire large disk images, and memory, let alone actively
hunt for indicators of compromise across your entire network.

You heard that Velociraptor, an advanced open source endpoint
visibility tool, is the ideal tool for effectively investigating,
hunting and monitoring your endpoints with minimal fuss.

You are excited to install Velociraptor and deploy it to your entire
infrastructure. This module is for you! In this module we will deploy
Velociraptor and gain an introduction to the basic operation of the
tool. We will learn the architecture and the unique mindset behind the
tool.

### Exercises

* Installing a typical secure Velociraptor server on a cloud VM.
* Deploy Velociraptor clients on a typical Windows network using group policy.
* Introduction to the Velociraptor Query Language (VQL). It is the
  workhorse behind the tool and mastering VQL will provide you with
  the flexibility you need to adapt to rapidly changing challenges.

## VQL Fundamentals

Velociraptor's secret source is really its powerful query
language. Using this you can flexibly query all your endpoints in
minutes to collect files, perform remote analysis and surgically
extract forensic artifacts. This module is a VQL deep dive, full of
practical exercises and low level information, we introduce VQL and
apply it to real life collections.

## Windows Forensic Analysis

Velociraptor puts the power of experienced digital forensic
investigators at your finger tips! This module will cover at a high
level the basics of modern forensic analysis techniques. You will now
be able to apply these techniques to answer many questions – from
determining evidence of malware execution, detecting persistent
malware to uncovering malicious user activity and determining
ex-filtration of proprietary data.

* Basics of Windows Forensics
 * NTFS Overview
 * Data Streams and the $MFT
 * Recovering evidence of deleted files from $MFT and $I30 carving
 * Evidence of execution: Prefetch, SRUM, USN Journal

* Registry
 * What is the windows Registry?
 * Inspecting user hives and user profiles.
 * Common registry based malware persistent mechanisms

* Windows Management Instrumentation (WMI)
 * What is WMI and what information is exposed with it?
 * Lateral movement and privilege escalation using WMI – an attacker’s favorite!
 * WMI persistence mechanisms (Filter/consumer bindings)

* System Resource Usage Monitor (SRUM)
 * The SRUM database can help us determine evidence of past
   executions, connected networks, bytes sent/received and much more.

* Windows Event Logs are the cornerstone of windows auditing
 * How are event logs structured?
 * What are event Ids and how do they relate to messages?
 * Some examples of common event log messages: lateral movement, powershell abuse etc.

* Machine state and process forensics.
 * Process listing, VADs, Mutants, DLLs loaded: Determine powershell script is connecting over HTTP by inspecting its VAD
 * Detect a Yara signature in process memory, dump the process memory and upload to server for further analysis.

## Triage and data collection – collecting data without an agent

A remote user is suspected of being compromised. The user is on a slow
network with limited bandwidth, and can not upload vast amounts of
data quickly. You need to triage their system to determine if they are
compromised. You would like to acquire memory, critical files and
capture as much of system state as possible. Unfortunately, the user
is not command line savvy – but luckily they are really good at double
clicking a binary!

In this module we learn how to perform offline collection with
Velociraptor. We prepare an automatic collection package which simply
acquires system state when double clicked.

### Exercises

* Full memory capture for later analysis with e.g. Volatility.
* Collect file sets – registry, $MFT etc.
* Configuring autoexec Velociraptor for simple double click execution.

## Lateral movement and hunting

You have discovered evidence of compromise on some of your
systems. Your boss wants to know if the attackers have laterally moved
through your network and the extent of compromise. You would like to
hunt for the indicators. You refer to the Mitre Att&ck framework for
typical Tools Technique and Procedures (TTPs) used by your adversary,
and want to hunt for these across your network.

In this module we also use Elastic and Kibana to demonstrate how
events and collections can be forwarded by Velociraptor to those
platform for scalable and efficient post processing/dashboarding.

### Exercises

* Use the Mitre Att&ck framework to develop a targeted VQL query for detecting a form of persistence. Hunt for it and identify the compromised hosts.
* Yara and Signature based searching. Searching both files and memory for patterns
* Performance management of endpoints

## Monitoring for events

You have learned so much in this course about how to detect malware,
lateral movement and compromise. But so far, everything was reactive –
we were looking at forensic evidence left behind after the fact. What
you really want is to design monitoring and alerting that will let you
know when evidence of compromise are found in real time. Luckily
Velociraptor is a complete endpoint monitoring and response tool!

* Introduction to Velociraptor’s event monitoring framework
* Windows Event Log forwarding and classification. Event log enrichment and prioritization.
* Monitoring for changes in system state: New file executions and High
  risk files such as office macros and remote PowerShell

# Extending VQL and API

Velociraptor is a great platform, but in a real deployment it is only
a small part of a wider solutions. In this module we explore how to
seamlessly extend VQL using Powershell or an external binary. This
opens a wide range of possibilities including automated remediation at
scale!

We then move onto Velociraptor system administration (Using VQL of
course!) and learn how to safely expose the Velociraptor API to
external programs so Velociraptor can be completely controlled by an
automated pipeline.

### Exercises:

* Adapt a Powershell script to VQL, write an artifact, hunt for it everywhere.
* Remediate a Cryptominer infection using scheduled tasks for persistence from the entire fleet in seconds.
* Automatically decode encoded powershell command lines on the server.
* Write a python script to connect to the server, collect and artifact from a client, wait for it to complete then retrieve the results.

# This course should not be missed!

You have heard about Velociraptor and how it makes DFIR easy and
accessible. Learn what all the buzz is about from the people who wrote
it! This is a rare opportunity to become involved and support this
open source tool.

## Testomonials

What did you most like about the workshop?

* Hands on labs using various scenarios
* understanding the potential of the tool
* Good balance of theory and hands on lab
* The structure of the course covered a lot of the theoretical basis and practical applications of the tool. Mike was happy to alter the flow of the course to better suit the participants which was much appreciated.
* I didn't know much about the product before attending so it was a great overview of everything Velociraptor.
* Filled in some of the gaps in my knowledge about how Velociraptor works.
* Everything! The course content was already inclusive, but extra thanks for considering my on_the_fly arbitrary requests and demo'ing via `quiz method` :)
* Mike's methodology for teaching process, the slides, the notes, i loved this course!!!


### About Velocidex

Velocidex Enterprises was founded by well established industry
professionals with many years of proven expertise in the development
of digital forensic software and its use to support a wide range of
digital forensic investigations and cyber breach response cases.

Velociraptor aims to provide the "last step" in the process of digital
forensic investigations, security monitoring and threat hunting. We
already know a great deal about how to investigate computer systems
and monitor for malicious activities. Velociraptor aims to encapsulte
this industry knowledge and empower both experts and novices to
leverage it, to collect and analyse evidence of malicious activities
with speed and precision.

# Sample chapter

A sample module from the full course is now available! [Click here to view](/docs/presentations/training_2020/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/l1_sKDmNWS4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/c-XOeuT4qg8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/u7KBwgHIZ3U" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/HvwFdaTJvd0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
