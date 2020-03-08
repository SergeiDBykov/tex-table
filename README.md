# tex-table
Here you can find a python script for creating LaTex-styled cells in a pandas dataframe. It also helps you to write values with errors (upper and lower) with LaTex style features. 

The core code is in 'pandas_to_tex.py', while an example of usage is in 'pandas_to_tex_demo.py'. The program demands a dataset, which is provided for out example (sample_data.txt). A files of different types are in '.tex' format.

Assuming you have table in CSV or text format with columns named like: "par", "par_lo", "par_hi" and others, e.g., "statistics", "exposure", "obsIds" etc. 

Some of the columns you can keep unchanged with or without any formating (e.g. the latter column names), but for estimated parameters it will look like: " $par^{+err1}_{-err2}$ ", where err1 = par_hi - par, err2 = par - par_lo
