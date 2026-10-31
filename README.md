# Limiting Reagent Analysis

An interactive teaching tool for general chemistry students learning limiting reagent, theoretical yield, and percent yield calculations.

**Live tool:** https://lufox2021.github.io/Limiting-Reagent-Analysis/

Built by Tad Fox, Adjunct Chemistry Instructor, Campbell University (Adult & Online Education, Camp Lejeune campus).

## What students do

Each problem gives a reaction (unbalanced), the grams of two reactants, and the grams of product actually isolated. Students work through the problem step by step; each step unlocks only after the previous one is correct.

### Review tab
- What a limiting reagent is, with an everyday analogy
- The step-by-step procedure
- Common mistakes
- A fully worked example (Al + Cl₂ → AlCl₃) in which the reactant with the *larger* mass is the limiting one

### Coaching tab
1. **Balance the equation:** enter coefficients. Balanced answers not in lowest terms are accepted with a note.
2. **Molar masses:** calculate molar masses of the reactants and the product (atomic masses to 3 decimals are shown on screen).
3. **Limiting reagent:** for each reactant, enter moles, the mole ratio (mol product / mol reactant, as a fraction or decimal), and the moles of product it could make; then choose the limiting reagent.
4. **Excess reagent remaining:** moles and grams consumed, grams left over.
5. **Theoretical yield:** moles and grams of product.
6. **Percent yield.**

Feedback escalates from a hint to the rule, and a **Show answer** button appears after three tries. The tool recognizes and names common mistakes, for example:
- choosing the reactant with the smaller mass or fewer moles as limiting
- a mole ratio that is upside down or assumed to be 1:1
- calculating the yield from the excess reagent
- multiplying grams by molar mass instead of dividing
- applying a subscript only to part of a parenthesized group
- inverting the percent-yield ratio

### Testing tab
Molar masses are given. Students enter only the key answers: coefficients, the limiting reagent, grams of excess remaining, the theoretical yield, and the percent yield. Feedback is correct/incorrect only. Attempts are unlimited ("Show answer" after three tries), and a summary at the end shows how many steps were correct on the first try.

### Difficulty levels
| Level | Reaction type |
|---|---|
| 1 | Synthesis |
| 2 | Single displacement |
| 3 | Double displacement & neutralization |
| 4 | Combustion & simple redox |
| 5 | Larger combustion & redox |

## Problem design
- The built-in bank holds 60 reactions, all with exactly two reactants.
- Masses are generated fresh each time a problem is drawn, so students can practice the same reaction with different numbers. Either reactant can turn out to be limiting, and percent yields fall between 60% and 95%.
- All masses given and answers asked for are in grams.
- Numeric answers are accepted within ±2% (±0.5% for molar masses) to allow for rounding. Significant figures are not enforced.

## Adding your own problems (Instructor tab)
1. Enter two reactants and the product(s), unbalanced. The tool balances the equation and shows the molar masses.
2. Choose the level and the product to report the yield for. Optionally fix the reactant masses and the actual yield; leave them blank to have new amounts generated each time.
3. **Save problem.** Saved problems are stored in *your browser only*.
4. To share them with students, click **Export problems.json** and add that file to this repository next to `index.html`. The live site loads it automatically.

## Technical notes
- A single self-contained `index.html` (HTML, CSS, and JavaScript). There is nothing to install and no external libraries.
- Runs in any modern desktop browser. To use it offline, download `index.html` and double-click it. (`problems.json` loads only from the live site, not from a local copy.)
- Equations are balanced automatically by integer Gaussian elimination, so any reaction with a unique balanced form can be added.

## Related tools
Part of a set of general chemistry teaching tools by the same author: Factor-Label Workbench, Diatomic MO Lab, Molecule Viewer, Orbital Atlas, and others at https://github.com/lufox2021.
