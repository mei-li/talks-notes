# Predicting the Future of Web develpoment

by Richard Feldman, author of Elm in Action

Choose tech:

- Boring tech ----> NO
- What will age well -> best predicting possible

Typescript - hypescript
-----------------------
  -> Coffescript dropped, never picked as much as Typescript
  -> Massive adoption from top frameworks - Vue, Angular, Ember

  -> starts looking like Java in typewise, too much typechecking, it is ugly
  -> + not 100% type safety as there is Any

  -> Teams do not switch to it and later go back to JS

Prediction:
    * end of 2020: Typescript will take over the world
    * end of 2015: more writing typescript daily than JS

Web assembly
------------
    Lin Clark: explains it great
    Machine language in the browser

Usages:
    * improve performance of JS apps -> Not so important seems that it is fast enough
    * Figma: (photoshop in the browser): 
        it is in C++, native apps distributed in browser    
    Browsers like app stores and installers
    Multi MB apps? -> maybe seems to be widely tolerated
    Will JS, HTML stack go away -> No it will be more broad field. eg.
    * Games rendering -> Better with webassembly and C++, than CSS, JS
    
Prediction:
    Webassembly wexpands the webb App pie
        Maybe around 2025

NPM
----
Is npm the feature? Maybe entropic.dev - CJ Silverio JSConf EU 2019

yarn vs github package manager (eg. npm login --registry=...github)

npm attacks: left-pad, event-stream
Takeaway: USE that to avoid npm attacks!!!!!!
npm config set ignore-scripts true # to avoid extra script installation and attacks

Prediction: npm ecosystem will last
    2020: one security incident
    2025: at least one malicisous npm package


Complile to JS
--------------
* Js dialects (Dart, Babel...): similar PROS and CONS of JS
* Other langs (Closure -> JS, occaml -> JS, EML -> JS), Why?
    - Cheat code in hiring good people

ELM
-----
* faster than JS
* less errors - complier finds them
* Error as very nice and polite
* Things normally work

Prediction:
* Js alternatives stay nice and age well (like Elm)
    2020: grow not as facets as TS

# Becoming a team, one pixel at a time

by Lena Reinhard, Engineering Director, Circle CI

* Pixel as small actions 
* distributed systems of People

More companies are embrassing it ... like Circle CI
Distributed team challange:
    
  * more intentional
  * succesfully working remotely is a skill takes time


High perfoming team:

  * equal opportunities to contribute
  * phycological safety - culture, no fear of being embarassed or punished
  * Dependandability
  * Clarity
  * Meaning
  * Impact: Feeling of impact

Connection
----------
- When we are there we see, how much coffe, tired or not
+ Building trust remote:
    * connecting as people: need to meet once in a while to remind they are actual people
+ Hummaness
    * add photos in all the tools
    * greet people with the appropriate timezone: mindful
    * special interests channels, like random, etc, we are humans
    * reach out on special events: Birthday, etc
+ Expectations: 
    * What info goes where: emails, slack etc
    * How we make decision: ADR Architectural decision records adr.github.io
+ Lifting
    * coaching and offer learning opportunities
+ Sharing praise:
    * Expressing our gratitude, eg. in public channel
+ Training our feedback muscle
    * Share small feedback frquently, we do it more effectively:
        - Feedback guide: template fromm Book: Feedback (and other dirty words)
        - Observations -> Impact -> Question
           I saw you merged your PR without addressing my comments -> can you help understand why?
+ Staying aligned: avoid rabbit holes:

WHAT PROBLEM ARE WE TRYING TO SOLVE:
    * helps to stay focused
    * pull us out of rabbt holes
    * Ask it often

+ Remote loneliness
    * talk about it
    * structure work day
    * break and walk or physical exercise
    * meet other people
    * donut application
    * missing out of important discussions: talk to your manager

Collaboration
-------------
  * Stay humble: make space for others (explicit or implicit power also biases and blind spots)
  * No hero culture: pressure on the hero, no knowledge share
  * Being open of what we do not know, learn together
  * Experiment: embrace the change, try sth for 4 weeks and iterate

Communication
-------------
  55 % is body language !??!?
  30 % voice
  * be curious to learn from other, listen to learn not respond
       So you are saying that: .....
  * Give time to answer, enjoy the silence
  * Communicating difficult news, better than uncertainty 
  * **Learn to write better: being crisp, inclusive, emoji, explain of what you expect back (avoid idioms, jargon, cultural things)** <========== TAKEAWAY
  * Document with all abbrev and part of the onboarding
  * Edit before send (message clear? expectation what by when from whom, what can I already answer now?)
  * Better documentation with better writing


Continuity
----------
  * Building teams is never over
  
# Serverless Beyond Tutorials

by Ivan Culjak, Cloud solutions architect
@culajaklvan

Serveless is a methodology
    -> focus on your core business

etc. NO discovery , authentication


Pick scaling can be solved with overprovision but you do not pay since you do not use it

Azure or AWS lambdas for state management use:
* step/durable functions

Front door on Azure (AWS has sth similar) --> multi region

Event driven cloud at scale
* mind-shift needed

Security: SQL injection with file names

Testing: is more complicated, infrastructure as a service, CI/CD

Logging: Beware of the costs of logging per API request, use bulk logging


# Conducting Humane Code Reviews

by Adrienne Tacke, author Coding for Kids Python

@adriennetacke

Why we do code reviews?
-----------------------

  * catch design flaws
  * clarity and coherence
       If it is hard to understand
        -> complexity hides bugs
        -> refactor would be even harder
  * validate necessity
  * confirm functionality
    -> does it do what it is supposed to do?
    -> does it do what the dev intended to do?

Why we do not love code reviews?
--------------------------------

code review complains

  ### subjectivity  
  
  
  Get consensus with your team, get at the same page

  * Team Working Agreement: (always changing with consensus)
      - name conventions
      - style guide
      - code review process

  * Tools: Prettier, ESLint, (me: like Black, Flake8 for Python)

  * Objectivity always wins: Facts, Deprecated, Ticket requirements etc.

  ### tone of voice
  
  
    NO ->  This is terrible, 
           this is sh**
           it is not following the rules (passive aggressive)
 
    NO -> "Why would you use this?"
          "Are you really using this tool, really?"

    Give the benefit of the doubt.
    Give reasons, use facts

Avoid tone of voice issues:

- *Suggest with facts*
- *Reject with courtesy*
- *Clarify with an open-minded*  # ask before assuming, or jumping fast into conclusions

### Process Loopholes

 
   - Buddy reviewing/approving, with skipping actual process
   - Bias: review te rockstar code too with the same criteria
   - Solo dev: push to master 

Minimum viable effort

Avoid the process loopholes

  - Code review policies: Why is it needed?
  - 2 or more people
  - CODEOWNERS: (feature in github) auto add reviewers based on knowledge

Enforce the process for EVERYONE

