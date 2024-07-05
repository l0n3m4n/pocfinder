
# Custom Templates
You can create a custom templates as many as you can 
```bash
# Structure directories for custom templates
.
├── CVE-2024-4577_Sample.html
├── README.md
├── pocfinder.py
├── requirements.txt
└── templates
    ├── custom_templates.md
    └── report.html

2 directories, 6 files
```
## Custom Templates
All custom templates must be report.html name
```py
def save_to_html(exploit_info, filename):
    """Save into cyberpunk font HTML report."""
    try:
        current_dir = os.path.dirname(os.path.abspath(__file__))
        template_path = os.path.join(current_dir, 'templates', 'report.html')# modify and add path to your custom templates
```