Scumbag
=======

Back in 2013 we had the first BSides Winnipeg conference, later renamed to The Long Con. At this convention, we decided to throw a CTF. The 'scumbag' challenge was the only one that remained unsolved when the CTF ended. This challenge holds a special place in my heart because it gave me the opportunity to program in a stack-based language, something I hated and enjoyed.

Scumbag bills itself as "a troll in two parts" because the solution has two phases. When you open the PostScript file `scumbag-obfuscated.ps` in a PostScript viewer it will pin a CPU attempting to render itself. This is because the code that describes the output is intentionally, insanely inefficient. The code is so inefficient that I have never seen it render the page without alteration. If you take the time to reverse engineer the PostScript code, you can discover the inefficiency and bypass it, leading to the output shown in `scumbag-output.pdf`.

Once the output has been generated, the contestent will likely immediately recognize what they have to do next... and groan.The output is a diagram showing a substitution-permutation network that spans 10 pages. It is possible to avoid going through the network by hand to generate the flag, or implement the network in code. Either way, the flag at the end is `DONT-HAET-ZE-AUTHR-HATE-MAI--CTF`. It's been 8 years and I'm still laughing about this puzzle.

-Mak
