# Kofax RPA Connector - levenshtein_distance
Kofax RPA Connector is specific add-on to RPA, which can be used to implement missing features.
This specific connector uses Levenshtein algorithm to calculate similarity between two strings and return the similarity in percentage.

Connectors in general have some limitations, like the output number can't be decimal, so the output similarity range is integer between 0 and 100.

# How to add connector to RPA
Here is an explanation directly from Kofax, how to upload and use finished connector: https://docshield.kofax.com/RPA/en_US/11.4.0-vcsft2fhaw/help/rpa_help/help_main/designstudio/c_das_customactionstep.html

Here is my simple explanation:
1) Copy the connector file to any folder in your project (via File explorer) and synchronize the project with Management Console.
2) Open your robot and via Desktop Automation add new step called "Integration" → "Custom Action".
3) When everything is ok, you'll be able to select "Levenshtein distance" connector from the drop-down list with one Action "distance".
4) It has two inputs "String 1" (Text) and "String 2" (Text) and one output "Similarity" (Integer)
