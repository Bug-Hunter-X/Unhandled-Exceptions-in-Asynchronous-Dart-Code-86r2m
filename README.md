# Unhandled Exceptions in Asynchronous Dart Code

This repository demonstrates a common error in Dart: neglecting to handle potential exceptions when using asynchronous operations, specifically `Future`s and the `http` package.  The `bug.dart` file showcases the faulty code, while `bugSolution.dart` provides the corrected version with proper error handling.

## The Problem

The original code attempts to fetch data from a remote API using `http.get`.  However, it lacks robust error handling. Network issues, invalid URLs, or server-side errors can result in exceptions, potentially crashing the application.

## The Solution

The solution involves using a `try-catch` block to gracefully handle exceptions that might occur during the API call. This ensures that the application doesn't crash and allows for appropriate error reporting or fallback mechanisms.

## How to Run

1. Clone this repository.
2. Run the `bug.dart` file to observe the unhandled exception.
3. Run the `bugSolution.dart` file to see the improved, exception-handled version.