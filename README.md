## What is it?

This is a ZSH plugin that enables you to use OpenAI's powerful Codex AI in the command line. OpenAI Codex is the AI that also powers GitHub Copilot.
To use this plugin you need to get access to OpenAI's [Codex API](https://openai.com/blog/openai-codex/).


## How do I install it?
### Manual Installation
1. Install the OpenAI package.
```
pip3 install openai
```

2. Download the ZSH plugin.

```
git clone https://github.com/hewhomustnotbenamed/ai_autocomplete.git ~/.oh-my-zsh/custom/plugins/ai_autocomplete 
```

3. Add the following to your `.zshrc` file.

Using oh-my-zsh:
```
    plugins=(zsh_codex)
    bindkey '^X' create_completion
```

4. Create a file called `openaiapirc` in `~/.config` with your ORGANIZATION_ID and SECRET_KEY.

```
[openai]
organization_id = ...
secret_key = ...
```

5. Run `zsh`, start typing and complete it using `^X`!