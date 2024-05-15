---
layout: post
title: "MaraudersMapAI: Encrypting AI Prompts in Images with Python Steganography"
date: 2024-01-27
categories: [AI, Coding Projects, Cybersecurity]
tags: [python, encryption, steganography, ai, chatbot]
image: assets/images/81.png
---

# MaraudersMapAI: Mischief Managed

*I solemnly swear that I am up to no good.*

Welcome to the hidden chambers of the Enigmatic Codex, where the art of concealing and revealing secrets mimics the mysterious charm of the Marauder's Map. This Python project combines the power of Fernet encryption and steganography to hide information within images. I took it a step further by using this technique to keep the system prompt for an AI chatbot hidden and encrypted, ensuring that the prompt remains secure and undisclosed to prying eyes.

## Overview

Discover the tools to encrypt your most confidential messages (`mischief_managed.py`) and unveil secrets hidden within plain sight (`marauders_map.py`). Like the Marauder's Map, these scripts guard your secrets and reveal them only to the worthy.

## Features

- **Mischief Managed (`mischief_managed.py`)**: Encrypt and conceal messages within images, akin to hiding secret rooms within a castle.
- **Marauder's Map (`marauders_map.py`)**: Reveal the hidden messages, similar to uncovering hidden footsteps in the corridors of Hogwarts.

## Integration Guide

### Preparing Your Secrets

1. **Prompt Preparation**: Utilize `prompt.py` to input the information you wish to encrypt. Edit `user_input` within this file:

    ```python
    user_input = ''' 
    Enter information to encrypt here. This will be the prompt for your AI system. 
    It can also be used to store other information, such as a password or a secret message or entire codebase.
    '''
    ```

2. **Clone or Copy Necessary Scripts**: Incorporate `mischief_managed.py`, `marauders_map.py`, and `prompt.py` into your project.

3. **Setup the `Prompt` Folder**: Ensure a folder named `Prompt` exists in your project, as `mischief_managed.py` uses an image named `output.png` from this folder.

4. **Environment Configuration**: Include a `.env` file in your project's root with the `SECRET_KEY`.

5. **Install Dependencies**: Use `requirements.txt` to install the necessary Python packages:

    ```sh
    pip install -r requirements.txt
    ```

### Using in Your Chatbot

1. **Encrypt and Hide Prompts**:

    In your chatbot script, import and use `mischief_managed` to encrypt and hide the contents of `user_input` from `prompt.py`.

    ```python
    from mischief_managed import encrypt_message
    import prompt

    encrypt_message(prompt.user_input)
    ```

2. **Reveal and Decrypt Prompts**:

    Use `up_to_no_good` from `marauders_map` to decrypt and retrieve the hidden prompt.

    ```python
    from marauders_map import up_to_no_good

    decrypted_prompt = up_to_no_good()
    # Use decrypted_prompt in your chatbot
    ```

## Notes for Usage

- This setup ensures your chatbot can securely manage prompts or sensitive information, echoing the discreet nature of the Marauder's Map.
- "Mischief Managed" clears all traces, maintaining the secrecy of your data.

## Epilogue

"As the corridors of Hogwarts hold secrets behind every portrait, your project now holds encrypted mysteries, waiting to be revealed only to those who know the magic words."

Mischief Managed.

---

Check out the [GitHub repository](https://github.com/ECTO-1A/MaruadersMapAI) for more details and to get started with your own Marauder's Map AI project.