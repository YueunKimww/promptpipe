# promptpipe

Tiny streaming CLI for OpenAI-compatible chat APIs

## Examples

```bash
chatsh explain this error < error.log
cat diff.patch | chatsh review this diff
```

## Install

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=sk-...
```

## Highlights

- Works with any OpenAI-compatible endpoint
- Model and system prompt via flags or env
- Reads the prompt from args or stdin
- Streams tokens as they arrive

## Project structure

```text
├── docs/
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── chatsh.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT - see [LICENSE](LICENSE).
