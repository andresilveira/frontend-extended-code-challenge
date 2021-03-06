Hubrick Frontend Challenge
========================

We're excited that you're interested in joining the [Hubrick](https://hubrick.com/) team. 
The purpose of this test is to see how you approach problems as well as to evaluate the quality of your code.

# Challenge description
The challenge is to create a simple flow engine.

A flow engine is an application that executes a flow consisting of several linked rules, in this case against some incoming data (*a JSON string that can be parsed to a JavaScript object literal*). 

Each rule should contain (at least)
	
- An ID (unique within the flow, required)
- A rule that will be run against the incoming json data. This is a function that takes a parameter and returns a boolean result. Each function should be called with the same incoming data (the JS object literal)
- An ID of the rule to execute if the function returns true (`true_id`)
- An ID of the rule to execute if the function returns false (`false_id`)
	 
Pass an object (an example of an object and a rule is given below) to the created flow. 

The execution will end when a `null` is provided for the `true_id` (and the function returns `true`) or when `null` is provided for the `false_id` (and the function returns `false`).

Additionally, the flow engine (with the provided rule-set) should not be circular.

# Mockup
Please implement UI according to the design provided here frontend-challenge-flow-mockup.png

# Instructions
- Please use ReactJs as view layer. For the Flow logic use a pure JavaScript (no underscore and other libraries)
- Unit tests and bundler/task runner are a plus.
- Use pure CSS preprocessor for the styling of the UI - no external libraries

# What we're looking for:
- Code quality
- Correctness
- Technical choices

We appreciate your time and energy completing the coding exercise and will review your solution as quickly as possible.
