# Unexpected Behavior with Mutable Variables in F#

This example highlights a potential pitfall when working with mutable variables in F#.  Unlike imperative languages, F#'s immutable nature can lead to unexpected results if not handled carefully.  The included code demonstrates this issue, showcasing a mutable variable's behavior in a way that might contrast with expectations.

## Bug

The provided `bug.fs` file shows the incorrect usage of mutable variables. It demonstrates how changes to mutable variables *after* their values are used in calculations may not reflect as expected. 

## Solution

The `bugSolution.fs` file offers the preferred approach. It uses a function to encapsulate the calculation, ensuring that the result reflects the current values of the inputs.