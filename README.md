# Flask Learning Examples

A collection of beginner Flask applications demonstrating routing, templates, forms, static files, template inheritance, and a small JSON API.

## Contents

| File or folder | Description |
| --- | --- |
| `app.py` | Routes, a student-mark average form, pass/fail redirects, and a JSON sum API. |
| `Eg.py` | Registration form and confirmation page example. |
| `hyperlink.py` | Two-page navigation example. |
| `image.py` | Serves a page with a static image. |
| `inherient.py` | Template inheritance example. The filename preserves the original project spelling. |
| `templates/` | HTML templates used by the Flask applications. |
| `static/download.jpg` | Image displayed by `image.py`. |
| `templates/test.jaon` | Sample JSON data retained from the original project. |
| `requirements.txt` | Python dependency list. |

## Setup

Use Python 3.9 or later. In a terminal opened in this folder:

```bash
python -m venv .venv
```

Activate the environment on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

Then install the dependency:

```bash
pip install -r requirements.txt
```

## Run an example

Start one application at a time. For the main routing and form example:

```bash
python app.py
```

Open the local address shown in the terminal (normally `http://127.0.0.1:5000`). Try:

- `/` for the welcome page
- `/form` to calculate an average score
- `/success/80` or `/fail/40` for route-parameter examples

The JSON API accepts a `POST` request at `/api`:

```json
{"a": 10, "b": 20}
```

Run the other lessons with their filename, for example `python image.py`.

## GitHub notes

The virtual environment is intentionally excluded. Create it locally using the setup steps above. The GitHub-ready copy also fixes the JSON parsing and calculation in `app.py`.

## License

Add a license before publishing if you would like others to reuse or modify this project.
