# Evals

This is the clone of the following OPENAI evals repo: [https://github.com/openai/evals](https://github.com/openai/evals).

With Evals, we aim to make it as simple as possible to build an eval while writing as little code as possible. An "eval" is a task used to evaluate the quality of a system's behavior. To get started, we recommend that you follow these steps:

## Setup

To run evals, you will need to set up and specify your OpenAI API key. You can generate one at <https://platform.openai.com/account/api-keys>. After you obtain an API key, please search and replace the string 'API_KEY' in the code with your own key.

**Minimal Required Version: Python 3.9**

### Making evals

If you are going to be creating evals, we suggest cloning this repo directly from GitHub and installing the requirements using the following command:

```sh
pip install -e .
```

Using `-e`, changes you make to your eval will be reflected immediately without having to reinstall.

### Running evals

```sh
oaieval gpt-3.5-turbo test-jee-match
```

If you want to reduce the number of threads that are run concurrently (default is 10) - to avoid rate limiting errors - run the following command:

```sh
EVALS_THREADS=1 oaieval gpt-3.5-turbo test-jee-match
```
