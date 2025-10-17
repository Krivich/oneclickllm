# #OneClickLLM

A lightweight, browser-friendly protocol for secure per-user API key delivery from LLM providers.  
Users don’t need to know what an LLM or token is — setup happens in one click.

🔗 **Official site**: https://krivich.github.io/oneclickllm/

## Language versions

- 🇷🇺 **Russian**: https://krivich.github.io/oneclickllm/#ru
- 🇺🇸 **English**: https://krivich.github.io/oneclickllm/#en
- 🇨🇳 **Chinese**: https://krivich.github.io/oneclickllm/#zh

All links are stable and work immediately.

## Goal

Simplify LLM integration for open-source and enterprise tools by eliminating manual token copying. The protocol enables:
- **User simplicity**: no technical knowledge required,
- **Security**: token may never leave the user's browser,
- **Reliability**: no copy-paste errors,
- **Provider control**: issue tokens only to verified apps.

## How to support

If you’re an LLM provider (OpenRouter, SambaNova, Mistral, etc.), please consider implementing this flow:

1. User is redirected to your setup page:  
   `https://your-provider.com/setup?client=AppName&redirect_uri=https://app.com/`
2. After login, you redirect back with a token in the URL hash:  
   `https://app.com/#token=sk-xxx&model=...`

This requires no backend on the app side and works on GitHub Pages, static sites, and offline apps.
