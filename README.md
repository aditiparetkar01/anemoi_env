
# Anemoi environment

Pinned pip environment captured from a venv on my laptop, for reuse on the HPC.

## Recreate

    python -m venv anemoi_env          # use the Python version noted in the lock file
    source anemoi_env/bin/activate
    pip install -r requirements-lock.txt

torch may need reinstalling with a CUDA tag matching the target machine's
driver. Check whether the cluster provides its own torch build or requires
`module load cuda/...` first.
