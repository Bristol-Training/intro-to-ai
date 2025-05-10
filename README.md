# Introduction to AI

Course material for introduction to AI and neural networks, mostly being run by Huw Day.

## Course materials

The course notebooks are in the [`notebooks`](./notebooks/) directory.

## Run on your own machine

> [!NOTE]
> ### Windows users
> Install Git and Git Bash first, unless you are using Windows Subsystem for Linux (WSL). You should be able to do this by running the following command in command prompt or Powershell:
>
> ```shell
> winget install --id Git.Git -e --source winget 
> ```
>
> If this doesn't work, then [follow the instructions on the Git website](https://git-scm.com/downloads/win).

1. **Open a terminal** (or Git Bash)

2. **Install `uv`** by running:

    ```shell
    curl -LsSf https://astral.sh/uv/install.sh | sh
    ```

    Close and re-open your terminal, if the installer requests this.

    If you already have `uv` installed, then upgrade to the latest version before continuing by running `uv self update`, or by upgrading through whatever means you used to install `uv` originally (for example, Homebrew users would run `brew upgrade uv`).

3. **Download the course content**:

    ```shell
    git clone https://github.com/Bristol-Training/intro-to-ai
    cd course
    ```

4. **Check your PyTorch version**:

    ```shell
    uv run python -c "import torch; print(torch.__version__)"
    ```

    This command will automatically download the version of Python and all the Python libraries that are required for the course.

5. **Run Jupyter Lab**:

    ```shell
    uv run jupyter lab
    ```

    In future, just re-run this command to get access to the course again.
