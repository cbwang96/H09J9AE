- C does not support exception handling. 
	- It can be implemented by library/macros/code jumps, but this is sometimes more a source of error than anything else. 
	- On the other hand C/POSIX does support signals that can trigger a handler.
- Ada
	- Supports explicit exception declaration
	- Termination model
	- Propagation of unhandled exceptions
	- Limited exception parameters (only strings)
	- How Ex. work in Ada is treated below
	- Last wishes: reraise the exception at the end of the handler
	- Suppress: `pragma` used to ignore exceptions at run- time - saves time because no detection.
	- When using subprograms, not always clear which package raised which exception.
	- Function don't have to declare they can throw exceptions (can be done in comments)
- Java does support exception handling. 
	- Similar to Ada, also termination model, propagation
	- Exceptions can be inherited
	- How Ex. work in Java is treated below
	- Last wishes: reraise the exception at the end of the handler through finally clause.
	- Can pass any exception parameter
	- Functions that can throw an exception must formally declare so (throws XY_exception)