# Data Dictionary

## Dataset
Combined Tennessee Eastman Process (TEP) workbook collection from `TEP00.xlsx` through `TEP10.xlsx`.

## Rows and labels
- Number of files: 11
- Total rows after concatenation: 4881
- Fault labels: `fault_id = 0..10`, derived from the workbook filename.

## Columns
- Original raw variables: `x_01` to `x_53`
- Dropped constant variables across the combined dataset: x_46, x_50, x_53
- Additional engineered metadata columns:
  - `fault_id`
  - `source_file`
  - `time_index`

## Modeling target
- For supervised classification tasks, `fault_id` is the target.

## Notes
- Workbooks were read with `header=None`.
- Constant columns are removed before modeling.
