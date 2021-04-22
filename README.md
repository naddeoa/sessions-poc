
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

# Create a kernel for jupyter for this env
python -m ipykernel install --user --name=guest-session-demo

# Run jupyter and open the Guest Session Demo notebook
# NOTE: remember to switch to the guest-session-demo in your notebook
jupyter notebook Guest\ Session\ Demo.ipynb
```
