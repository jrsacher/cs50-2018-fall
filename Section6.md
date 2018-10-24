[Slides](https://docs.google.com/presentation/d/1SxJ5zGLdUv6EQsWQ1ibzwhRUwVU58MP8ljavtqFMX5I/edit?usp=sharing)

[Programming examples](http://bit.ly/2q6b6qR)

[Attendance](https://docs.google.com/forms/d/e/1FAIpQLSe_1Lmef9IAXcrX0AWc4ZOzgvYnPhB_F7i3wSXDxln2cZpv1w/viewform?usp=sf_link)

[CS50 short on Python](https://www.youtube.com/watch?v=8xCzjOnfQbw&list=PLhQjrBD2T380Ze8wxWJBPgo2XZzYlnN0N&index=2&t=0s)

The [Python 3 documentation](https://docs.python.org/3/) should be a go-to resource!

Discussion on what it means to be ["pythonic"](https://docs.python-guide.org/writing/style/). Or, in a python interpreter, `import this`.

Fun things to build your (Python) programming skills:
* [Rosalind](http://rosalind.info/): Biology and bioinformatics based problems
* [Python Challenge](http://www.pythonchallenge.com/): Solve puzzles to get to the next clue

If you're curious, you can see how Staff [implemented cs50.py](https://github.com/cs50/python-cs50/blob/develop/src/cs50/cs50.py), where `get_string` and the like are defined.


### Question in section regarding `if __name__ == '__main__':` block
Python's [documentation](https://docs.python.org/3/library/__main__.html) has a bit to say about it, but it's a little cryptic. [This source](http://ibiblio.org/g2swap/byteofpython/read/module-name.html) clarified it a bit more for me.
#### (hopefully) simple version:
If a Python program is run from the command line, `__name__` is set to `'__main__'` as a default.
If a Python program is incorporated via `import`, `__name__` is set to the file name itself.
>> A module can discover whether or not it is running in the main scope by checking its own __name__

Translation: `if __name__ == '__main__':` checks if it is being run from the command line.
