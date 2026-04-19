# Automata Studio

A web-based tool for converting Regular Expressions to NFAs, DFAs, and Minimized DFAs with interactive visualization.

## Features

- **Regex to NFA Conversion**: Convert regular expressions to Non-deterministic Finite Automaton using Thompson's Construction
- **NFA to DFA Conversion**: Subset construction algorithm to convert NFA to Deterministic Finite Automaton
- **DFA Minimization**: Minimize DFA using partition refinement algorithm
- **Interactive Visualization**: See the automaton with states, transitions, and accepting states
- **Simulation**: Test if a string is accepted by the automaton
- **Step-by-Step Mode**: Watch the conversion process step by step
- **Animation Mode**: Animate the conversion process

## Usage

1. Enter a regular expression in the input field (e.g., `(a|b)*abb`)
2. Click the pipeline steps:
   - **NFA** - Generate NFA from regex
   - **DFA** - Convert to DFA (step-by-step or all at once)
   - **Minimize** - Minimize the DFA
3. Use the simulation panel to test input strings
4. Export visualizations as PNG

## Supported Regex Syntax

- **Literals**: `a`, `b`, `c`, etc.
- **Concatenation**: `ab` matches "ab"
- **Alternation**: `a|b` matches "a" or "b"
- **Kleene Star**: `a*` matches zero or more "a"
- **Plus**: `a+` matches one or more "a"
- **Question Mark**: `a?` matches zero or one "a"
- **Grouping**: `(ab)*` for complex patterns
- **Character Classes**: `[abc]` matches a, b, or c

## Examples

| Regex | Description |
|-------|-------------|
| `a*` | Zero or more 'a' |
| `(a|b)*abb` | Strings ending with 'abb' |
| `a?b+` | Optional 'a' followed by one or more 'b' |
| `(a|b)*` | Any combination of 'a' and 'b' |

## Technology

- Pure HTML/CSS/JavaScript (no dependencies)
- Thompson's Construction for NFA
- Subset Construction for NFA→DFA
- Partition Refinement for DFA Minimization

