# Hands-on: Deep Learning and CNN

## Slides and Source Code

**Nearly everything is originally from Stanford CS231n under MIT License**. Especially I didn't make most of the slide content, they are from excellent talks / papers / study notes and I carefully cite their works.

I modified all code to be PEP8 compliant and Py3k compatible. In addition, most of the practices are shorter to fit in an one-hour talk.


## Envorinment Setup

### Root Python version

Recommend to use [miniconda3] or Anaconda3 (they are same in essence). This should work on Windows, Linux, and OSX.

I target for Python 3.4+ but should be fine on Pyhton 3.3. **Never ask me how to run on Python 2.7.** ...okay, the original source runs on Python 2.7 and I simply change some library import path and classic 2vs3 difference.


### (Skippable) Setup using pyenv

You can use [pyenv] to manage multiple Python versions without breaking the system-wide setting. Follow pyenv's readme to set up, which has been tested to work on Debian, Ubuntu, and OSX.

```bash
# under this repo root
pyenv install miniconda3-3.8.3
pyenv local miniconda3-3.8.3
```

Now all `python` command under this repo root use miniconda's python, which can be checked by

```bash
pyenv which python
# ~/.pyenv/versions/miniconda3-3.8.3/bin/python
python
# Python 3.4.3 |Continuum Analytics, Inc.| (default, Mar  6 2015, 12:07:41)
# ...
# >>>
```

### Python virtual environment

(Mini)conda handles the virtual environment itself. It is powerful and makes everything simple for numerical computing packages.


```bash
conda create -n dnn python=3.4 \
	numpy cython            \
	matplotlib              \
	ipython-notebook
```

Activate and deactivate the envrionment is easy,

```bash
source activate dnn      # activate
deactivate               # deactivate
```

[pyenv]: https://github.com/yyuu/pyenv
[miniconda3]: http://conda.pydata.org/miniconda.html
[mkl]: https://store.continuum.io/cshop/mkl-optimizations/


### Init the dataset
(TODO)

## License

The slide is powered by

- [shower.js]: HTML5 slideshow framework by Vadim Makeev *et al.*, under MIT license
- [highlight.js]: Syntax highlight library by Ivan Sagalaev *et al.*, under MIT license

Unless explicitly stated,

- the content of the slides (at `slides` folder) is shared under Creative Commons 4.0 BY licesne.
- the code is shared under MIT license.

More information about license at [CC Attribution 4.0] and `LICENSE_MIT`.

[reveal.js]: https://github.com/hakimel/reveal.js
[shower.js]: https://github.com/shower/shower
[highlight.js]: http://highlightjs.org/
[CC Attribution 4.0]: https://creativecommons.org/licenses/by/4.0/