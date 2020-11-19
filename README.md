## Minted.com Address Book Export
My fiancée and I were just under 100 days until our wedding and I was trying to export the addresses that we had previously saved to [minted.com](https://minted.com) from our Save the Dates, but was dismayed to learn that there was no export feature! 
So I built a Python script to effectively export the saved address book.

Check out my [blog post](https://medium.com/@willkarnasiewicz/wedding-planning-meets-hacking-1c95be79035e) for more info.

## Getting Started
1. Assuming you have [Python 3.6+](https://www.python.org) and a [GitHub](https://www.github.com) account, clone the repo:

```bash
git clone https://github.com/wkarney/minted-export.git
```

2. Navigate into the repository you just cloned:

```bash
cd minted-export
```

3. Start a virtual environment:

```bash
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

>You can deactivate the virtual environment with `deactivate`.


4. Export your Minted address book:

Before getting the addresses, you'll need to have your Minted login credentials handy. 
It might be helpful to add them as environment variables called `minted_email` and `minted_password`, respectively. Or simply run the script and input them when prompted.

To run the script:

```bash
python minted_api_request.py
```

Running the above will scrape all of the events and output the address book fields as csv and xlsx file into a new `data/` dir of the project.

### Need Assistance?
Are you running into an issue and don't know what to do next? Write a comment in [this issue feed](https://github.com/wkarney/minted-export/issues/4) and I'll help you get it sorted.

### Improvements & Suggestions
Experienced developer with comments or tweaks? Fork the repo and file a pull request with your changes.
