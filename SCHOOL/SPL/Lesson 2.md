## Rules of Programming

- Create programs that are easy to validate and maintain
- Build units of program that are GENERAL, FLEXIBLE  and promote CODE REUSABILITY.
- Programs should have a well organized internal structure.
- Programs should be well documented.
- Programs must be portable and have strict adherence to standards.
- Appropriate algorithms should be carefully chosen.
- Bug free code is more important than clean code.
- Keep code has simple as possible; think of the next developer.
- Clarity is more important than efficiency.
## Naming in Programming

A naming convention is a set of rules for choosing the character sequence to be used for identifiers which denote variables, types, functions etc.

### Rules for naming variables

- Use nouns, noun phrases, adjectives and verbs for naming identifiers.
- Use prefixes, suffixes and delimiters when necessary.
- Identifiers must not be named after reserved words in the PL.
- Consistency is key.
- Use capitalizations and initial caps when necessary.
- Names must be expressive of what they are intended for.


### Variable Components

1. Name.
2. Type.
3. Location (l-value).
4. Reference (r-value).
5. Scope.
6. Lifetime (Interval of time in which a location is bound to a variable).

## Binding

Binding in PL refers to how a variable is created and used or bound by within the given program or possible other programs.
Attributes of parts of programs must be bound to objects before or during execution. a binding fixes a a value or other properties of an object (from a possible set of values).
Time at which binding occurs is called binding time.

### Types

- Dynamic binding: occurs at execution or run time. e.g. Lisp and some scripting languages.
- Static binding: occurs at translation, language implementation, language definition or compile time. Most languages apply this e.g. C, Java, Pascal etc.

Many language design decisions affect binding time.

- **Late binding:** more flexible.
- **Early binding:** more efficient.

It is more efficient to bind at translation than at execution i.e. Static binding is early.
Programming choices may affect binding time.

### Binding storage

Bindings can be stored at both compilation and execution.

#### Compilation

- Declarations are stored in symbol tables (name -> attributes).
- Most bindings are used during compilation process.

#### Execution

- Run time environments keeps track of meaning of names (name -> location).
- Contents of location stores in memory (also called state) (location -> values).
- Interpreters keep all 3 kinds of bindings in one environment.

## Scope

Variable scope determines a variables visibility to other parts of the code and how *how long* a variable is available when the program is executing.
A variable's scope is determined from the location by which the variable is defined.

### Types

- **Local scope:** refers to variables declared inside functions and not accessible outside the function.
- **Global scope:** refers to variables declared outside functions and accessible by every function in its scope.
- **Static scope:** helps a program *remember* what value is stored in between function calls. An initialize static local variable when called more than once in the program keeps is value throughout execution. 