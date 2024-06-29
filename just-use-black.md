# Just use Black
After laying your eyes upon the beauty that is PEP 8, you go through a phase of trying out various code formatters - comparing their differences and performance. You nag your friends over their lines being 80 characters long and not breaking off at 79. You can't bear the sight of mathematical operators without whitespaces around them.

However, many developers overlook a crucial point from PEP 8:
> A style guide is about consistency. Consistency with this style guide is important. Consistency within a project is more important. Consistency within one module or function is the most important.

Most sane programmers realise pretty quickly that it is better to leave the styling to a tool, as long as it remains consistent. This brings us to the big question: which formatting tool should you and your team use?

## (Kinda) Brief History
### Early Days
Before the release of [PEP 8 (2011)](https://peps.python.org/pep-0008/#a-foolish-consistency-is-the-hobgoblin-of-little-minds), authored by Guido van Rossum himself, the Python scene was a bit like the Wild West. PEP 8 gave us rules to follow, but it also gave birth to endless nitpicking. There was a need for a tool that reminded the programmer to follow the guide.

### Initial Tools
[pycodestyle](https://pypi.org/project/pycodestyle/) was released to enforce PEP 8 rules. They'd point out style issues and potential errors, but it was still on you to fix them.
[pylint](https://pypi.org/project/pylint/) a static code analyser, also enforced PEP 8 conventions.

### Formatters
[autopep8](https://pypi.org/project/autopep8/): automatically formats Python code to conform to [PEP 8](https://www.python.org/dev/peps/pep-0008/). It uses [pycodestyle](https://github.com/PyCQA/pycodestyle) to determine what parts of the code needs to be formatted.

Guess what? Not everybody liked PEP 8. Many formatters arrived on the scene with varying degrees of customisation available. The most prominent was yapf. It came from Google.

[YAPF (Yet Another Python Formatter)](https://pypi.org/project/yapf/0.3.1/) generally adheres to PEP 8, but it goes beyond that by trying to produce the best possible formatting based on a set of formatting rules.

### The Holy War goes on
YAPF descended upon the scene like a beacon of hope. Its mission was noble: to transform Python code into something beautiful and readable while respecting the ancient texts of PEP 8. But the wars waged on. The 79-character-line tribe was still fiercely battling the 80-character-line tribe. The wars raged on, now with prettier, more context-aware weaponry.

### Any Color You Like
I won't even paraphrase how Black describes itself. Here's their unedited description:

------------------------------------------------------------------------
![black](Pasted image 20240629184559.png)
_Black_ is the uncompromising Python code formatter. By using it, you agree to cede control over minutiae of hand-formatting. In return, _Black_ gives you speed, determinism, and freedom from `pycodestyle` nagging about formatting. You will save time and mental energy for more important matters.

Blackened code looks the same regardless of the project you're reading. Formatting becomes transparent after a while and you can focus on the content instead.

-------------------------------------------------------------------------------------------------------------

Why though? It’s simple really…no more configuration, no more debates, just consistent code. It’s an “opinionated” formatter, which means it makes style decisions for you. And that’s a good thing. It removes the need for style discussions entirely. “Should we use single or double quotes?” Let Black decide. Imagine all the time you’d waste nitpicking over style in code reviews. Black frees up that time. Now, reviews can focus on what really matters: the logic and functionality of your code.

Black was not here to negotiate or cater to individual tastes. Its doctrine was simple: there is only one way to format code, and Black’s way is the way.

Black is opinionated, so you don’t have to be. Focus on the content, not the style. Just use Black.
