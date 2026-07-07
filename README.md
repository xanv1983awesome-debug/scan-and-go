# Scan & Go — hosted shell

Installable PWA shell for a personal bin-to-bin inventory scanner (Receive / Pick FBA /
Move), served over HTTPS so the iOS camera scanner works.

**No inventory data lives in this repo.** The product catalog is loaded on the device
from a local `Data_master.csv` (☰ item-count badge, top right → *Load Data_master.csv…*)
and persists in the browser's localStorage. Bin locations embedded here are furniture
labels only; new/renamed bins are learned automatically from the loaded CSV's
`Bin Location` column.

Built from a local master copy; regenerate with the owner's `build_shell.py` (strips the
embedded catalog and asserts no product data leaks into the output).

Not intended for general use — schema and workflow are specific to one Excel/VBA
inventory system.
