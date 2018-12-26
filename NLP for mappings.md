
We could look at what it would look like to use natural language processing to make predictions for new mappings based on the data available in the `configuration.mappings_id` and `configuration.mappings_text` tables.

## What Success Would Look Like

  - Use an set of examples (e.g. discipline - reasons student was disciplined) mapping to test what it would look like to predict the correct mappings
  - Put together a report with thresholds as examples of the different implications of different levels of prediction
    - Walk the data team through what it would / could look like
    - Determine as a group whether it's something we can safely pursue
  - Build a module/task which we could use^ to convert new mappings from -9 / "error" to a valid value

^ Something we'd need to consider is whether the process of using the module would occur in airflow as a task (after handling uploads of mappings), or as part of the dcpcsb/etltools> package.

## Resources

  - [fuzzywuzzy](https://github.com/seatgeek/fuzzywuzzy)
