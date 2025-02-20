# Node.js Server Hang Issue

This repository demonstrates a common Node.js server issue where long-running requests can cause the server to hang and become unresponsive.  The problem stems from blocking the event loop with synchronous operations within the request handler.

## Problem

The `server.js` file contains a simple HTTP server that simulates a long-running task. During this task, the server is unable to process other requests, resulting in a hang.

## Solution

The `serverSolution.js` file provides a solution using asynchronous operations to prevent blocking the event loop.  This allows the server to remain responsive even during lengthy tasks.