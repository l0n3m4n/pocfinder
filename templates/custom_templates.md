
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
    """Save into cyberpunk looking HTML report."""
    try:
        current_dir = os.path.dirname(os.path.abspath(__file__))
        template_path = os.path.join(current_dir, 'templates', 'report.html') # just modify and add path to your custom templates
        total_entries = 0  
        
        with open(template_path, 'r', encoding='utf-8') as template_file:
            template = template_file.read()

            template = template.replace('{{ description }}', exploit_info['description'])

            entries_html = ''
            for file_type, urls in exploit_info['entries'].items():
                for url in urls:
                    entries_html += f"<tr><td>{file_type}</td><td><a href='{url}' target='_blank'>{url}</a></td></tr>"
                    total_entries += 1 

            template = template.replace('{{ entries }}', entries_html)
          
        with open(filename, 'w', encoding='utf-8') as html_file:
            html_file.write(template)
        print(f"{Fore.LIGHTGREEN_EX}Data saved to {Style.RESET_ALL}{Fore.LIGHTBLUE_EX}{filename}{Style.RESET_ALL}\n{Fore.LIGHTGREEN_EX}Total Entries: {Style.RESET_ALL}{Fore.LIGHTBLUE_EX}{total_entries}{Style.RESET_ALL} {Fore.LIGHTGREEN_EX}out of{Style.RESET_ALL} {Fore.LIGHTBLUE_EX}20{Style.RESET_ALL} {Fore.LIGHTGREEN_EX}entries display on terminal{Style.RESET_ALL}")
    except FileNotFoundError as fnf_error:
        print(f"{Fore.RED}Error: File not found - {fnf_error}{Style.RESET_ALL}")
    except IOError as io_error:
        print(f"{Fore.RED}Error: IO error - {io_error}{Style.RESET_ALL}")
    except Exception as e:
        print(f"{Fore.RED}Error saving to {filename}: {e}{Style.RESET_ALL}")
```