# Introduction to AI

The introduction to AI and neural networks course is aimed at the Python programmer who wants to learn how to apply deep learning to data problems.

## How to use the course materials

The course materials can be read online [on the course website](https://bristol-training.github.io/intro-to-ai/).

To run the code on your own machine, [follow the setup instructions](https://bristol-training.github.io/intro-to-ai/setup.html).

You can also access individual pages from the course as [Juypter notebooks](./notebooks).

## Making changes to the course

We are happy to receive issues or pull requests for this course.

Please install [nbstripout](https://pypi.org/project/nbstripout/) before you commit any changes, to ensure that output is stripped from the notebooks before Git sees them.
If you're using uv, this should be as simple as:

```bash
uvx nbstripout --install
```

We use [Quarto](https://quarto.org/) to build the website, and this happens automatically when you push your changes back up to GitHub, via a [GitHub Action](https://github.com/Bristol-Training/intro-to-ai/blob/main/.github/workflows/publish-page.yaml).
To preview your changes locally before committing/pushing, install Quarto and then run:

```bash
uv run quarto preview
# or
uv run quarto preview --no-execute
# to skip running the python code in the notebooks
```

## License

This content is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0), unless specified otherwise.

To view a copy of this license, visit https://creativecommons.org/licenses/by/4.0/
