---
title: Security Concepts in ASP.NET Core SignalR
author: rachelappel
description: Learn how to use authentication and authorization in ASP.NET Core SignalR.
monikerRange: '>= aspnetcore-2.1'
ms.author: rachelap
ms.custom: mvc
ms.date: 05/01/2018
uid: signalr/hubs
---

# Security Concepts in ASP.NET Core SignalR

By [Andrew Stanton-Nurse](https://twitter.com/anurse)

## Overview

SignalR provides a number of security protections by default, but it is important to understand their limitations.

### Cross-Site Request Forgery

Cross-Site Request Forgery (CSRF) is an attack where a malicious site sends a request to a vulnerable site where the user is currently logged in. ASP.NET Core SignalR requires that Cross-Origin Resource Sharing (CORS) be configured on the server, in order to protect against these issues.