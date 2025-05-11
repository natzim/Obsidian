## Amazon Link
[Clean Code in Python by Mariano Anaya](https://www.amazon.com/Clean-Code-Python-maintainable-efficient/dp/1800560214)

## Referenced Books
# Notes
## Chapter 1 - Introduction
- Technical debt refers to the concept of problems in the software as a result of a compromise or a bad decision being made
- `Sphinx` - Creates the basic scaffold for the documentation of your project. With the `autodoc` extension (`sphinx.ext.autodoc`) in particular, the tool will take the docstrings from the code and place them in the pages that document the functions
- If the functions you are writing is really simple, and self-explanatory, it is probably better to avoid adding a redundant docstring that will require maintenance
- The name of the argument `dely_in_seconds` seems quite verbose, but despite that fact, it still does not provide much information. What constitutes acceptable good values for seconds? Does it consider fractions? Instead consider:
```python
Seconds = float
def launch_task(delay: Seconds):
```
- With the introduction of annotations, a new special attribute is also included, and it is `__annotations__`. This gives us access to a dictionary that maps the name of the annotations with their corresponding values
- When looking at the code written by a peer, you should ask such questions as:
	- Is this code easy to understand and follow to a fellow programmer
	- Does it speak in terms of the domain problem
	- Would a new person joining the team be able to understand it, and work with it effectively
- Makefiles are powerful tools that let us configure commands to be run in the project, mostly for compiling, running, and so on
- These tools (`black`, `pylint`, `mypy`, and many more) can be integrated with the editor or IDE of your choice to make things eve easier. It is a good investment to configure your editor to make these kinds of modifications either when saving the file or through a shortcut
## Chapter 2 - Pythonic Code
- Magic methods are those surrounded by double underscores that Python uses to reserve special behavior
- Context managers are a good way of separating concerns and isolating parts of the code that should be kept independent, because if we mix them, then the logic will become harder to maintain
```python
# Before
fd = open(filename)
try:
	process_file(d)
finally:
	fd.close()

# After
with open(filename) as fd:
	process_file(fd)
```