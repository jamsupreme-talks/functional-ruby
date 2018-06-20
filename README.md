
# Fun[ctional] Ruby

Mulling over how we could bring some functional practices into Ruby and pondering why we would want to do that.

# Tentative agenda

- Pixie Procs (fancy chain-able procs)
- Names for "Higher order functions"
  - Pipe
  - Pipeline
  - Pipework
  - PipeTrait (module mixins)
- Easy way to do patterns
  - Saga
  - CQRS?
  - Event Sourcing?
  - Cross-cutting concerns (logging?)
- Reasons we want "functional" code
  - Simplified readability
  - Simplified testing
  - Easy to enforce an obvious convention
  - Once the latter, easy to develop cross-cutting concerns
  
  # Sample scenario
  
  - Pull data from a source (Pipe)
  - Pulling data from several sources (Pipeline)
    - Some local data
    - Some remote data
    - Some cached data
    - If any fail, easy bailout
    - Simplified error handling at top level
    
  Contrast the latter to a "OO" style implementation.
