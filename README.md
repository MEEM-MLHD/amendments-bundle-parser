# Amendments bundle parser

A Python 3 utility that parses PDF of amendments bundle coming from http://www2.assemblee-nationale.fr/recherche/amendements and outputs a list of json objects containing the following keys:

- `number`: amendment number
- `authors`: authors of the amendment
- `article`: target law project article
- `text`: text modification (the amendment)
- `reason`: the reason of the amendment

## Install

(pip 9.0.1 works)

```
pip install amendments-bundle-parser --process-dependency-links
```

## Usage

Common use (output to a json file)

```
amendments-bundle-parser.py <amendments.pdf> > <amendments.json>
```


Generic use (output to standard output)

```
amendments-bundle-parser.py <amendments.pdf>
```

License : BSD (3-Clause)