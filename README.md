# Complexity Theory for Agile Software Developers
## test-first TDD can be frustrating
- paralysis of the first test
- fighting a legacy code base
- rewriting code AND tests over and over again while figuring out a sensible
  design

## workaround: test-after TDD
- write code until happy, then test
- test-DRIVEN design -> listen to the tests and refactor
- somehow this feels wrong

## spike and stabilize
- considered an advanced technique, to be used when you mastered TDD
- basically, code has to prove its value, only then do we need to test it
- spikes are somewhat functional and thus have value

## context to the rescue
- different people see the same problem in different lights
- where a novice doesn't understand the problem, a master resolves it easily

## the cynefin framework of sense-making
- change some text on a web site
  - simple domain
  - solution is self-evident
  - best practice
  - sense, categorize, respond

- change styling of an element on a web site
  - complicated domain
  - solution requires expert knowledge
  - known unknwon: how is the styling done? where can I put my change?
   (unless you are the CSS master)
  - several proper solutions possible
  - good practice
  - sense, analyze, respond

- implement a new feature
  - complex domain
  - emergent solution
    save-to-fail experiments (try different approaches on a development system)
  - unknown unknowns: we have no idea beofrehands, how an approach will
    actually interact with the existing code
  - probe, sense, respond

- emergency production bug
  - chaotic domain
  - just fix it, any way possible (novel solutions and innovation)
  - move to another domain as soon as possible and fix it properly
  - act, sense, respond

## so what?
- figure out where you are
- use appropriate techniques for the domain
- work on the constraints to move to the desired domain
  - relax constraints to open up novelty
     - complicated -> complex
     - code spikes
  - increase constraints to exploit the results
     - complex -> complicated
     - TDD (stabilize spike)
     - automation (complicated -> simple)
- TDD (test-first) is probably best for complicated problems
- spike-and-stabilize for complex problems
- same for other agile techniques like pair programming
  - multiple parallel safe-to-fail experiments (code spikes) w/o pp
  - use pp to stabilize the best solution or in complicated domain
