
This is a demo notebook that shows how anonymous sessions work in whylogs. There
is a sample that uses a dataset from Kaggle that should be easily adapted to
other datasets.

## Setup

The project is just a requirements.txt file for pip and a notebook. Setup
whatever python environment you prefer, install dependencies, and open the
notebook.

```bash
# If you're using virtualenv
virtualenv env
source env/bin/activate

# Install the dependencies
pip install -r requirements.txt

# Run jupyter and open the Anonymous Session Demo notebook
jupyter notebook Anonymous\ Session\ Demo.ipynb
```

## Caveats

This is very much in development. There are a few things to keep in mind while
testing this.

- There isn't a lot of feedback while whylogs is uploading profiles to WhyLabs. Depending on the amount of data it may take a minute or so.
- There is a minimum of 4 days of data right now. If you use this feature on a dataset with fewer days or without a notion of time then it won't work. A workaround for the later case is to just log it 4 times with fake timestamps for the past 4 days.
- We'll spit out a link to `hub.whylabsapp.com` but it should actually point to `observatory.development.whylabsdev.com`, so you'll have to substitute that in manually.
